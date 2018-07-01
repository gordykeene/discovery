# RPi OCR

## Purpose

Takes an image and converts it to text, identifies and extracts values of interest.

This is a sub-project for the meter-reader.

## Approaches

### Simple

This post [OCR - turning your photo into text]<https://www.raspberrypi.org/forums/viewtopic.php?t=45645> describes a bash solution.

Setup:

```bash
sudo apt-get install tesseract-ocr
```

Operation:

```bash
raspistill -o page.jpg
tesseract page.jpg pagetext
cat pagetext.txt
```

### NodeRED

NodeRED is looking really promising, possibly only needing a few libraries.

- [node-red-contrib-camerapi](https://flows.nodered.org/node/node-red-contrib-camerapi)
- [node-red-contrib-tesseract](https://flows.nodered.org/node/node-red-contrib-tesseract)

### .NET Core

A .NET Core solution appears possible, but the online information is fractured, and will require more researching and testing.

- <https://github.com/charlesw/tesseract/issues/298>
- <https://www.google.com/search?q=nuget+tesseract>
- <https://www.nuget.org/packages/Tesseract/>
  - May need to use a beta version.
- <https://github.com/Microsoft/Cognitive-Vision-DotNetCore>
  - Requires a 3rd party "Cognitive Services Vision API Key"

## RPi Camera Concerns

The current most likely hardware platform is a Raspberry Pi, however this raised concerns with heat. One solution is to only mount the camera externally using a longer cable.

This [Pi Camera Extension](https://www.tindie.com/products/freto/pi-camera-hdmi-cable-extension/) might help.

## Other Resources

[tesseract-ocr](https://github.com/tesseract-ocr/)
