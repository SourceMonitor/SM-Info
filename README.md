# SourceMonitor Information

The developer of [SourceMonitor], [Jim Wanner], is retiring from software development. The software will become open source and a new home at GitHub.

The repository is not public at the moment because of licensed code. This is required until the licensed code is replaced. Then we're able to start with a clean and public repository without the licensed code.

If you want to join the team, please contact me [here][email].

## Support needed

- C/C++ developers to maintain the code
- Know how for GitHub automation
- Know how for HelpFiles (\*.chm at the moment, something else for the future?)
- Know how for creating tests
- Know how for git pages
- Know how for [Inno Setup][inno]
- Replacement of licensed code with open source code

## The proposed steps/roadmap

- Remove Campwood related parts like
  - ~~Paths~~
  - ~~Registry keys~~
  - ~~(C)-Notes~~
    - Except for the graphic classes done - this classes will be replaced.
    - Except for the grammar files - new grammars and parsers will come with the parser replacement.
- Get rid of the licensed code either by creating own or use of public licensed code as substitution.
- Start with a clean and public repository without licensed code.
- Get rid of proprietary and licensed software for building SourceMonitor - this affects the parser and will maybe result in a replacement with something else, e. g. [ANTLR4][antlr].
- Enable a 64-bit version of the software with the goal of better usage of the provided OS/hardware resources.
- Seperate the UI from the code to become the software running on different plattforms like MacOS, Linux and Windows. Maybe a WebUI is possible?
- In case the software will run on different OS, there is a need for another installer.
- Parallel a constant refactoring of the software is required. While this process is running tests for the software have to be created. For example using [Catch2][catch] or something else.
- ~~In parallel replace proprietary logging with a more modern logging system like [Plog][plog] or something similar. This is to concentrate more on the features of SourceMonitor instead of developing some logging solutions.~~ 20220208 - Old logging functions replaced with plog logging to file and console. Added additional logging for solving a bug. Needs to be customizable (loglevel) by a setting, will use registry entry like before.

## Download

The latest version can be downloaded [here][dpsm]. Keep in mind that this is a Windows only version, other OS are not supported at the moment.

[antlr]: https://www.antlr.org/
[catch]: https://github.com/catchorg/Catch2
[dpsm]: https://www.derpaul.net/SourceMonitor
[email]: mailto:SourceMonitor@derpaul.net?Subject=SourceMonitor
[inno]: https://jrsoftware.org/isinfo.php
[jim wanner]: https://campwoodsw.com/emcomp/about-us/
[plog]: https://github.com/SergiusTheBest/plog
[sourcemonitor]: https://www.campwoodsw.com/sourcemonitor.html
