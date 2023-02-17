# Information_Security_IA_ImageSteganography
### Created by Soham Dubewar (16010120069), Khushal Jhaveri (16010120074), Mihika Dakappagari (16010120076) and Shruti Mungale (16010120086), KJ Somaiya College of Engineering.
### It was made for Information Security IA1 in KJ Somaiya College of Engineering.

**Image Steganography:** Steganography is derived from two Greek words:'stegos,' which means 'to cover,' and 'grayfia,' which means 'writing,' thus translating to 'covered writing,' or 'hidden writing.' Steganography is a method of concealing sensitive information by embedding it in an audio, video, image, or text file. It is one of the techniques used to protect confidential or sensitive data from malicious attacks. Image Steganography, as the name implies, is the process of concealing data within an image file. The image chosen for this purpose is referred to as the cover image, and the image obtained after steganography is referred to as the stego image.

**Block Diagram**

![Pic]( https://github.com/Mihika135/Information_Security_IA_ImageSteganography/blob/main/images/image1.png?raw=true)

In memory, an image is represented as a N*M (for greyscale images) or N*M*3 (for colour images) matrix, with each entry representing the intensity value of a pixel. Image steganography embeds a message into an image by changing the values of some pixels chosen by an encryption algorithm.

**Conversion Table**

![Pic]( https://github.com/Mihika135/Information_Security_IA_ImageSteganography/blob/main/images/image2.png?raw=true)

The above table shows the conversion of character to decimal and binary numbers.

**Screenshots of Implementation**

![Screenshot (739)](https://user-images.githubusercontent.com/91322195/219712671-c6fc6941-971c-4c77-9c7d-d6bd2afdbbfc.png)

![Screenshot (740)](https://user-images.githubusercontent.com/91322195/219712717-ffac08e9-2083-4e33-b651-891f60ebd672.png)

![Screenshot (741)](https://user-images.githubusercontent.com/91322195/219712775-aa9fab50-7408-4412-a8b6-d87d68934289.png)

![Screenshot (742)](https://user-images.githubusercontent.com/91322195/219712815-936b180c-bad0-4c32-90b0-a719128db6c1.png)

![Screenshot (743)](https://user-images.githubusercontent.com/91322195/219712842-f486a0f3-ef01-4092-883a-9bc021f71318.png)

![image](https://user-images.githubusercontent.com/91322195/219716326-1f6d644f-23d1-41d0-a07c-eb675979d1ed.png)

**Explaination:**

- We have utilized the Least Significant Bit Algorithm for this method.
- In Least Significant Bit Algorithm a secret key is appended to the data to be hidden in the image and the new data is converted to binary.
- Images are made up of pixels which usually refer to the color of that particular pixel. 
- In an coloured image, these pixels are made up of three components (Red, Green, Blue) and each component is in the range 0-255.
- In this algorithm, we take the input text from user and using the secret key value we get the data message which we encode by converting it into binary format. 
- The encoded string is then encrypted in the image bit by bit.
- On doing the same for every pixel, a new image matrix is created.
- The new image has negligible changes because only the least significant bits are changed.
- To decode, the least significant bit BGR components of pixels are extracted and concatenated in a string.
- Groups of 8 bits are formed and converted to corresponding character values and once the key is found at the end of the string the decryption stops and the message is returned without the key.

### Is Steganography a Safe Way to Communicate?

When steganography is used alone, it provides security through obscurity, which may result in the secret message being revealed. Combining steganography and cryptography is the most effective way to hide a message from adversaries while still protecting it if it is discovered.

