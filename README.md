# vscode-issue-sample
A sample with the files necessary to reproduce a bug within Visual Studio Code;

Issue link: https://github.com/Microsoft/vscode/issues/5125

Did some tests today and found out the following:

1. Task runner is fine
2. When changing the ref URL in the .js, VS Code can't run "Launch" with the .ts file
3. Same happens when editting the name field in Source map file.

So, presumably the error is not at finding generated files nor source code. It may be at reading the source map, or placing breakpoints, but I sincerely don't know how I could test something like that. 
