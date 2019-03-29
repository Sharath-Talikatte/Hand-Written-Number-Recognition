# Hand-Written-Number-Recognition

This is a very simple implementation of an Artificial Neural Network. The aim was to create a Network that would train on the MINST dataset so that it could learn to classify hand written numbers. 

The weights of the network are changed based on Stochastic Gradient Descent Algorithm (SGD).
The input image is captured using the webcam on the laptop, then cropped and then finally converted to gray scale and inverted. The image has to be inverted because the MINST data has images that contain white numbers on a black background. So, make sure you write the numbers on white piece of paper with a black pen.

The image processing is the crucial step. I had initially thought that the black and white images that are captured by the webcam were sufficient but it turns out that I was wrong. You can try it out without the image processing to see what I am talking about.

As I have informed before, this is just a rudimentary project which does not save the network weights once the network is trained. So, when you feed a new image, the network trains again and only then the prediction is done. Thankfully, because of the SGD algorithm, it only takes about 5 mins to train the netwrok(may depend on your system specs also!!) I'm working on a patch that enables you to store the network weights in a CSV file and retrieve the weights when required. I'll be updating that soon.
