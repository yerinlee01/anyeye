# ANyEye
![anyeye io - small](https://github.com/yerinlee01/anyeye/assets/97585388/d891d84f-f835-42e1-982d-ec9ed611faa1)

## Getting started
**Python==3.7**
1. Git clone or download this repository.

2. Install requirements on your virtual environment with

        pip install -r requirements.txt

3. Prepare the input data based on the following instructions:

   For image files:
   * Place all the image files in a single folder.
   * Ensure that the images are in either PNG (.png) or JPEG (.jpg) format.
   * Make sure the images are properly sorted in sequential order, representing frames of a video if applicable.
        
   For video files:
   * Prepare the video data in either AVI (.avi) or MP4 (.mp4) format.
   * Store the video file separately.

4. Edit config.ini.

        [config]
        input_dir = <directory of your folder, image, or video>
        filetype = <specify data type 'image' or 'video'>
        num_eyes = <count eyes of your input>
        left_eye_index = <insert index of left (inverted) eye if exists>
        video_out = <1 if you want video result 0 if you don't>
        model = <unet, unet++l2, unet++l3, or unet++l4>
        slippage_removal = <1 if you want slippage removed result 0 if you don't>

6. Execute ANyEye with

        python anyeye.py

7. Results will be created in `./results`.
