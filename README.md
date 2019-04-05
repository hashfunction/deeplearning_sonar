# Deeplearning Sonar

Use deep learning techniques to convert any phone or speaker/mic combo in to a powerful Sonar. This is just an investigation in to the feasability. 

Note that there are classical techniques such as cross correlation which can also be used and were not evaluated as part of this project. 

## Summary

The data collection and cleanup took most of the time. I collected the data in a 'noisy' environment so as to not make the task too easy. Understanding the data and cleaning up/normalizing the audio files was a big part of the project. It turned out that the model for doing the actual mapping from audio to distance was a very shallow, simple one. 

The overall accuracy I was able to attain was just over 99% in both the test and validation set. This looks promising considering for this project, the dataset consisted of echo's from 7 different distances so one would expect an accuracy of less than 15% by chance. 

## Assets

* [Jupyter Notebook Output](http://htmlpreview.github.io/?https://github.com/hashfunction/deeplearning_sonar/blob/master/Audio_Echo_Detection.html)
* [Jupyter Notebook](Audio_Echo_Detection.ipynb)
* [Sample Data](data/)

### Further steps and investigations

From the analysis above, its clear that the data is not of very high quality and the S/N ratio is quite low. This is why its hard for us to visually distinguish some of the samples. Still we were able to achieve > 99% accuracy from our testing set.

Some next steps are outlined below. 

* Gather more data. This will give us a better gauge of the effectiveness of the model.
* Look at the failed cases in more detail and see if we can spot the issues there.
* Remove the original chirp from the data so we are feeding the network less noise.
* Experiment with some blurring/averaging techniques to see if that can bring out the signal better.
* Use a different mic. This was captured with a ps3 eye toy 4 microphone array with low fidelity. 
* Try different waveforms for the chirp to see if perhaps different frequencies yield better results.
* I am also curious about how general this trained model is to variations in ambient noise. 
