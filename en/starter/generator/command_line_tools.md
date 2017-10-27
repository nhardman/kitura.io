---
### TRANSLATION INSTRUCTIONS FOR THIS SECTION:
### TRANSLATE THE VALUE OF THE title ATTRIBUTE AND UPDATE THE VALUE OF THE lang ATTRIBUTE.
### DO NOT CHANGE ANY OTHER TEXT.
layout: page
title: Command-line tools
menu: starter
lang: en
redirect_from: "/starter/generator/command_line_tools.html"
### END HEADER BLOCK - BEGIN GENERAL TRANSLATION
---

<div class="titleBlock">
	<h1>Command-line tools</h1>
	<p>This article summarizes Kitura CLI tool commands for generating servers.</p>
</div>

For MacOS, the `kitura create` and `kitura init` are the commands provided to allow the generation of a kitura server.
The generator is an [npm](https://www.npmjs.com) module using the [Yeoman](http://yeoman.io/)
library. This means that the generator is a plugin that is executed using the `yo` command-line
front-end to Yeoman. Use the [installation instructions](installation.html) to ensure the
generator and its prerequisites are installed correctly.

> ![info] Note: The generator is also available indirectly using:
>
> * [IBM API Connect toolkit CLI](https://www.ibm.com/support/knowledgecenter/en/SSMNED_5.0.0/com.ibm.apic.toolkit.doc/capic_swift_overview.html) via `apic swiftserver`  
> (uses v1.0.4 of the generator).
> * [Bluemix CLI Developer Plug-in](https://console.ng.bluemix.net/docs/cloudnative/tutorial_web.html#tutorial/) via `bx dev create`  
> (only supports scaffolded applications).


`kitura create` will display a series of prompts asking questions that define what
application will be generated. Once all questions have been answered, the project
directory and files will be written to the filesystem. Then the application will
be built using `swift build`.

*Table 1. Available commands*

| Command                           | Command type                                   | Description                                                                                                                                                                                                                                                            |
|---------------------------------  |------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **`kitura init`**              | [Application generator](#application-generator) | Create a new Swift Server application with default options selected.                                                                                                                                                                                                                       |
| **`kitura create`**              | [Application generator](#application-generator) | Create a new Swift Server application.                                                                                                                                                                                                                       |
| **`kitura create <modelname>`** | [Model generator](#model-generator)             | Add a new model to a Swift Server Generator CRUD application.                                                                                                                                                                                                               |

> ![info] For Linux see [linux tools](command_line_tools_for_linux)

[info]: ../../../assets/info-blue.png
[tip]: ../../../assets/lightbulb-yellow.png
[warning]: ../../../assets/warning-red.png
