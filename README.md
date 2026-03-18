# Open Graph Image generator

[![Publish package](https://github.com/febog/ogp-image-generator/actions/workflows/publish.yml/badge.svg)](https://github.com/febog/ogp-image-generator/actions/workflows/publish.yml)
[![NPM Version](https://img.shields.io/npm/v/%40febog%2Fogp-image-generator)](https://www.npmjs.com/package/@febog/ogp-image-generator)
[![NPM License](https://img.shields.io/npm/l/%40febog%2Fogp-image-generator)](https://www.npmjs.com/package/@febog/ogp-image-generator)

Open Graph Protocol image generator for my personal blog.

This script generates an open graph PNG image file for my personal blog for the given `title` and `date`.

## Installation 

```
npm install
```

## Usage

Set the required options `title`, `date` and `filename`. You can change the site name with the optional argument `site`.

Run:

```
npm start -- -t 'Hello world!' -d 'March 12th, 2026' -f 'my-image'
```

## Options

```
Options:
  -t, --title     Blog post title                            [string] [required]
  -d, --date      Date of the blog post i.e. March 2nd, 2026 [string] [required]
  -f, --filename  File name for the PNG i.e. my-image        [string] [required]
  -s, --site      Site name                          [string] [default: "febog"]
      --version   Show version number                                  [boolean]
      --help      Show help                                            [boolean]
```

## Output

The generated PNG image will be located under `images/`.

## Sample image

The script will generate an image as follows:

![Example of a generated open graph image showing the site name, blog post title and date in white letters on a blue background. The text says febog; Hello world!; March 16th, 2026.](assets/sample-output.png)
