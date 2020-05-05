# Computer Vision
So the main question is how does our Brain work?
This is one of the major questions in Neuroscience and Machine Learning!!! yet to be answered

<img src="C:\Users\Abhishek\Desktop\My_Projects\Northeastern\CV.png" alt="My cool logo"/>

## Neural nets are suppose to mimic the way our brain works, but still i believe we are far being figuring out whether we can predict how our brain works!!

Coming back to #Computer Vision, 
as we have not figured out how our brain is able to depict every thing, and understand what is what, so i believe we are still not sure about the algorithms we are using for predicting images!!
Computer Vision is mainly pattern prediction- we train our algorithms with some test data ( images with labels), and the machine trys to figure out the pattern in those data which later can be used for prediction of a image without a label.
# Example:-
If you feed an image of Dog to the machine, maybe Millions of images of Dogs, 
the algorithm will try and figure out the different patterns of colors, different shapes in which it can be showed, distances, borders.
When finished the computer will be able to use its experience when fed other unlabeled images of dogs

Computers usually read image as its pattern of colors, which is usually a combination of 3 series - Red , Green , Blue (RGB)
So basically each pixel has 3 additional value to store along with the position of pixel, that is its combination of RGB (Like 26 * 190 * 255)
## Isnt that alot of information to store along within a picture!!
## Just imagine when we feed thousands, or maybe millions of data to a machine for analysis!!

# Evolution of Computer Vision 
Ealier the for the same prediction of an image as mentioned above ( the Dog example)
- a specific format of image was required
-the system required an imput of information like distance between eyes, lips, legs etc etc...thats alot of key points that the system required 
- mentioning all these key points on the picture that is fed to the system
phheww!!! alot right???
this involved alot of coding.
After all this hard coding the application would finally compare the measurements provided to the measurements of the image already stored.
The Error margin was still highhh!!!

## Then Came Machine Learning
It provded another approach of resolving this issue. With ML the developers no longer had to send every measurement of the image to the system.
ML used statistical learning, Logical regression, Decision trees, Support Vector Machine(SVM) to detect patterns andclassify images.
For instance:- years ago ML Engineers were able to predict breast cancer way better than human experts, although it took a lot of experts in various fields to develop it.

## Then coming to Deep Learning
This one provided a different approach of using Machine Learning. Deep learning relies on neural networks, a general-purpose function that can solve any problem representable through examples. When you provide a neural network with many labeled examples of a specific kind of data, it’ll be able to extract common patterns between those examples and transform it into a mathematical equation that will help classify future pieces of information.

## Example 
Creating a facial recognition application with deep learning only requires you to develop or choose a preconstructed algorithm and train it with examples of the faces of the people it must detect. Given enough examples (lots of examples), the neural network will be able to detect faces without further instructions on features or measurements.
## Deep learning is a very effective method to do computer vision. 

## Compared to previous types of machine learning, deep learning is both easier and faster to develop and deploy.
Most of current computer vision applications such as cancer detection, self-driving cars and facial recognition make use of deep learning. Deep learning and deep neural networks have moved from the conceptual realm into practical applications thanks to availability and advances in hardware and cloud computing resources.

# Now coming to the Computer Vision
Computer vision is one of the areas in Machine Learning where core concepts are already being integrated into major products that we use every day. 

## CV In Self-Driving Cars
But it’s not just tech companies that are leverage Machine Learning for image applications.
Computer vision enables self-driving cars to make sense of their surroundings. Cameras capture video from different angles around the car and feed it to computer vision software, which then processes the images in real-time to find the extremities of roads, read traffic signs, detect other cars, objects and pedestrians. The self-driving car can then steer its way on streets and highways, avoid hitting obstacles, and (hopefully) safely drive its passengers to their destination.
## CV In Facial Recognition
Computer vision also plays an important role in facial recognition applications, the technology that enables computers to match images of people’s faces to their identities. Computer vision algorithms detect facial features in images and compare them with databases of face profiles. Consumer devices use facial recognition to authenticate the identities of their owners. Social media apps use facial recognition to detect and tag users. Law enforcement agencies also rely on facial recognition technology to identify criminals in video feeds.
## CV In Augmented Reality & Mixed Reality
Computer vision also plays an important role in augmented and mixed reality, the technology that enables computing devices such as smartphones, tablets and smart glasses to overlay and embed virtual objects on real world imagery. Using computer vision, AR gear detect objects in real world in order to determine the locations on a device’s display to place a virtual object. For instance, computer vision algorithms can help AR applications detect planes such as tabletops, walls and floors, a very important part of establishing depth and dimensions and placing virtual objects in physical world.
## CV In Healthcare
Computer vision has also been an important part of advances in health-tech. Computer vision algorithms can help automate tasks such as detecting cancerous moles in skin images or finding symptoms in x-ray and MRI


## Challenges of Computer Vision
Helping computers to see turns out to be very hard.
Inventing a machine that sees like we do is a deceptively difficult task, not just because it’s hard to make computers do it, but because we’re not entirely sure how human vison works in the first place.

# Many popular computer vision applications involve trying to recognize things in photographs; for example:
Object Classification: What broad category of object is in this photograph?
Object Identification: Which type of a given object is in this photograph?
Object Verification: Is the object in the photograph?
Object Detection: Where are the objects in the photograph?
Object Landmark Detection: What are the key points for the object in the photograph?
Object Segmentation: What pixels belong to the object in the image?
Object Recognition: What objects are in this photograph and where are they?

# Outside of just recognition, other methods of analysis include:
Video motion analysis uses computer vision to estimate the velocity of objects in a video, or the camera itself.
In image segmentation, algorithms partition images into multiple sets of views.
Scene reconstruction creates a 3D model of a scene inputted through images or video.
In image restoration, noise such as blurring is removed from photos using Machine Learning based filters.

# Conclusion
Despite the recent progress, which has been impressive, we’re still not even close to solving computer vision.








Source :- TowardsDataScience (https://towardsdatascience.com/everything-you-ever-wanted-to-know-about-computer-vision-heres-a-look-why-it-s-so-awesome-e8a58dfb641e)