# Steganography-Android-App

What is Steganography?
Steganography is the process of hiding a secret message within a larger one in such a way that someone cannot know the presence or contents of the hidden message. Although related, Steganography is not to be confused with Encryption, which is the process of making a message unintelligible. Steganography attempts to hide the existence of communication. The main advantage of steganography algorithm is because of its simple security mechanism. Because the steganographic message is integrated invisibly and covered inside other harmless sources, it is very difficult to detect the message without knowing the existence and the appropriate encoding scheme.

How Encoding Algorithm works?
Firstly, the secret message that is extracted is compressed as the contents in the compressed string will significantly hard to detect and read, furthermore it reduces the size of string. 
Secondly, the compressed string is encrypted with the secret key.
Finally, encoding the encrypted message in the image. It uses LSB steganographic embedding to encode data into an image. Once the message is encoded the process stops.

What is LSB (Least Significant Bit) Embedding?
The LSB is the lowest significant bit in the byte value of the image pixel. The LSB based image steganography embeds the secret in the least significant bits of pixel values of the cover image (CVR). The concept of LSB Embedding is simple. It exploits the fact that the level of precision in many image formats is far greater than that perceivable by average human vision. Therefore, an altered image with slight variations in its colors will be indistinguishable from the original by a human being, just by looking at it. In conventional LSB technique, which requires eight bytes of pixels to store 1byte of secret data but in proposed LSB technique, just four bytes of pixels are sufficient to hold one message byte. Rest of the bits in the pixels remains the same.

How Decoding Algorithm works?
Firstly, decode the message from the encrypted image using LSB decoding. 
Secondly, decrypt the compressed message from the decoded message using the secret key. 
Finally, decompress the message to get the original compressed message.

![menu](https://user-images.githubusercontent.com/43198468/185630282-07c6f610-1cf1-4329-9715-faa486a24b6d.png)
![about](https://user-images.githubusercontent.com/43198468/185630331-84b1e0a5-d2dd-41e6-8296-592b7c92f1c7.png)
