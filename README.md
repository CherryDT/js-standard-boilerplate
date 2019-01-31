# js-standard-boilerplate

<a href="https://standardjs.com" style="float: right; padding: 0 0 20px 20px;"><img src="https://cdn.rawgit.com/feross/standard/master/sticker.svg" alt="Standard JavaScript" width="100" align="right"></a>

**Note: This readme file applies to `js-standard-boilerplate` only. If you expect to find the readme file for a different project here, please disregard this file.**

By David Trapp

This project can serve as an opinionated bare-bones boilerplate for new node.js projects using the [JS Standard](https://github.com/standard/standard). It is designed for use with:

* Windows 10 + Windows Subsystem for Linux
* VS Code in Windows
* node.js 10 in Linux (WSL)
* JS Standard

Features:

* Configured in a sensible configuration for Linux, but working well with VSCode in Windows.
  * In package.json, future npm script commands should be added in the same way as the existing ones, using `node .scripts/ensure_linux.js \"actual command here\"`. The idea is that this will always run those commands in WSL, and if started from Windows (e.g. by VSCode), they will run themselves inside `bash.exe`.
  * Embedded console in VSCode will use WSL Bash.
* Configured to use JS Standard and enforce it using a pre-commit hook.
* Comes with a .gitignore which should cover the basic needs.
* The `package.json` is by default configured with `private: true` and `license: "UNLICENSED"` - you can always loosen it up.

This project is under the CC0 license. The `package.json` says otherwise but that's because it is part of the boilerplate for the projects it will be used with, it does not reflect the license of the boilerplate itself. Also, don't forget to change `README.md`, `LICENSE` as well as the package name in `package.json` when you use this boilerplate for a new project!
