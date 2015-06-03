# Requirements #
To build fully-functionaly libraries and demos, you need have:
  * GTK+ 2.x or higher.
  * libpng, zlib, libjpeg and libtiff with development files.
  * libavcodec from ffmpeg 0.4.9-pre1 or later + headers.
Earlier version do not work with OpenCV because of different API. **libavcodec** is **LGPL** software, so to use it with **non-GPL** software (such as OpenCV) you need to build and use a shared library **libavcodec.so.**

Get **ffmpeg** from http://ffmpeg.sourceforge.net

Build **ffmpeg** on your system
```
./configure --enable-shared
make
make install
```
You will get:

**/usr/local/lib/libavcodec.so.**

**/usr/local/lib/libavformat.so.**

**/usr/local/include/ffmpeg/_.h_**

in your _/usr/_ directory.


# Obtain the OpenCV library #

Download the library from http://sourceforge.net/projects/opencvlibrary/.

Since OpenCV is 2.0 now, please download _OpenCV-2.0.0.tar.bz2_, please do not download the windows version.

# Building OpenCV from sources #
Uncompress the packaged file
```
tar -xjf OpenCV-2.0.0.tar.bz2
```
Make a temporay build directory
```
mkdir opencv.build
```
Enter into the directory
```
cd opencv.build
```
Configure the building spec
```
../OpenCV-2.0.0/configure [<extra_options>]
```
Make
```
make -j 2
```
Install to _/usr/_
```
sudo make install
```
Register the library
```
sudo ldconfig
```







# Details #



Add your content here.  Format your content with:
  * Text in **bold** or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages






# Introduction #

Add your content here.


# Details #

Add your content here.  Format your content with:
  * Text in **bold** or _italic_
  * Headings, paragraphs, and lists
  * Automatic links to other wiki pages