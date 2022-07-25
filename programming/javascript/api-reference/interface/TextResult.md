---
layout: default-layout
title: Dynamsoft Barcode Reader JavaScript API - Interface - TextResult
description: Use this interface syntax to set text results for barcodes in Dynamsoft Barcode Reader for JavaScript.
keywords: TextResult, BarcodeReader, api reference, javascript, js
needAutoGenerateSidebar: false
noTitleIndex: true
breadcrumbText: TextResult
permalink: /programming/javascript/api-reference/interface/TextResult.html
---


# TextResult

`interface` TextResult

* barcodeText: *string*

  > The barcode text.

* barcodeFormat: *number &#124; [EnumBarcodeFormat](../enum/EnumBarcodeFormat.md)*

  > The barcode format.

* barcodeFormatString: *string*

  > Barcode type in string.

* barcodeBytes: *number&#91;&#93;*

  > The barcode content in a byte array.

* localizationResult: *[LocalizationResult](LocalizationResult.md)*

  > The corresponding localization result.

```js
let reader = await Dynamsoft.DBR.BarcodeReader.createInstance();
let results = await reader.decode(imageSource);
for(let result of results){
  console.log(result.barcodeText);
}
```

Some advanced parameters are not listed. See [C++ TextResult](https://www.dynamsoft.com/barcode-reader/programming/c-cplusplus/struct/TextResult.html?src=cpp&&ver=latest) for more info.
