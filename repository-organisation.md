## General principles

###Organize by Application and Library
Repositories should be organized on an application, or library level.


###Keep unique dependencies with their project 
Any dependency that is unique to a project should reside in the same repository as teh project.

The benefits are:

* Exponentially less devops workflow overhead: if you split up unique dependencies into many repositories, any time you update one, you will usually need to update others. In functional programming based systems (like Nix) managing within one codebase can allow you to write specifics once, and inherit or re-use in many places. This can cut down on lines of code, and complexity of managing projects. Lowering the complexity can also translate into more reliable software overall.
* It is easier for most people to track and hold fewer concepts in their minds.
