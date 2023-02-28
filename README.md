# SafetyPro

Recognize stop signs and other safety-related objects from photos using Microsoft Azure Cognitive Services! Upload an image and find out whether there are safety concerns to be aware of.

* image detection
* computer vision

Sample images are provided in the public/img folder.

I kept the layout intentionally simple because it is a tech demo.

---
## Tech Used

* Machine learning API: Microsoft Azure Cognitive Services
* * Computer Vision
* JavaScript & EJS
* HTML / CSS

## Take-aways / Optimizations
* I learned that Azure's off-the-shelf computer vision counts every road sign as "stop sign".
* This might change or improve over time, and since this app gets classification by API, it will be automatically reflected as changes are made.

Other possible updates may include:
* Use Cognitive Services for OCR, optical character recognition, to read signage
* Recall images from a library
* Open text input to check for custom keywords
* Overlay rectangles over objects, using CSS
* Layout improvements

## Install

`npm install`

## Things to add

- Create a config folder with a `.env` file and add the following as `key = value`
  - PORT = 2121 (can be any port example: 3000)
  - CLOUD_NAME = `your cloudinary cloud name`
  - CLOUD_API_KEY = `your cloudinary api key`
  - CLOUD_API_SECRET = `your cloudinary api secret`
  - MS_COMPUTER_VISION_SUBSCRIPTION_KEY = `your Microsoft Subscription Key`
  - MS_COMPUTER_VISION_ENDPOINT = `your Microsoft Computer Vision Endpoint`
  - MS_FACE_ENDPOINT = `your Microsoft Face Endpoint`
  - MS_FACE_SUB_KEY = `your Microsoft Face Key`

## Run

* `npm start`
* Go to http://localhost:2122
* If you need example images to try it out, navigate to public/img/

---
