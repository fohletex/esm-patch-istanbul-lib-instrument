# esm-patch-istanbul-lib-instrument

Patches issue https://github.com/istanbuljs/istanbuljs/issues/614: Having an ESM+TS-project and trying to fetch the code coverage via jest.

```
yarn add --dev patch-package
mkdir patches && cd patches
curl -LO https://raw.githubusercontent.com/fohletex/esm-patch-istanbul-lib-instrument/main/istanbul-lib-instrument+5.2.0.patch
patch-package
```

And don't forget to add the patch-package command in your `postinstall`-routine, as shown here:
https://www.npmjs.com/package/patch-package (Set-Up)
