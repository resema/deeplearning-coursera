## Week 2 Quiz - Autonomous driving (case study)

1. To help you practice strategies for machine learning, in this week we’ll present another scenario and ask how you would act. We think this “simulator” of working in a machine learning project will give a task of what leading a machine learning project could be like!

You are employed by a startup building self-driving cars. You are in charge of detecting road signs (stop sign, pedestrian crossing sign, construction ahead sign) and traffic signals (red and green lights) in images. The goal is to recognize which of these objects appear in each image. As an example, the above image contains a pedestrian crossing sign and red traffic lights


Your 100,000 labeled images are taken using the front-facing camera of your car. This is also the distribution of data you care most about doing well on. You think you might be able to get a much larger dataset off the internet, that could be helpful for training even if the distribution of internet data is not the same.

You are just getting started on this project. What is the first thing you do? Assume each of the steps below would take about an equal amount of time (a few days).

- [ ] Spend a few days getting the internet data, so that you understand better what data is available.
- [ ] Spend a few days training a basic model and see what mistakes it makes.
- [x] Spend a few days collecting more data using the front-facing camera of your car, to better understand how much data per unit time you can collect.
- [ ] Spend a few days checking what is human-level performance for these tasks so that you can get an accurate estimate of Bayes error.

2. Your goal is to detect road signs (stop sign, pedestrian crossing sign, construction ahead sign) and traffic signals (red and green lights) in images. The goal is to recognize which of these objects appear in each image. You plan to use a deep neural network with ReLU units in the hidden layers.

For the output layer, a softmax activation would be a good choice for the output layer because this is a multi-task learning problem. True/False?

- [x] True
- [ ] False

3. You are carrying out error analysis and counting up what errors the algorithm makes. Which of these datasets do you think you should manually go through and 

- [ ] 10,000 randomly chosen images
- [ ] 500 randomly chosen images
- [x] 500 images on which the algorithm made a mistake
- [ ] 10,000 images on which the algorithm made a mistake

4. After working on the data for several weeks, your team ends up with the following data:

- 100,000 labeled images taken using the front-facing camera of your car.
- 900,000 labeled images of roads downloaded from the internet.
- Each image’s labels precisely indicate the presence of any specific road signs and traffic signals or combinations of them. For example, ```y^{(i)} = \begin{bmatrix} 1 \\ 0 \\ 0 \\ 1 \\ 0 \end{bmatrix}``` means the image contains a stop sign and a red traffic light.
Because this is a multi-task learning problem, you need to have all your ```y^{(i)}``` vectors fully labeled. If one example is equal to ```\begin{bmatrix} 0 \\ ? \\ 1 \\ 1 \\ ? \end{bmatrix}``` then the learning algorithm will not be able to use that example. True/False?

- [ ] True
- [x] False

5. 

