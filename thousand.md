Thousand Ideas for Computing
===

This is a summary of my ideas. My theme tends to be toward integrating technologies and existing ideas together.

## 1. Email Metadata

Emails could contain comprehensive metadata about the human readable content depending on the sort of email it is. This machine readable information could be interpreted metadata to:
 
 * display specialised interfaces for certain information
 * integrate and collect information together
 * enable contextual computing

For example:

 * view a list of your newsletter subscriptions, online invitations/requests, confirmed orders

Potential Integrations

 * HATEOAS for determining actions on an email
 * Life Engine
 * Living document
 * Contextual

Existing:
 
 * OpenEmailMetadata
 * [MailXML](http://www.idealliance.org/specifications/mailxml)

## 2. Decentralised Social Networking

The industry lacks an open social network. A DSN should support:

 * data privacy through permissions and encryption
 * ability to export content

Potential Integrations

 * Email metadata
 * Life Engine
 
 Existing:
 
  * [Diaspora](https://joindiaspora.com/), [BuddyCloud](http://buddycloud.com/), [Status.Net](http://status.net/), [SockNet](http://socknet.net/w/The_Socknet), Apple Seed, Freenet Sone
 
## 3. Community Idea: Design This

Developers need designers to give websites viable designs. This community brings developers with complete website backends and matches them with designers to give the backend a design.

## 4. Living Documents

Blogs, forums, wikis and social networks solve variations of the same problem. Unfortunately they are not integrated enough. Writing a post should allow me to take advantage of:

 * collecting arbitrary structured data from the recipient rather than just a freestyle comment box. Collect information *within* the article.
 * allow users to provide corrections (wiki functionality)
 * split up the document into reuseable components (wiki like transclusion)
 * renderers display data in multiple ways
 

## 5. Life Engine

Life engine is a dashboard that attempts to collect relevant information about your life into one place.

 * bank account balances
 * upcoming birthdays for friends
 * dream diary
 * family, friend member status
 * important emails
 * to-do list, goals, reminders, calendar integration
 * lent possessions

Existing:

 * business dashboards
 
 
## 6. Community Idea: Ethical Me

A tool to track the decisions of organisations and allow consumers to register their buying decisions in a thoughtful way.

## 7. Peer to Peer Blocking

Block by default is inconvenient to users. Community driven blocking reduces risk. Configuration options should be shareable and synchronizable to increase security.

 * Firefox Request Policy
 * Host file blocking
 * Firewall rule
 * Application behaviour
 
Potential Integrations:

 * web of trust, trust score for a people you know
 
Existing:

 * cloud based security providers, Site Advisor, 

## 8. Command Line Auto-complete

Command line auto-complete could be offered by:

 * indexing the man pages intelligently to extract argument documentation
 * typing a comamnd line searches the index for arguments and either displays completion of the argument and/or provides a documentation panel for that argument.

For example, if the user types `grep -v`, they may get an auto-complete for `--invert-match`.

## 9. Elements Represent Themselves

A rendering of data should stand-in and represent itself.

 * If you have an open program and see a filename in the title bar next to that file's icon, you should be able to interact with that name or icon in the same as you can elsewhere. For example, you should be able to move the file or rename it. You should be able to drag it into an open email.

 * If an application displays an IP address, a hostname, a filesize or some unit measurement, the user should be able to interact with these things with a tool that accepts these as arguments. Clicking a filesize may show where that space is being taken on the filesystem. Clicking an IP address may offer actions such as 'ping'. Clicking a unit measurement may show unit conversion tools.

Potential Integrations:

 * the environment has knowledge, representational computing
 
## 10. The Environment has Knowledge / Context-Aware Computing
 
Running applications expose information on what information they can provide and what they will accept. Bring type systems up into the desktop environment. Everything - including programs, have a type and have typed parameters. The system helps you fulfil type arguments for running programs:

 * You have window open that is requesting an IP address.
 * Your machine exposes an IP address and your VPN provides an IP address. Your online friends provide an IP address.
 * You can pick the IP address from the available sources without having to type it in.

Existing: 

 * Content Negotiation
 
Potential integration:

 * drag and drop is no longer handled specifically

## 11. Representational Computing

Representations are specific or generic. Completing a task has a representation, such as 'render image' and if requested will select a program depending on contextual criteria. If the input data is in PNG format then it must pick a program representation that can render PNG. The inputs and outputs of programs are representations themselves so the type matching works upon programs themselves.

RC is akin to a program requesting a library that provides 'X' and having that library injected in.

Existing:

 * Negotiation protocols
 * Type systems
 * Dependency Injection

 
## 12. The Package Manager-Package Manager

There are multiple package managers that have to be controlled with separate programs. Setting up a machine involves installing various package managers. It seems a hierarchy of package managers woud permit installing any number of packages.

 * package managers have consistent standard command-line API that lets them be driven by other programs to avoid special cases for package managers

## 13. Package Driven Development

Software complexity prohibits quick and repeatable set-ups. Software should be written to be packageable and repeateable from the very start.

 * Not only does software need testing but the packages do too.
 * Installing the package should be enough (minus configuration) to begin running software

Existing:

 * [Vagrant](http://www.vagrantup.com/)
 
## 14. Configuration Spider
 
Infrastructure is complicated and the relationships between hosts, paths, ports and servers create a web of complexity. Tools like Chef and Puppet help generate configuration files that programs can read. A configuration spider would allow detecting and connecting the relationships between these configuration files.

The spider would scan for configuration files, identify port numbers, paths and hostnames to insert into a graph. When the spider detects a reference to the same value, it creates an edge from both usages to the actual data. This graph then becomes a reprsentation of system configuration, the edges link the configuration values are live and synchronized, an administrator can change the data in a single location and cause the usages to update.

## 15. Community Idea: Create This

This is like the 'Design This' but in reverse. Designers create a design and a developer creates a backend to the site. Ideally suited to open source projects.

## 16. Team Fund

A group of people want to create something but do not have the time or energy to create it. They collaboratively decide what they want and raise funding.

 * users form committees to oversee the development effort
 * committees create 'open positions' as roles to fulfil
 * users who possess the required skills for a role offer to work
 * experts get paid, committee gets idea implemented

This is like a reverse kickstarter or a petition. Existing crowdfunding services
 
Existing:

 * Kickstarter, in reverse

## 17. Bubble Routing

Bubble routing is an approach to detecting and handling events on the clientside. Most frameworks do not use bubbling to its full potential, they create a handler for each area where an event needs to be handled and stop propagation once it has been handled. Bubble routing uses a single event handler by taking advantage of the natural structure of the DOM and bubbling. Each element the event passes through enhances the information of the request before it gets to the topmost level where the event is actually handled.

 * Example: http://fiddle.jshell.net/SWrX5/15/


## 18. Shortcut Format

Keyboard shortcuts are configured differently in each program. Shortcut configuration should be in a standard format.

## 19. Separating Frontends and Backends

Good design separates the frontend and the backend. This should be the case on the desktop too. If frontends and backends were separated, one could use the same underlying mail or instant messenger client but switch between frontends. Backends and Frontends would communicate according to some representation.

## 20. File Explorer Features

These are some features for file exploring programs I have always wanted. Some are already existing:

 * `Put in Folder` puts the selected content into a new folder
 * `Copy Path` why do I need to copy path if I can see the file
 
## 21. If you can see it, you can use it (SIUI)

This is the principle that if you can see some data on the screen, even in different window, you should be able to use it in your active program. On the command line, 'use it' means 'refer to it', such as the path of a file icon or a file path on the shell.

Take the output of git status for example:

```
# On branch master
# Changes to be committed:
# (use "git reset HEAD ..." to unstage)
#
# modified: hello.py
#
# Changes not staged for commit:
# (use "git add ..." to update what will be committed)
# (use "git checkout -- ..." to discard changes in working directory)
#
# modified: main.py
#
# Untracked files:
# (use "git add ..." to include in what will be committed)
#
# hello.pyc
```

If you want to refer to a file name in the above, you could type it out and use your shell's auto-complete functionality. You could copy and paste it with the mouse or your terminal multiplexer. You should be able to refer to paths mentioned directly.

 * A program puts the paths into environment variables. The output of the program is adjusted to add numberings such as:
 
```
# modified: hello.py [1]
```
 Now I should be able to refer to the 1 in some way, perhaps `$m1` now stands for 'modified file 1'.

 * Hint mode places an overlay over the interface and numbers various things on the screen to be clicked. (see vimperator hint mode)

Existing:

 * [Plan 9 ACME](http://doc.cat-v.org/plan_9/4th_edition/papers/acme/) (clicking certain strings has behaviour)
 * TermKit
 * Vimperator / [Pteradactyl](https://en.wikipedia.org/wiki/Pentadactyl_(extension)

## 22. Shell as REPL

An invocation of a program on the terminal and its output could be interpreted as an assignment to variables in the current scope. The output of the program should be useable to the user. The developer should be able to interact with the shell or the output in a language of choice.

For example,

```git status -s```

Gives me the status of each file and the filename. If I want to use this data in Javascript or in Ruby I have to parse this text manually. Ultimately the structural output of this command is this same every time. There is a list of structure data with a consistent format that could be idiomatically represented in many languages. In Javascript this could be:

```
{"file": "hello.py", "status": "modified"}
```

The output of the Git command should be treated like an object that has already been parsed and interactions are already possible.

```
output.modified[0].file
```
This could be implemented lazily so that the effort to parse the output is not made until the user attempts to access fields.

Shell operations may be simpler as programming constructs. This way one could use the shell programmatically, in different languages.

wget http://example.com/ |  
(require '[cheshire.core :refer :all])
(require '[clj-http.client :as client])
(let [input (parse-stream (io/reader *in*))]
	(client/post "http://localhost:8383/" {
		:query-params {(input "m") (input "l")}
	} )
)

Existing:

 * [Haskell shell scripting (Shelly)](http://www.yesodweb.com/blog/2012/03/shelly-for-shell-scripts)
 * TermKit

## 23. Live Data

The display of data - perhaps through widgets or in documentation should be synchronized when the underlying data is updated. When something is changed in one location, all views of that information should be updated.

For example:

 * You change a keyboard button setting in an application, the documentation should automatically update to show the active shortcut.
 * An application is customized to change its appearance. The `screenshots` in the documentation should update accordingly.
 * Applications that want something but cannot function such as an internet connection or are waiting input should know and continue when the desired state is restored.

Existing:

 * When a folder is open and a file is added, the file should appear in the folder.


## 24. Error to Issue Tracker Linkage

There should be some kind of mapping between the product's error state and a potential issue number. Currently the connection between an error condition and an issue in a tracking system is completely human - someone has to manually enter the error into an issue tracker. Bug reporting should either be intregrated into an application or interpreted by the desktop or container environment.

 * An graphical application facing an error condition typically report through a dialogue. This dialogue should display the known cases that cause this error. This is possible because Error Condition X was mapped to Issue Y which had associated Reason Z.

``` 
Error copying files: drive removed. Typically caused by:

 * Unplugging drive during copy 		[I didn't unplug it]  
 * Internet connection lost				[Diagnose internet connection]
```
```
 Compiler error: undefined is not a function (line 13)  
 	> A variable on Line 13 is undefined
 ```

## 25. Error Heuristics

Errors have numerous causes. Once an error becomes common enough and becomes common knowledge, it may not be justified to adjust the program to provide a better error mesage because the error is human. Separate tools can take advantage of heuristics can provide better insight to the problem. For a compiler error, this heuristic knows where to begin its search. These tools do not necessarily need to check if the error exists, they merely provide heuristics that help narrow down the problem. For example:

```
Line 13: user.mailboxes()[selectedMailbox].preferences: undefined is not a function
	> `user`, `mailboxes` could be `undefined`.
```

```
Error: install is not defined
 > This was reported as fixed in version 1.3	[Open update manager / run package-manager update x]
```

```
Expected ; saw }
 > Function expressions should be followed by a ;
 > Mismatching curly brackets, counted 4 {{{{ and 3 }}}
```

Existing:
 
 * Windows Reliability Problem and Reports
 * Brew Doctor
 
## 26. System-wide Data interpeters

There are many data patterns that are not explicitly marked up.

 * phone numbers
 * addresses
 * line numbers
 * units of time, standard measurements
 * paths, filenames, extensions, port numbers
 * system commands
 * standardized reference numbers
 * SHA, MD5 hashes
 * URLs
 * System or network usernames, hostnames

Data classification algorithms can be ran against the text displayed on terminals or within graphical programs. This could be deferred until the user interacts with the information, perhaps on mouse hover or clicking on the information.

 * Clicking

Existing:

 * Mailto links
 * Protocol handlers
 * Contextual computing / Representational computing

## 27. Applications Expose Data Visually and Programmatically

Information can be used to find relationships and connect actions that operate on this data. The desktop environment can forgo use of specialised libraries and instead communicate with the services provided by other programs.

 * An application or form on a website is requesting a piece of data. Data of the same type is also being displayed in another user interface. Selecting the input field will display a list of potential sources of this information, one being the active application.
 
 * An open folder manager window a folder open. This can be interpreted as a list of dates and times. A calendar program can read and display the sequence of dates and times to show when files were created/modified along a timeline. This may be useful with photographs.
 
 * A spreadsheet program is opened and contains a sequence of dates. When the user views a date in a different application or on a web page, the environment refers to the spreadsheet filename.
 
This functionality would be user driven as to avoid performance issues.
 
Existing:
 
 * Object Linking and Embedding
 * Wiki software

## 28. Representations, Interfaces and Tests

A representation dictates what you can do or how you can use it. A PNG file, a JSON or C sourcecode or a HTML file. An interface is validated by the tests that it passes. What something is can be determined by the tests that it passes.

 * A HTTP server supports the 'HTTP Protocol'. A HTTP server has an interface of HTTP methods over TCP. This can be verified by a test suite, perhaps one based on an RFC.
 * A sort algorithm can be stable or unstable.

The hard part is providing a mapping between a representation definition and the true interface. Tests

## 29. Community Idea: API Competition

Libraries compete on performance and API design. The representation of a problem stays the same but can be solved in multiple ways. For example:

 * an API for making HTTP requests
 * a query language for data
 * database backend query implementation
 * widget APIs
 * sort algorithms
 * client side web frameworks
 
Existing:

 * Js Perf
 * Benchmarks


## 30. Triple Architecture

Modern architecture splits web applications internally between a backend API and a web interface that communicates with the backend API. This is inadequate for designers.

 * Backend business logic
 * Creating widgets or website components
 * Organizing and placing widgets onto pages
 

## 31. Mounting Sourcecode

Sourcecode we compile or execute need not be the same as that rendered to the screen. Developers should be able to work on the same code base but view sourcecode in different ways. Mounting a source directory means we can apply bidirectional transformations between the stored sourcecode and what is opened in a text editor.

Coding style preferences can be configured on the mounted source code so that it appears according to the developer's taste. Developers can choose indention rules and spacing settings without affecting other developers.

Personal preference also changes how people like to organize sourcecode by directory. Many conventions such as the following

```
 - src
  - models
  - controllers
  - views
 - docs
``` 

Potential integrations:

 *  Easier userspace file systems

## 32. The Built-In Enemy

Users are not informed about security issues waiting to happen unless they:

 * read documentation properly
 * read start-up warnings
 * check mailing lists or online communities
 * update packages frequently

The 'Built-In Enemy' is a suite of heuristics that find security problems on a machine. Examples:
 
 * versions of libraries or running software
 * permission problems, the permissions of running applications (user, group)

Existing:

 * anti-virus software
 * [Secunia PSI](http://secunia.com/vulnerability_scanning/personal/)

## 33. Personal Infrastructure

Individuals lack personal infrastructure for photographs, videos, email or other services. User data is locked into assorted individual applications from vendors and service providers. A personal infrastructure is a set of machine instances or distribution of software that create a useful and serviceable infrastructure.

 * email server
 * catalogue, photograph management
 * backup provision
 * synchronization

Personal infrastructure providers could take the same approach as business hosting or cloud providers. They sell use of the infrastructure but provide value added services. This would be nice as an open source.
 
Personal infrastructure providers should start a trend where they provide not only the front end applications or web clients but provide direct access to the backend machinery hosted in the cloud. This would cater for power users and casual users.
 
## 34. Bluetooth Friend Mesh

Modern mobile phones are powerful and possess large unutilized CPU power. The resources available to a phone such as images, videos, maps, software and cached websites should be shareable in a mesh when people get physically close to one another.

 * People in the work place. Family members. Friends at a restaurant or a meetup.


## 35. Edit Servers: Team Active File Visualization

People working in the same area of software can cause problems where integrating changes is difficult. Decentralised source control systems mitigate integration pain but they do not actively help prevent it. As a user enters a file, the user's position, the following information is announced:

 * File level: file name, path, line number and column
 * Language level: method name, class, symbol name, module
 * Project level, functional area

Users can therefore be warned when a user attempts to update something that has also been changed by someone else. For example:   
 
 * A user opens a HTML template or XML file, this triggers an announcement that the file is open by a given user. If any other users then open this file, there is a list of users that also have this file open.
 * The current cursor position is indicated in the editor, perhaps in a certain color.
 * No warnings are raised unless changes are made.
 * When the user enters makes a change to a node in the HTML/XML file, this registers a change at this position in the file.
 * Any users who also enter this node will be warned about conflicts when they attempt to change the file.
 
This should permit multiple users editing the same file without tripping eachother up.

Existing:

 * any collaborative text editor such as Etherpad

## 36. Documentation Linked Code

Documentation and wikis are prone to fall behind a code base. Creating documentation from sourcecode or embedding documentation in the sourcecode are approaches to keeping documentation. Documentation and code should be linked together in such a way that it is difficult for it to fall out of date.

 * When code is visible in an IDE or in a text editor, the **relevant** documentation for this area should be quickly available to edit. This could be a panel, a tab or a split view that updates to always display documentation.
 * Documentation acts as a specialised test case. When example code in the documentation no longer compiles the build should fail.
 * Documentation should be linked to refactoring operations. When variables are renamed or code is moved, all the references to variables and methods should automatically update.

## 37. Code Overlays

Code overlays can make sourcecode more like a document and make it easier to understand. Source code editors make poor use of space when rendering code. For example:

```
someLongMethodName	(type identifier, type identifier, type identifier,
					type identifier, type identifier type identifier
					type identifier, type identifier, type identifier)
```
Code quality problems aside, an IDE does not necessarily need to display this exactly the way the source is. There is wasted space below the method name. An auto-indenter could align the source perfectly but this seems like catering to the plaintext format of sourcecode rather than the expressive power of a user interface. 

This could be rendered like a table:

`someLongMethodName`

Type |	Argument	| type	| identifier | type | identifier
-	 |	
type | identifier	| type | 	identifier | type | identifier
type | identifier	| type | 	identifier | type | identifier
type | identifier	| type | 	identifier | type | identifier

This does not necessarily rendered by graphical widgets, it could be rendered with `text widgets` that respond to


## 38. Code as a Wiki

Code is inherently linked and related. This is similar to wikis and the nature of hyperlinks and the web.

 * Code can be navigated as a wiki.
 * Edit code in the same style as a wiki.
 
## 39. Data Trails

The data on your screen has a trail of influence. Multiple sections of code are touched before output is displayed.

 * There is data displayed in a wdiget. Viewing the influences of this widget would show the source of the data such as the file, the API that was used, the connected database, the query that was executed.
 * An error is displayed, viewing the influences of this data will show what component the error was raised in and the configuration of that component.
