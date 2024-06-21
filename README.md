generate_key: Generates a random key of the same size as the image.
encrypt_image: Adds the key to the pixel values of the image and wraps around using modulo 256 to ensure values stay within the valid range.
decrypt_image: Subtracts the key from the encrypted image to get back the original image.
main: Executes the process of loading an image, encrypting it, and then decrypting it.
Notes:
This implementation assumes the image is in grayscale. For color images, the process needs to be repeated for each color channel.
For stronger encryption, more complex algorithms and keys should be used.
This basic tool demonstrates the concept of image encryption using pixel manipulation. For real-world applications, consider more secure methods and thorough testing.
