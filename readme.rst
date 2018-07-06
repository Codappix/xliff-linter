CLI Wrapper around Symfonies XLIFF-linter
=========================================

Abandoned, use xmllint instead, e.g.:

.. code-block:: bash

   apk --no-cache add libxml2-utils
   wget https://raw.githubusercontent.com/symfony/translation/v4.1.1/Resources/schemas/xliff-core-1.2-strict.xsd
   xmllint --schema xliff-core-1.2-strict.xsd --noout $(find localPackages -name '*.xlf')

Where `localPackages` is the folder containing your custom code.

Old description:

Symfony provides a translation package which delivers an XLIFF-Linter.

This packages provides a binary wrapper to lint xliff files using this linter.

Just require the package and call `./vendor/bin/xlifflinter <folder|file>`.

All further information are available in official documentation of symfonies
translation package: https://symfony.com/doc/current/translation/lint.html
