# SimilarImagesFinder
A simple program to find similar images based on hashes. It compares all images by subtracting their hashes, and checking if the difference between these is less than a threshold.
It uses multiprocessing to speed up the job.

<b>How to use</b>

1) Navigate to the program folder
2) Install the requirements
```
pip install -r requirements.txt
```
3) Execute the program
```
python sif.py "path/of/the/images"
```

<b>Command line arguments</b>
* -processes [int]<br>
Specify the number of processes that multiprocessing should use. Default is 1 (single process).<br>
<i>Exaple:</i>
```
python sif.py -processes 4 "C:\Users\Snakkos\Photos"
```
* -threshold [int]<br>
Specify the threshold used when comparing images hashes. Default is 4<br>
<i>Example.</i>
```
python sif.py -threshold 4 "C:\Users\Snakkos\Photos"
```
* -subdirs
Use this command to extends the search of images to all subdirectories.<br>
<i>Example:</i>
```
python sif.py -subdirs "C:\Users\Snakkos\Photos"
```
