## A Few Rules for dealing with repositories

- **Each project directory contains one or more `README.md` files in sub directories. These should be your guide to working with the projects & subdirectory content.**
- **As a standing rule of style & organization use lowercase-kabob-case as your directory naming convention**
- **NoCamelCase**
- **No Directories With Spaces**
- **If you add a project directory or update an existing directory please update this README.md and update or create any other appropriate README.md files**

## Directory & Filename Conventions

- Markdown (.md) files should be declared in all caps: `README.md`, `CHANGELOG.md`, `CONTRIBUTING.md`
	- Only the extension .md should be used, not .markdown
- License files declaring copyright can also be declared in all caps: `LICENSE` 
- Directory & Filenames should be declared in lowercase-kabob-case only unless an expection applies.
- Reasonable naming convention exceptions:
	- The SASS underscore: A partial is a Sass file named with a leading underscore. You might name it something like `_partial.scss`. The underscore lets Sass know that the file is only a partial file and that it should not be generated into a CSS file. Sass partials are used with the @use rule. [see ref ->](https://sass-lang.com/guide#topic-4)
	- Some React projects may decide to use a folder or file structure that mimics PascalCase component naming conventions [see more ->](https://stackoverflow.com/a/56196707)
	- in general: keep it kabob-case unless a project, framework or tooling call for something different

## Writing Markdown

### Links:
  - Markdown link convention can be used to point users to more information, references or community opinions
  - use `see ref ->` to point user to technical reference & documentation: [see ref ->](https://sass-lang.com/guide#topic-4)
  - use `see more ->` to point users to community answers or opinionated content (blogs, vlogs etc..): [see more ->](https://stackoverflow.com/a/56196707)

## Tabs & Spaces
  - A common tab structure should be set to indent using 1 tab, set as 2 spaces
  - set your code editor up so 1 tab = 2 space characters
  - set your code editor up so 1 line indent will indent content by 1 tab / 2 spaces

## Common Gitignore

Current `.gitignore`

```
# .gitignore [see ref ->](https://git-scm.com/docs/gitignore#_pattern_format)
# helpful .gitignore tests & breakdown [see more ->](https://www.hilman.io/blog/2015/09/what-you-need-to-know-about-gitignore/)

# ignore .DS_Store [see more ->](https://en.wikipedia.org/wiki/.DS_Store)
.DS_Store
# ignore node_modules directory created by NPM or YARN
/node_modules/
# ignore common dist directories
/_dist/
/dist/
# ignore commong temporary directories
/_tmp/
/tmp/
/temp/
# ignore Jet Brains intelliJ .idea/ directory & files
/.idea/
# ignore vscode editor directory if you don't want to be sharing settings across project users
/.vscode/
# optional - evaluate if the project should ignore yarn lock file
yarn.lock
# optional - evaluate if the project should ignore package json lock file
package-lock.json
# optional (personal preference here) - ignore scratch directory
/scratch/ 
# ignore .log files
*.log
# ignore hidden cache files
.cache
# ignore hidden eslintcache files
.eslintcache
```

If you are working with an editor (like Atom) that does not show content listed in `.gitignore` files, you can temporarily comment out lines of the `.gitignore` file or use a file manager / editor like Visual Studio Code.

**If you update the `.gitignore` file please update this README.md**

## Opensource & Public Developer Styleguides

  - Google:
    - https://google.github.io/styleguide/
    - https://google.github.io/styleguide/vimscriptguide.xml
    - https://google.github.io/styleguide/jsguide.html
    - > If you are going to be humorous, be like our friend [Uther](https://google.github.io/styleguide/jsguide.html#appendices-documentation-annotations)
    - https://google.github.io/styleguide/htmlcssguide.html
    - https://developers.google.com/style
      - found it via searching for documentation on common developer documentation practices for writing terminal commands & shell code syntax https://developers.google.com/style/code-syntax


  - Airbnb:
    - https://github.com/airbnb/javascript

  - Facebook:
    - ?