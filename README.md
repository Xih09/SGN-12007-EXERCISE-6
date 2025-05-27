Download link : https://programming.engineering/product/sgn-12007-exercise-6/

SGN-12007-EXERCISE 6
The tasks should be completed and presented to TA during the lab session. Do not forget to upload your solutions to Moodle! Questions about exercises should be addressed to the TA personally, through Moodle messages or via email, which can be found on the Moodle page of the course.

    Signal Creation

Create the following 128 x 128 gray-scale images:

    Constant value 0.5 for whole image.

    20×20 white square in the middle.

    Ramp from 0 to 1 in horizontal axis, constant in vertical axis.

    Delta function at the center of the image.

    Cosine signal having four periods in both directions; (help meshgrid).

All the images should be created using the full range of double precision from 0 to 1, and without using any for or while loops.

    DFT

    Perform the 2D Fourier transform on all the images in task 1. Take a look at Ex6_DFT.pdf for instruction of DFT in MATLAB. (help fftshift, fft2, log)

    Explain what information you get from Fourier transform of an image.

    Consider DFT images from task 1. Where is the energy concentrated and why?

    Filtering in the Frequency Domain

Butterworth filters can be defined as follows:

1

(a) Butterworth low-pass filter: ( , ) = 2

1+( ( , ))

0

1

(b) Butterworth high-pass filter: ( , ) = 1 − 2

1+( ( , ))

0

where 0 is the so-called cut-off frequency distance and ( , ) = √( − /2)2 + ( − /2)2 where × is the size of the image.

Use the given Butterworth low-pass filter (BWLPfilter.m), set the values 0 = 20, = 2 and filter the image cameraman.tif with both (a) and (b) filters. Show images of the filters and the final filtered images.
