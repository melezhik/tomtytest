# TomtyTest

Integration and blackbox testing service for Raku modules.

# TomtyTest Features

* Black tests are written on Tomty/Sparrow6 Task Check DSL - see this [post](https://dev.to/melezhik/simple-blackbox-testing-with-raku-and-sparrow6-g32) for details

# Benefits for modules authors

* You'll get extra tests for your module get run on a **separate** service
* You'll get **notified** upon tests failure. You'll be able to see a detailed report
* You'll get a nice **badge** similar to the Travis build with the status of the the last tests and link to the test report
* As Sparrow6 has a very good integration with Bash/Powershell so **command line utilities** authors could tests their tools much easier then it could be done with conventional test frameworks, with minimal code and under **Linux/Windows**
* You can create **integration tests** as well, for example some modules depend on external libraries, so on. [Sparrow6 DSL](https://github.com/melezhik/Sparrow6/blob/master/documentation/dsl.md) has a preset of functions for common system, configuration management tasks - installing packages, services and managing users, so on and could be used to prepare environment for your tests

# How do tests change my module development life cycle?

* The change is delicate and does not affect your usual development habits
* You place tests under `.tomty` folder and notify the TomtyTest maintainers you want to run tests with the Service, providing them with a module name and a module github source code URL   
* Tests get run separately from your conventional workflow (Travis/unit tests during zef install ) and do not burden your development cycle
* **You're not tied to the TomtyTest**, if something goes wrong ( the service goes down or you're decide not to use it anymore ) - nothing has to be done, you just notify the service maintainers and they  remove your module from a check list. Or you just remove `.tomty` folder from your source code.

# Who write tests?

* So far I'am probably the only person who use Sparrow6/Tomty so if you notify me here through comments I'd create a simple test suite for your module and you'll get understanding how to write tests. However the Tomty/Sparrow6 tool is quite simple and has a low learning curve so you could start writing tests very soon

# Benefits for TomtyTest service*

\* ( well for me ;=), but also for everyone! )

* Tomty/Sparrow6 will get a great opportunity to grow through the usage across many Raku modules
* Eventually Raku community will get an alternative testing service available for everyone 

# Suggested modules

* your module comes here 

# Conclusion

This is just a draft of the idea.

I'd like to see your comments. If you're interested in testing your module you can mention a module name in PR to this repository or by an email.

Thank you.

Aleksei
