Ad Inpainting API Guide
Introduction
This guide demonstrates how to use the ad inpainting API to create ads with images.

API Endpoint
The API endpoint for the ad inpainting service is: [API Endpoint]

Input Parameters
Prompt: Description of the desired image and context.
Image Number: Number of images to be generated.
Image Path: URL of the base image to be inpainted.
Product Size: Desired size of the product in the image.
Negative Prompt: Optional parameters for influencing the output.
Code Example
python
Copy code
import replicate
'''
input = {
    "prompt": "modern sofa+ in a contemporary living room, filled with stylish decor+;modern, contemporary, sofa, living room, stylish decor",
    "image_num": 4,
    "image_path": "https://replicate.delivery/pbxt/JAIk0rFAOUG00uetuiLOHPz42lBcf7QfX3xWi7TVaxMXXD4n/sofa1.png",
    "product_size": "0.5 * width",
    "negative_prompt": "illustration, 3d, sepia, painting, cartoons, sketch, (worst quality:2)"
}

output = replicate.run(
    "logerzhu/ad-inpaint:b1c17d148455c1fda435ababe9ab1e03bc0d917cc3cf4251916f22c45c83c7df",
    input=input
)
print(output)
'''
Output
The API generates inpainted images based on the provided prompts and input images.

GitHub Repository
Find the code and resources related to the ad inpainting project in the GitHub repository: [Repository Link]

Usage Guide
Clone the repository.
Install the required dependencies.
Use the provided code example to call the API with your desired parameters.
Explore the generated inpainted images.
Sample Images
Included are sample images demonstrating the before and after results of inpainting, along with the corresponding prompts used.

Conclusion
Utilize the ad inpainting API to effortlessly create compelling ads with visually appealing images. Explore further or contribute to the project as needed.

This guide provides comprehensive instructions for integrating the ad inpainting functionality into your application or project.
