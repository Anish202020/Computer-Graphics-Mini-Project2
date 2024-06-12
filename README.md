Topic-

Recognition of Face Emotion in Real-Time

Requirements-


Programming Language Used: -

Python

Packages:

Open CV (Live Video),

FER (Emotion Detection) &

NumPy (Numeric calculation and Array)

Working-

Fer (Package to detect emotion and tell what is it)

In our daily life, we knowingly or unknowingly carry out different types of Facial Expressions. These movements convey the emotional state of humans. We can judge the mood and mental state of the next person by his Facial Expression.

In the early Twentieth century, Ekman and Friesen defined `six` basic emotions. This expression does not change with cultures, they are universal.

Six Facial Expressions are: -

Happiness,

Sadness,

Fear,

Anger,

Surprise,

Disgust

I’ll show how to build a Facial Expression Recognizer using the `FER` library from python.

Facial Expression Recognition Library is developed by Justin Shenk.

This Library requires OpenCV>=3.2 and Tensorflow>=1.7.0 dependencies installed in the system.

Faces are detected using OpenCV’s Haar Cascade classifier.

OpenCV (For Real Time Video from Camera)

OpenCV, short for Open-Source Computer Vision Library, is an open-source computer vision and machine learning software library.

Originally developed by Intel, it is now maintained by a community of developers under the OpenCV Foundation.

OpenCV is a huge open-source library for computer vision, machine learning, and image processing. OpenCV supports a wide variety of programming languages like Python, C++, Java, etc.

It can process images and videos to identify objects, faces, or even the handwriting of a human.

When it is integrated with various libraries, such as NumPy which is a highly optimized library for numerical operations, then the number of weapons increases in your Arsenal i.e. whatever operations one can do in NumPy can be combined with OpenCV.

NumPy (for array calculation and number arrangement etc.)

NumPy is a general-purpose array-processing package. It provides a high-performance multidimensional array object, and tools for working with these arrays. It is the fundamental package for scientific computing with Python.

Besides its obvious scientific uses, NumPy can also be used as an efficient multi-dimensional container of generic data.

Array in NumPy is a table of elements (usually numbers), all of the same type, indexed by a tuple of positive integers. In NumPy, number of dimensions of the array is called rank of the array. A tuple of integers giving the size of the array along each dimension is known as shape of the array.

An array class in NumPy is called as ND array. Elements in NumPy arrays are accessed by using square brackets and can be initialized by using nested Python Lists.

Creating a NumPy Array Arrays in NumPy can be created by multiple ways, with various number of Ranks, defining the size of the Array.

Arrays can also be created with the use of various data types such as lists, tuples, etc. The type of the resultant array is deduced from the type of the elements in the sequences.

Working of the Model

Explanation Initialization: FER (mtcnn=True) initializes the emotion detector with MTCNN for face detection. The webcam is initialized with cv2.VideoCapture(0).

Function draw_face_emotions: This function draws rectangles around detected faces and displays the dominant emotion with its confidence score.

Main Loop: The script captures frames from the webcam, flips them horizontally, and detects faces and emotions in each frame. It then calls draw_face_emotions to draw rectangles around the faces and display the emotions. The frame is displayed in a window named 'Face Emotion Recognition'.

The loop breaks if the 'q' key is pressed.

Clean Up: The webcam is released, and all OpenCV windows are closed when the loop exits.

This script will open a window displaying the webcam feed with rectangles drawn around detected faces and the dominant emotion displayed above each face.

Contribution-

Anish Kumar (1AY21CS028)
