# My Solve
Ran Exiftool on the image provided.
ExifTool Version Number         : 12.57
File Name                       : challenge.jpg
Directory                       : .
File Size                       : 371 kB
File Modification Date/Time     : 2025:10:02 02:43:04+05:30
File Access Date/Time           : 2025:10:02 02:43:04+05:30
File Inode Change Date/Time     : 2025:10:02 02:43:04+05:30
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
XMP Toolkit                     : Image::ExifTool 12.57
Author                          : kdj had a habit of hiding images within images
Image Width                     : 640
Image Height                    : 1017
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 640x1017
Megapixels                      : 0.651
KDJ hid images within images. Extract the hidden image from challenge.jpg using foremost or binwalk.
This gives us the embedded PNG which gives us the flag.
*Flag:* citadel{th1s_ch4ll3ng3_1s_f0r_th4t_0n3_ex1ft00l_4nd_b1nw4lk_enthus14st} `

