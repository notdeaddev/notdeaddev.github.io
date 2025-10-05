# [NotDead.dev](https://notdead.dev) Web Site

![Build](https://img.shields.io/github/actions/workflow/status/notdeaddev/notdeaddev.github.io/deploy.yml)
![GitHub top language](https://img.shields.io/badge/language-Markdown-blue)
![License](https://img.shields.io/github/license/notdeaddev/notdeaddev.github.io)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://notdead.dev/code-of-conduct.html)

Source repository for the Web site hosted at [notdead.dev](https://notdead.dev).

## Build instructions

This is a simple Maven documentation project. Build with:

```bash
mvn site
```

## Deploy instructions

Anything merged in the `main` branch is automatically deployed in GitHub Pages.

## License

License is MIT. Each source file must include the MIT header (build will fail otherwise).
To update source files with the proper header, simply execute the below command:

```bash
mvn license:update-file-header
```
