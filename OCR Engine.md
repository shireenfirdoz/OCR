# OCR Engine

OCR Engine applies artificial intelligence to extract informative data like bill no, bill date, type of bill and total amount from scanned bill uploaded by associate and filled in the form to reduce manual intervention..

## Ideal scenario for OCR Engine to work

- Standard template one image per pdf page
- If orientation of image is less than 30-degree acute angle, 90 degree ,180 degree ,270 degree then Engine can correct the orientation.
- Image is of good quality then accuracy percentage will be higher.
- Noise in scanned images is removed from noise filters.
- Handwritten bills are not taken in scope.
- Works best on images which have a DPI of at least 300 dpi


## Tech

OCR uses a number of open source projects to work properly:

- [Tesseract ] - extracting text from image
- [Xpdf] -   converting pdf to images
- [Java] - coding language
- [Linux Environment ] - to install and execute OCR Engine.
- [ImageMagick ] - cleaning the noise and maintaining the original structure of the image.
- [Custom Orientation Correction Algorithm] -  correcting the orientation of the image if image falls in category of 30-degree acute angle, 90 degree ,180 degree ,270 degree of orientation.
- [Custom Pattern Maching Algorithm ] - matching the keywords and extracting the informative information.


## Installation

OCR Engine requires [Tesseract](https://nodejs.org/) v10+ to run.

```sh
apt-get install tesseract-ocr
```

Install imagemagick with apt-get:

```sh
apt-get install imagemagick
```
Install x-pdf :
```sh
sudo apt-get update -y
```

```sh
sudo apt-get install -y xpdf
```

## Development


#### Building for source


## Problems

1)	Variation in template of bills, no standard template.
2)	Orientation issues in scanned images of bill.
3)	Noise in scanned images of bill like visibility and characters too small to identify.
4)	Handwritten bills were not able to read.
5)	Poor accuracy of transformed text.


## License

