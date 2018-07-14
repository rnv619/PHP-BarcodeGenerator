# PHP-BarcodeGenerator

This script generates barcodes in four barcode formats including
Code 128, Code 39, Code 2of5, and Codabar, you have options for generating as “vertical” or “horizontal” display,
varying barcode heights and one of four barcode formats. It does require
the GD Library to be installed as a module in PHP.

## Installation

```
$ php composer.phar require rnv619/barcode "@dev"
```
or add

```
"rnv619/barcode": "@dev"
```


## How to Use
- Create Object of rnv619\barcode\GenerateBarcode class 
- Provice required inputs
- Done

### Example:
    require 'vendor/autoload.php';
    
    $gen = new \rnv619\barcode\GenerateBarcode("Code39", "20", "Rahul Ranva", true, "horizontal");
    $result = $gen->getCode();
    echo "<img alt='testing' src='".$result."'/>";


#### Supported Barcode Types

- code128
- code128b
- code128a
- code39
- code25
- codabar




