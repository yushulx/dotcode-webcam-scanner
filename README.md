# DotCode Webcam Scanner
The sample demonstrates how to implement a DotCode webcam scanner in C++ on Windows 10.

## Usage

Get a valid [Dynamsoft barcode license](https://www.dynamsoft.com/CustomerPortal/Portal/Triallicense.aspx) and update the code:

```cpp
iRet = reader.InitLicense("LICENSE-KEY");
```

Set barcode types:

```cpp
// Decode all supported barcode types.
runtimeSettings.barcodeFormatIds = BF_ALL;
runtimeSettings.barcodeFormatIds_2 = BF2_POSTALCODE | BF2_DOTCODE;
```

Build and run the app:

```
mkdir build
cd build
cmake -G"Visual Studio 15 2017 Win64" ..
cmake --build .
.\debug\BarcodeReader.exe
```

![DotCode cpp](http://www.codepool.biz/wp-content/uploads/2020/05/dotcode-cplusplus.png)



