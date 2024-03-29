### dont rat me out[*]


![alt_text](images/image2.png "image_tooltip")


We need to find what this hamster is hiding. Image:


![alt_text](images/image5.jpg "image_tooltip")


Very cute hamster. Let’s use binwalk to check for hidden files. 


![alt_text](images/image17.png "image_tooltip")


Nope, no hidden files. That doesn’t mean that the file is clean. Let’s use [Exiftool](https://exiftool.org/) to check the photo for anything suspicious. 


![alt_text](images/image16.png "image_tooltip")


The comment and description “i am syrian” seem suspicious. We also know that the encoding process is [Huffman coding](https://en.wikipedia.org/wiki/Huffman_coding), which can be used to hide information. Let’s use [steghide](https://steghide.sourceforge.net/) to get the flag!


![alt_text](images/image8.png "image_tooltip")


Nice, we found the flag! Flag: WH2024{i_am_n0t_a_r4t}