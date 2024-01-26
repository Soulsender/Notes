## General
- exiftool shows image is ~652kb
- strings shows `base_images/2_c.jpgUT` string - hidden dir?
- image looks relatively normal
- file says it's really a .png and not a .jpg

## Hidden directories
- hexeditor says it is a zip file? *(see forensic magic numbers notes)*
	- ![[Pasted image 20221013114357.png]]
	- `binwalk -e` gets another zip file called `4286C.zip` and a directory called `base_images`
		- `base_images` has one image `2_c.jpg`
			- file shows this is also a png
			- strings shows
				- `base_images/4_c.jpgUT`
				- `base_images/3_c.jpgUT`
			- `binwalk -e` repeated process, similar output to before
- after repeating the process about 5 times, flag is in a text file
- flag is `picoCTF{bf6acf878dcbd752f4721e41b1b1b66b}`

![[dolls.jpg]]