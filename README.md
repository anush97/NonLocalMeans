# Non-Local Means Filter

This project implements the Non-Local Means filter for image denoising. The Non-Local Means filter is a non-linear method for image denoising, which replaces each pixel value with a weighted average of the values of neighboring pixels in the image. The weights are computed based on the similarity between the patch centered at the pixel being denoised and the patches centered at other pixels in the image.

## Usage

To use the Non-Local Means filter, you need to have Python and OpenCV installed on your system. You can install them using the following commands:

`sudo apt-get install python3`
`sudo apt-get install python3-pip`
`pip3 install opencv-python`


Once you have installed Python and OpenCV, you can run the script using the following command:

`python3 NonLocalMeans.py`


This will prompt you to enter the file path of the input image and the parameters for the filter. After entering the information, the script will apply the Non-Local Means filter to the image and save the result in a new file.

## Parameters

The Non-Local Means filter has several parameters that affect its performance. These parameters are:

- `h`: the filter strength
- `hForMean`: the filter strength used for the mean calculation
- `searchWindowRadius`: the radius of the search window
- `similarityWindowRadius`: the radius of the similarity window

You can adjust these parameters in the `NonLocalMeans.py` file to optimize the filter performance for your specific image.

## Examples

![Original Image](./images/lena.jpg)

![Denoised Image](./images/lena_denoised.png)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.
