
https://play.picoctf.org/practice/challenge/408?page=2

Description
How about some hide and seek? Download this file here. 

Hints

How can you view the information about the picture?

If something isn't in the expected form, maybe it deserves attention?

CLI

kappa@kappa-Aspire-Z5600:~/Desktop/canYouSee$ ls
can_you_see.md  ukn_reality.jpg  unknown.zip
kappa@kappa-Aspire-Z5600:~/Desktop/canYouSee$ exiftool ukn_reality.jpg
ExifTool Version Number         : 12.40
File Name                       : ukn_reality.jpg
Directory                       : .
File Size                       : 2.2 MiB
File Modification Date/Time     : 2024:03:11 17:05:55-07:00
File Access Date/Time           : 2024:12:27 13:41:05-08:00
File Inode Change Date/Time     : 2024:12:27 13:41:05-08:00
File Permissions                : -rw-r--r--
File Type                       : JPEG
File Type Extension             : jpg
MIME Type                       : image/jpeg
JFIF Version                    : 1.01
Resolution Unit                 : inches
X Resolution                    : 72
Y Resolution                    : 72
XMP Toolkit                     : Image::ExifTool 11.88
Attribution URL                 : cGljb0NURntNRTc0RDQ3QV9ISUREM05fNmE5ZjVhYzR9Cg==
Image Width                     : 4308
Image Height                    : 2875
Encoding Process                : Baseline DCT, Huffman coding
Bits Per Sample                 : 8
Color Components                : 3
Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
Image Size                      : 4308x2875
Megapixels                      : 12.4
kappa@kappa-Aspire-Z5600:~/Desktop/canYouSee$ base64 cGljb0NURntNRTc0RDQ3QV9ISUREM05fNmE5ZjVhYzR9Cg
base64: cGljb0NURntNRTc0RDQ3QV9ISUREM05fNmE5ZjVhYzR9Cg: No such file or directory
kappa@kappa-Aspire-Z5600:~/Desktop/canYouSee$ echo -n 'cGljb0NURntNRTc0RDQ3QV9ISUREM05fNmE5ZjVhYzR9Cg' | base64 --decode
picoCTF{ME74D47A_HIDD3N_6a9f5ac4}
base64: invalid input
kappa@kappa-Aspire-Z5600:~/Desktop/canYouSee$ 


cGljb0NURntNRTc0RDQ3QV9ISUREM05fNmE5ZjVhYzR9Cg


