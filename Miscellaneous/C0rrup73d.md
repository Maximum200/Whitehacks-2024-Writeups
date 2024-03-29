### C0rrup73d[*]


![alt_text](images/image11.png "image_tooltip")


Hmm, let’s try opening the file first. 


![alt_text](images/image3.png "image_tooltip")


We can’t open the file. It must be because the file is corrupted. Let’s open it in [HexEd.it](https://hexed.it/) to check if the file header is damaged.


![alt_text](images/image9.png "image_tooltip")


Yep, we were right. The file header is indeed damaged. 

For reference, a proper file header for a png file is shown below.


![alt_text](images/image1.png "image_tooltip")


Essentially, the first 8 hexadecimal slots of a png file are always 89  50  4e  47  0d  0a  1a  0a. Without this, the file will not work as intended. Let’s correct this and fix the image. 

Fixed image:


![alt_text](images/image14.png "image_tooltip")


Are you kidding me another cipher???

Let’s just continue on. After doing some googling, we find that this is a [dancing men cipher](https://www.arthur-conan-doyle.com/index.php/Dancing_Men_Alphabet). We’ll need to decode this again. We’re using [https://www.dcode.fr/dancing-men-cipher](https://www.dcode.fr/dancing-men-cipher) this time, as it gives us images of the dancing men themselves to click to decode, a huge help. Let’s decode the cipher.


![alt_text](images/image4.png "image_tooltip")


Nice, we found the flag! 

Flag: WH2024{WHITEHACKSISSOFUN}