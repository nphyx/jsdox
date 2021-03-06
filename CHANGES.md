ESDox Changes
=============

0.3.0
-----
* vast improvements to index file
  * now pulls author, license, description, and version info from package.json
  * indexes now show a summary of all top-level modules, classes, and functions and links
* new metadata for use by templates and other analysis improvements
  * functions with at least one default param get hasDefaultParams meta
  * files get hasMultipleModules if more than one module
  * example blocks are intelligently wrapped as needed
  * functions, modules, and classes can now have linebreaks in description
* template modularization improvements
  * links have their own partial for global use
  * summary partials for modules, functions, and classes
* file template updates
  * doesn't display header/navigation for modules if there's only one module in the file
  * @requires now shows in a bullet list instead of a single line
* function template updates
  * now shows "undefined" return value for functions without explicit return definition
* self-documentation updates for github wiki
  * internal methods tagged @private
  * regenerated with new templates


0.2.1
-----
* templateDir option fixes
  * now uses default templates for any template files that aren't supplied (you no longer have to supply a full set)
  * unbroke support for the option (oops...)
* markdown generation now loads templates asynchronously and caches them
  * should be a significant performance gain for projects with many files

0.2.0
-----
* support for custom index file name
  * --index-name \<name\> or --in \<name\> via CLI
  * opts.indexName via esdox module
* esdox generates docs for itself
  * found in docs/ folder
  * published to (https://github.com/nphyx/esdox/wiki)

0.1.0
-----
* template cleanups
  * function params now displayed in table
  * improved navigability of file-level docs
  * layout cleanup for functions and classes
  * file-level doc now includes original filename
  * @files/@emits tags now have nicer generated docs
* badges for readme
  * travis-ci
  * coveralls
  * npm version

0.0.1
-----

* hard fork from [jsdox](https://github.com/sutoiku/jsdox)
* migrated optimist to yarg
* incorporated istanbul/nyc for coverage testing
* (almost) complete unit testing
  * migrate to BDD style via should
  * stubs and mocks via sinon
* separate integration tests
* tests don't overwrite `sample_output` anymore
  * integration tests now create temporary output at `test/test_output`
  * they clean up afterward
* major refactor of core functions and CLI interface
  * replaced synchronous fs calls with async versions
  * esdox.js functions purely as a nodejs module
  * bin/esdox handles all CLI functionality
  * esdox.js no longer generates console output
  * some functions broken out and exported for easier unit testing

JSDox History
=============

0.5.0
------

* updated dependencies to latest releases
* migrated jscs and jshint to eslint
* added preliminary tests for analyzer (these are probably passing incorrect behavior, but they serve as a baseline)

0.4.10
------

* don't crash because argv is missing with debug on (psq)
* analyzer: include constructor params in class information (psq)
* add support for nested params (anselmstordeur)

0.4.9
------

* fix the error that occurs when a class has no methods (gaborsar)

0.4.8
------

* fix for subdirectories with an empty parent (gaborsar)

0.4.7
------

* Process descriptions for @link tags (nicksay)

0.4.6
------

* Add options to sort the index differently (nicksay)
* Add support for @namespace and @interface tags (nicksay)

0.4.5
------

* Require the latest version of JSDoc3 Parser (nicksay)

0.4.4
------

* fix undefined "argv" when using in programatic context (boneskull)

0.4.3
------

* Index generation for your generated documentation with -i (vdeturckheim)
* Recursive generation of documentation with -r (ie: documentation for subdirectories is generated too) (vdeturckheim)
* Respectful recursive generation with --rr (ie: the documentation for dir1/dir2/file.js will be in output\_dir/dir1/dir/file.md) (vdeturckheim)
* Use JSCS to check code formatting (mrjoelkemp, psq)
* normalizing headers to pound format (boneskull)
* use alternate horizontal rules so you don't get them confused with headers (boneskull)
* adding types to members (boneskull)
* types display monospace (boneskull)
* classes prefixed with "Class:" (boneskull)
* `@example` tag support for `@module` and `@function` (boneskull)
* separate `@author` from `@license` (boneskull)



0.4.2
------

* move `analyze` and `generatedMD` in their own module (mrjoelkemp)
* more tests (mrjoelkemp)
* `-A` option was ignored and became the default; fixed so it is no longer the default (boneskull)
* fixed issue wherein description of `@return` would become `@description` of function (duplicated) if not set for `@return` (boneskull)
* removed redundant `jshint-config.json` (boneskull)
* fixed `.jshintrc` (boneskull)
* fixed inability to find configuration file (boneskull)
* added `.editorconfig` so my editor doesn't blast trailing spaces in `.mustache` files (boneskull)
* `@example` tag support (boneskull)
* `@property` tag support (boneskull)
* `@private` tag support (boneskull)
* added types for class members (boneskull)
* correctly test for `@private` (mlms13)

0.4.1
------

* fix typo in `printHelp()` (psq)

0.4.0
------

* Add missing `templateDir` option in help output (psq)
* More CLI Tests (mrjoelkemp)
* Support for `@requires` and `@member` (lemori)
* New `--templateDir` option (lemori)
* More tests: CLI, Travis Integration, JSHint integration (mrjoelkemp)
* Travis badge (psq)
