# Go-Concurrency

Go-Concurrency contains practical use-cases for concurrency in Go.

These use-cases displays Go's concurrency constructs such as:  

- Go routines
- Channels
- Making downstream Go routines pre-emptible
- Multplexing inbound channels with ```Select```
- Pipeline concurrency pattern

***

## Image-Processing

This includes both sequential and concurrent program versions for purpose of comparison.

Image-Processing (```pipeline.go```) employs the pipeline concurrency pattern to convert source images to thumbnail images. This is a three-stage pipeline that invovles:

- Fetching the images from a directory, validating that they are truly images
- Processing the images, converting them to thumbnails
- Saving the thumbnail images to a destination directory

***

## Web-Crawler

Web-Crawler crawls the web for nested urls from a provided url given a provided level of depth. It includes both sequential and concurrent program versions.
