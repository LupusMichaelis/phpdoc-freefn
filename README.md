To reproduce the issue:

```bash
$ wget -O phpdoc https://github.com/phpDocumentor/phpDocumentor2/releases/download/v2.9.0/phpDocumentor.phar
$ php phpdoc  -d ./src -t ./docs
Collecting files .. OK
Initializing parser .. OK
Parsing files
Parsing C:\Users\Micka▒l WOLFF\repositories\phpdoc-freefn\src\bogus.php
Parsing C:\Users\Micka▒l WOLFF\repositories\phpdoc-freefn\src\working.php
Storing cache in "C:\Users\Micka▒l WOLFF\repositories\phpdoc-freefn\docs" .. OK
Load cache                                                         ..    0.000s
Preparing template "clean"                                         ..    0.094s
Preparing 17 transformations                                       ..    0.000s
Build "elements" index                                             ..    0.000s
Replace textual FQCNs with object aliases                          ..    0.000s
Resolve @link and @see tags in descriptions                        ..    0.000s
Enriches inline example tags with their sources                    ..    0.000s
Build "packages" index                                             ..    0.000s
Build "namespaces" index and add namespaces to "elements"          ..    0.000s
Collect all markers embedded in tags                               ..    0.000s
Transform analyzed project into artifacts                          ..
Applying 17 transformations
  Initialize writer "phpDocumentor\Plugin\Core\Transformer\Writer\FileIo"
  Initialize writer "phpDocumentor\Plugin\Twig\Writer\Twig"
  Initialize writer "phpDocumentor\Plugin\Graphs\Writer\Graph"
  Execute transformation using writer "FileIo"
  Execute transformation using writer "FileIo"
  Execute transformation using writer "FileIo"
  Execute transformation using writer "FileIo"
  Execute transformation using writer "FileIo"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "twig"
  Execute transformation using writer "Graph"
   1.264s
Analyze results and write report to log                            ..
```
