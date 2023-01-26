In order to have a common style code for all your projects, in Visual Studio Code you can use 2 extensions: ESLint and Prettier with their own configuration files :
•	.prettierrc
  with .prettierignore
•	.eslintrc.json
 This extensions require the following NPM packages to be installed: prettier, eslint.
 Select the default formatting extension as follows: Right-click in editor > "Format Document With" > "Configure Default Formatter" > "Prettier - Code Formatter".
 The step must be done for all file types (HTML, SCSS, TS, JSON) because there is a different default formatter for each extension. It must be Prettier everywhere.
 From now on ESLint should highlight code errors with yellow or red, and when saving a file Prettier should auto-format the code.
 In order to format all files between a project you must install globally Prettier:
npm i prettier -g
 And then run the command:
prettier --config .prettierrc --write 
