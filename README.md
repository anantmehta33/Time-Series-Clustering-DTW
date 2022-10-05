There is an increasing need to comprehend signals from devices deployed in homes, shopping centres, factories, and workplaces in modern world where Internet of Things (IoT) is becoming more and more dominant. Any voice assistant, for instance, recognises, verifies, and understands human commands, whether they are given quickly or slowly. At various periods of the day, our speech tones typically vary. When we first get out of bed in the morning, our interactions are slower, heavier, and lazier than they are at other times of the day. These tools analyse the signals as time series and compute a similarity score by comparing the peaks, troughs, and slopes while accounting for the various delays and phases in the signals. Dynamic Time Warping is one of the most often used algorithms for achieving this (DTW). By ignoring shifts and speed, it is a fairly reliable way to compare two or more time series.

![image](https://user-images.githubusercontent.com/87894541/194021047-9b04921b-56a1-4ccb-a35e-7c05a03de694.png)

On the time axis, any two time series can be compared using euclidean distance or a comparable metric. Specifically, we'll compare the amplitude of the first time series at time T to the amplitude of the second time series at the same time. Even if the two time series share a similar shape but occur at different times, the score for comparison and similarity will be relatively low if this is the case.

![image](https://user-images.githubusercontent.com/87894541/194021402-4efd503e-e3b0-4a98-8d52-1e7102a1cc85.png)

DTW compares amplitude of first signal at time T with amplitude of second signal at time T+1 and T-1 or T+2 and T-2. This makes sure it does not give low similarity score for signals with similar shape and different phase.

![image](https://user-images.githubusercontent.com/87894541/194021448-a87601c9-992f-4f4c-9a8f-f27dc5914222.png)






