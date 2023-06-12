# ANyEye

Python==3.7

1. git clone or download this repository

2. Install requirements on your virtual environment with

        pip install -r requirements.txt

3. Edit config.ini

        [config]
        input_dir = [directory of your image or video]
        filetype = [image or video]
        num_eyes = [count eyes of your input]
        left_eye_index = [insert index of left (inverted) eye if exists]
        video_out = [1 if you want tracked output 0 if you don't]
        model = [unet, unet++l2, unet++l3, or unet++l4]

4. Execute code with

        python anyeye.py

