# nhood: Contributing to nhood Engine

Thank you for reading this guide. It means you want to help in development of `nhood` project and you know where to start. We are looking for your help.

## How can I contribute?

### By reporting issues

Did you find a bug? Is there a feature you want in nhood-engine? Simply create a new issue in corresponding repository.

* Ensure the bug or similar feature was not already reported.

* If you're unable to find an open issue addressing the problem, open a new one. 

* Be sure you are following the templates:

    * [Bug template](./templates/bug-template.md)

    * [Feature template](./templates/feature-template.md)

* Be sure you are following issue naming with a clear description. Example: `Create contribution guide`.

* Feel free to contribute in issue discussions.

* When reporting an issue or taking part in discussion please follow the [Code of Conduct](#Code-of-Conduct).

### By implementing open issues

Feel free to follow list of [Open issues](https://github.com/nhood-org/nhood-docs/issues). Id there is an issue you are able to implement:

* Assign yourself to the open issue that is labeled with `help-wanted` and `read-for-development` or `bug`.

* Assign yourself to the issue only when sure you have time and you know how to implement it. If issue requires additional clarifications, feel free to open a discussion.

* Work in your own forked branch.

* Create a pull request when you implementation is complete:

    * Code fully covers bug-fix or feature with its acceptance criteria
    
    * Code is fully covered with:
        * unit testing
        * integration / component testing, when applicable
        * end-to-end, when applicable
        * tests are following existing testing conventions
    
    * Code is aligned with code style. We follow [Google Code Conventions](https://github.com/nhood-org/nhood-parent-bom/blob/master/checkstyle.xml)
    
    * Code change is minimal:
        * there are no excessive / duplicated logic implementations
        * there are no dependency duplicates
        * there is no additional refactoring or re-implementation (If you believe such is useful, create a separate issue)

    * Feature is documented in a way no further explanation is required

* Make sure you are following commit massage with a clear github-style change description. Example: `Fix invalid swagger configuration`.

* Assign at least one of the [Code Owners](./OWNERS.md) as reviewer. 

* Feel free to assign other contributors as reviewers as well.

* When opening a pull request please follow the [Code of Conduct](#Code-of-Conduct).

### By implementing minor changes

Minor changes like typos, docu updates may be implemented without opening an issue.

* Simply create a pull request with clear description of the change

* Assign at least one of the [Code Owners](./OWNERS.md) as reviewer. 

* Feel free to assign other contributors as reviewers as well.

* When opening a pull request please follow the [Code of Conduct](#Code-of-Conduct).

## Code of Conduct

When reporting and issue, taking part in issue or pull request discussion please:

* Use welcoming and inclusive language
* Be respectful of differing viewpoints and experiences
* Gracefully accept constructive criticisms
* Focus on what is best for the project and the community
* Show empathy towards other community members
