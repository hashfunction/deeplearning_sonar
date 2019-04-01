# Deeplearning Sonar

Use deep learning techniques to convert any phone or speaker/mic combo in to a powerful Sonar. This is just an investigation in to the feasability. 

Note that there are classical techniques such as cross correlation which can also be used and were not evaluated as part of this project. 

## Summary

The data collection and cleanup took most of the time. I collected the data in a 'noisy' environment so as to not make the task too easy. Understanding the data and cleaning up/normalizing the audio files was a big part of the project. It turned out that the model for doing the actual mapping from audio to distance was a very shallow, simple one. 

The overall accuracy I was able to attain was just over 50% in both the test and validation set. This looks promising considering for this project, the dataset consisted of echo's from 7 different distances so one would expect an accuracy of less than 15% by chance. 

## Assets

[Jupyter Notebook Output](Audio_Echo_detection.html)
[Jupyter Notebook](Audio_Echo_detection.ipynb)
[Sample Data](data/)
