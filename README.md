# Image Resize Function

The easiest way to resize images stored in Blob Storage (on Azure); uses [ImageSharp](https://github.com/SixLabors/ImageSharp)

## Quick Deploy to Azure

[![Deploy to Azure](http://azuredeploy.net/deploybutton.svg)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fhimanago%2Ffl-image-resize%2Fmaster%2Fazuredeploy.json)

## Configuration

Create container called 'images'; this is where images need to be uploaded into. Container 'thumbnails' will be generated, and files will be output there.

## Application settings

Here are the app settings that the function app depends on:

- **ImageRepository** - The storage account which houses the images to be processed; and where the resized images are stored.
- **ImageResize-Width** - The width the image is resized to.
- **ImageResize-Height** - The height the image is resized to.

## Running Locally

Visual Studio function app project is included. To run locally, create an `appsettings.json` file in the root of the function app. There is a sample included.
