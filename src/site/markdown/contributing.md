keywords: contributor
description: NotDead.dev established some rules to make sure your contributions are valued properly.
<!--
  ╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲
  NotDead.dev
  ჻჻჻჻჻჻
  Copyright 2025 NotDead.dev
  ჻჻჻჻჻჻
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
  The above copyright notice and this permission notice shall be included in
  all copies or substantial portions of the Software.
  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
  IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
  FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
  AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
  LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
  THE SOFTWARE.
  ╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱╲╱
  -->

# Contributing

You have found a bug or you have an idea for a cool new feature? Contributing code is a great way to give something back to
the open source community. Before you dig right into the code there are a few guidelines that we need contributors to
follow so that we can have a chance of keeping on top of things.

<!-- MACRO{toc|fromDepth=1|toDepth=2|id=toc} -->

## Getting started

* Make sure you have a [GitHub account](https://github.com/join).
* Find the corresponding [repository on GitHub](repos.html).
* Submit a **GitHub issue** in the repository to request a change, **assuming one does not already exist**.
  * Clearly describe the issue including steps to reproduce when it is a bug.
  * Include screenshots and outputs whenever relevant.
  * If known, explain what should be changed to fix the problem.
  * If possible, specify how to test the new feature.
* [Fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) and check out your forked repository.

## Making changes

* Ensure your fork of the repository is up-to-date (use [GitHub's fork sync feature](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork), and pull to your local clone of the repository).
* Create a _topic branch_ for your isolated work, named `feature/short-description` (the name is prefixed with `feature/` even if your change fixes a bug).
  * Usually you should base your branch on the `main` branch.
  * A good topic branch name can be the GitHub issue id (#_nnn_) plus a short description, e.g. `feature/issue-53-fix-https-certificate`.
  * If you have submitted multiple issues, try to maintain separate branches and pull requests.
  * Check our [branching model](branching.html) for more details.
* Make commits of logical units.
  * Make sure your commit messages are meaningful and in the proper format. Your commit message should contain the key of the GitHub issue.
  * Example: `Issue #53: Changed the implementation of the keystore`
* Respect the original code style (tabs, spaces, line width, etc.):
  * Create minimal diffs -- disable _On Save_ actions like _Reformat Source Code_ or _Organize Imports_. If you feel the source code should be reformatted or refactored somehow, create a separate PR for this change first. **Smaller changes are more likely to get approved by reviewers!**
* Make sure you have added the necessary tests for your changes.
* Run all the tests **before** submitting a PR to ensure nothing else was accidentally broken.
* Build the project site (if any) and verify the configured code quality reports (in the **Project Reports** section).

### Making trivial changes

Cosmetic or trivial changes in a project, like indentation, white spaces, typos, or minor refactoring **don't require** creating a dedicated GitHub issue, but they must not be mixed with other significant changes: a separate commit and separate Pull Request must be submitted.

In this case, the _topic branch_ should be named `trivial/short-description`.

## Submitting changes

* Push your changes to a topic branch in your fork of the repository.
* Submit a _Pull Request_ (PR) to the corresponding repository in the `notdeaddev` organization.
  * Verify _Files Changed_ shows only your intended changes and does not include additional files or changes like white spaces, etc.
  * Make sure all automatic checks are successful.
  * Verify comments produced automatically by code quality automatic checks.
* When implementing additional changes after reviewers suggestions, simply commit and push such changes. **Never squash or rebase commits that you have already pushed!**
* Once your PR is merged (if approved), [sync your forked repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork), pull these changes to your locally cloned repository and delete your branch.

Happy coding! 😊

## Additional resources

* [Git Branching Model](branching.html)
* [General GitHub documentation](https://help.github.com/)
* [GitHub pull request documentation](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
