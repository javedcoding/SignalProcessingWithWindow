# SignalProcessingWithWindow
This is a python project of Computational Intelligence to find the peak of a signal autonomously from a data set read from xlsx formatted file.
![Screenshot 2022-12-04 160522](https://user-images.githubusercontent.com/59325753/205498488-8041a03f-519f-44b4-9fdd-583907c2e4a6.png)

To Start the program first we have to put the data file's path location the first box.
Then from that data file we have to select a single signal by the number of that signal (as in our file the signal is given in each row of the xlsx file it's the row number)
All the other fields are optional as they already have a predefined default value given.
Noise ignoring amplitude is the cutting amplitude from where the windowing will start and the average signal is calculated. Any point above this average signal is counted as a peak. 
Initial Threshold is the initial average signal's peak which will be changed as the signal proceeds. In the process we will get many of the peaks as its a smooth signal data set, among these peaks the highest value is counted as the highest peak.
Influence of the previous window is required to shape the emerging average signal. More the value, more the avg signal takes shape close to the original one.
Threshold to remove spike is required for the second catagory data set (DataSet2.xlsx file which could not be uploaded in github because of it's size) where the signals have spikes and we have to remove the spike using regression algorithm.
The Result pannel will give the detected outlier peaks range of the signal and the highest peak value with the predefined theshold amplitude and influence for that signal as a suggestion.
There are three curves showing the main signal with the highest first peak as the red dotted position, the x axis time points where outlier peaks are detected and the emerging average signal shape.
