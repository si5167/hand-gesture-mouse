# hand-gesture-mouse

Abstract— We propose a new approach for controlling mouse movement using a real-time camera. Most of the existing approaches involve changing mouse parts such as adding more buttons or changing the position of the tracking ball. Instead, we propose to change the hardware design. Our method is to use a camera and computer vision technology, such as image segmentation and gesture recognition, to control mouse tasks (left click and right click, selection, scroll and drag). Hand gestures are acquired using Web camera based on colour detection. In our project, three colour tapes are used on fingers. The tapes will be used for clicking events of the mouse. Through Web camera the real time video is captured. Image processing is performed on each frame of that video to detect the colour and mouse tasks are performed.
Keywords: Hand gesture, colour detection, human computer interaction (HCI), HSV (hue, saturation, value) Colour Model, Web camera, RYB (red, yellow, blue).
1. INTRODUCTION
Human Computer Interaction today, mainly deals with natural interfaces. The Graphical User Interface (GUI) on Personal Computers (PCs) is developed, providing an efficient interface for a user to interact with the computer and access the various applications effortlessly.
Today, the technology used for interaction by mobile phone is mainly touch screen. But this technology is still not that cheap to be used in laptops and desktops. Our aim is to create a virtual mouse system having a user-friendly interface and an alternative to touch screen.
Human Computer Interaction is not just limited to keyboard and mouse interaction. Interaction between humans comes from different sensory modes like gesture, speech, facial and body expressions. Being able to interact with the system naturally is becoming even more important in many fields of Human Computer Interaction.
We use gestures to operate the cursor. Gestures are a major form of human communication. A primary goal of
gesture recognition is to create a system which can identify specific human gestures and use them to convey
information for controlling device a user can control a computer by making a specific gesture in front of a video camera which is linked to the computer.
Our project is based on human computer interaction. To make fewer human efforts to operate their computer and to use hand gestures to communicate with the computer.
• Our project emphasizes to command your computer using natural hands gesture
• No remote controls required
• No wearable devices required
• Only one thing required: YOUR HAND
Our aim is to create a virtual mouse system a user-friendly device and an alternative to touch screen. By applying vision technology and controlling the mouse by natural hand gestures, we can reduce the workspace required. We propose a novel approach that uses a video device to control the mouse system.
2. LITERATURE REVIEW
Many researchers in the human computer interaction and robotics fields have tried to control mouse movement
Siddhika Aher Bhairavi Brahme
Department of Computer Engineering Department of Computer Engineering
NHITM, Mumbai University NHITM, Mumbai University India India
siddhika.aher@gmail.com bkbrahme@gmail.com
Chhaya Upadhyay Megha Gupta Debajyoti Mukhopadhyay
Department of Computer Engineering Department of Computer Engineering Department of Computer Engineering
NHITM, Mumbai University NHITM, Mumbai University NHITM, Mumbai University
India India India
upadhyaychhaya433@gmail.com meghavgupta@outlook.com debajyoti.mukhopadhyay@gmail.com
An Experimentation to Simulate Mouse Movement Using Hand Gestures based on Human Computer Interaction
using video devices. However, all of them used different methods to make a clicking event.
In [1], the wearable unit will consist of buttons on fingertip for click, an accelerometer inside the glove for sensing the motion and getting the direction of motion. This would be connected to a microcontroller and also a transmitter to communicate wirelessly to the base unit. The accelerometer reads the tilt of each axis and outputs each as an analog voltage. Push buttons are used for enabling and disabling the mouse and for making left click and right click. RF module is used to provide wireless communication.
In [2], Zhi-hua Chen uses real-time hand gesture recognition using the finger segmentation method. The hand region is extracted from the background with the background subtraction method Then, the palm and fingers are segmented so as to detect and recognize the fingers. Finally, a rule classifier is applied to predict the labels of hand gestures. Basically, what the position of the fingers is based on that it will only show the pattern of fingers on the screen.
In [3], Chu-Feng Lien used only the finger-tips to control
the mouse cursor and click. His clicking method was based on image density, and required the user to hold the Mouse cursor on the desired spot for a short period of time. It starts from retrieving images from camera drivers. Upon a valid image, it firstly finds the location of the possible projected screen by Canny Edge detection. After finding the target screen, it then calculates the position mapping between camera resolution and device resolution. The projected screen detection is executed every 10 seconds in case the camera or the target screen is moved accidentally. After the basic environment setup process, the system reads images in a ring buffer and shows the differences between frames based on MHI.
In [4], Kamran Niyazi used a web camera to detect colour Fig.1 Proposed System Architecture
tapes for cursor movement. The clicking actions were performed by calculating the distance between two coloured tapes in the fingers. For left click on the very first step, the system records the distance (say D) between the yellow and red tapes in the index finger and the thumb respectively. Here, the index and thumb must be apart as much as possible so as to get maximum distance. This distance is regarded as the threshold distance for the event. Now, as the thumb moves towards the index finger, the distance between the fingertips or in other words, the distance between yellow and red tapes is decreased. In the second step, when the thumb is closer to the index finger the system records the reduced distance. When the distance between the tapes is reduced to D’ or less we consider the event as the left click event of the mouse cursor. The right click event of the cursor is simulated using the concept of waiting time. If the yellow tape on the index finger is waiting for 7 seconds(say) in front of the camera pointing at the same location, then the
event is recognized as the right click event of the mouse cursor. Here, the distance between the red and yellow tapes should be between D and D’ respectively. The double click event of the cursor is also simulated in the same way as the right click event considering the waiting time. The only difference is that the double click event of the mouse cursor.
In [5], A. Erdem uses a fingertip tracking to control the motion of the mouse. A click of the mouse button was implemented by defining a screen such that a click occurred when a user’s hand passed over the region.
3. PROBLEM DEFINITION
Hand gesture mouse is a recognition system based on Human Computer Interaction (HCI) and Image Processing which can control the cursor movement and
click events like left click, right click, drag, select, scroll similar to that of a mouse using hand gestures. The hand gesture will be acquired by a web camera and programmed using RYB colour detection technique. The
system should identify the colour cap and perform the corresponding mouse event. The camera is positioned such that it recognizes the moment of the finger tips and perform the operations of the mouse. Depending on the user’s preferences, the system shall perform adjustments according to user’s dominant hand. Based on the distance between the centers of the colour the mouse actions will perform.
4. PROPSED SYSTEM OVERVIEW
4.1 System Overview
One of the important challenges in Human Computer Interactions is to develop more intuitive and more natural interfaces. Computing environments presently are strongly tied to the availability of a high-resolution pointing device with a single, discrete two-dimensional cursor. While the utility of such devices in today’s interfaces cannot be denied, there are many users who find that the capability of the GUI is rather limited when they try to do some tasks by using gestures.
There are opportunities to apply other kinds of sensors and techniques to enrich the user experience of such users. For example, video cameras and computer vision techniques may be used to capture many details of human shape and movement. The shape of the hand may be analyzed over time to manipulate an onscreen object in a way analogous to the hand’s manipulation of paper on a desk. Such an approach may lead to a faster, more natural, and more fluid style of interaction for certain tasks.
Our project, Mouse Simulation Using Three Coloured Tapes is an attempt in ubiquitous computing. Here, we will be using three colour tapes on our fingers. One of the tapes will be used for controlling cursor movement while the relative distance between the two-coloured tapes will
be used for click events of the mouse. Thus, the system will provide a new experience for users in interacting with the computer.
4.2 Technical Overview:
The platform used for project implementation is Anaconda3. Anaconda3 is an open source distribution of Python language. Anaconda Navigator (virtual environment manager) helps in eliminating the need to learn to install each library independently also it gives high performance computing. The program uses Image Processing, it is a method to perform some operations on an image, in order to get an enhanced image of palm or to extract some useful data. It is a type of processing in which image or characteristics/features are extracted associated with that image to perform tasks the mouse. The program is implemented in Python. It uses image processing module OpenCV and implements the mouse actions using python specific library PyAutoGUI.
Packages installed for successful compilation of the program are Python interpreter to read and execute the code, OpenCV an open source computer vision for capturing real time video and for the analysis of features of the hand. NumPy for numerical operations and PyAutoGui is a library function that provides a method for controlling the mouse.
Video captured by the webcam is processed and only the three coloured tips are extracted. The distance between centers of particular colour are calculated using the method of moments and depending upon their relative positions mouse actions are performed.
4.2.1 Capturing the real time video
For the system to work we need a sensor to detect the hand movements of the user. The webcam of the computer is used as a sensor. The webcam captures the real time video at a fixed frame rate and resolution, which is determined by the hardware of the camera. The frame rate and resolution can be changed in the system if required.
4.2.2 Image Processing
1. We convert the video into HSV format.
2. Now the user gets to calibrate the colour ranges of individual finger. This is done by calling the calibratecolour() function.
3. Depending upon the calibration, only three fingertips are extracted from the video one by one using cv2.inrange() function.
4. To remove noise from the video feed we apply two step morphism erosion and dilation. The noise filtered image referred as mask in the program is then used for locating centers.
5. Finding location of the three centers involves:
a) Finding contours in the mask relevant to colour range.
b) Discarding contours of irrelevant areas using area filters.
c) Finding the largest contour amongst the remaining one’s and applying the method of moments to find the center.
4.2.3 Cursor Position
Defining cursor position with yellow. The user might be left or right handed, so a video frame of rectangular sub
portion of smaller size is considered. Due to the noise captured and vibrations of the hand the centers keep dislocating the mean position. We use setCursorPos() so that the new center position is set close to the old center. Now the three centers are sent for deciding what action to be performed depending upon their relative position. This is done in the chooseAction() function in the code depending upon its output. The performAction() function carries out either of the following pyaotogui library function: click, select, drag, scroll.
4.2.4 Controlling Mouse
a) Moving mouse cursor
For finding the cursor on the screen and for the cursor moment any specific colour (yellow) centroids of a specify finger are used to perform movement on the screen.
b) Clicking Action
Clicking action is based on the detection of coloured area and its centroid.
• Yellow colour is used for cursor movement
• Yellow and Red is used for right click movement
• Red and Blue is used for left click movement
• Blue in downward direction for scroll up
• Red in downward direction for scroll down
• Yellow, Red, Blue for drag and scroll
4.3 Pseudo Code
Step 1. HSV (Hue, Saturation, Value)
The video captured is converted into hsv format. This helps to detect an object with a certain colour.
hsv=cv2.cvtColour(frame,cv2.COLOUR_BGR2HSV)
Step 2. Colour Calibration
Colour calibration is to measure and/or adjust the colour response of a device.
Input for colour ranges of each colour in inRange() functions.
blue_range=np.array([[88,78,20],[128,255,255]])
yellow_range=np.array([[21,70,80],[61,255,255]]
red_range=np.array([[0,95,82],[180,255,255]])
Each colour range is calibrated by using cv2.inRange() function.
mask=cv2.inRange(hsv_frame,colour_Range[0], colour_Range[1])
Step3. Noise Removal
The noise removal algorithms reduce or remove the visibility of noise by smoothing the entire image, leaving areas near contrast boundaries. It is done in two step morphism i.e. erosion and dilation. Dilation adds pixels to the boundaries of objects in an image, while erosion removes pixels on object boundaries.
eroded = cv2.erode(mask, kernel, iterations=1)
dilated = cv2.dilate( eroded, kernel, iterations=1)
Step 4. Centroid Detection
The centers of each colours are detected using the method of moments.
M = cv2.moments(contour[0])
if M['m00'] != 0:
cx = int(M['m10']/M['m00'])
cy = int(M['m01']/M['m00'])
Step 5. Set Cursor Position
The yellow coloured finger is used for cursor movement. Due to the noise captured while calibrating the colour the centroid vibrates reduce the vibrations of the cursor we compare the new position with the previous position of the cursor using the def setCursorPos() function. The new cursor position is calculated in such a way that the mean deviation from the desired steady state is reduced.
Step 6. Perform Mouse Movements
Based on the position of the cursor left click, right click, scroll up, scroll down, drag/select are performed.
IF distance yellow, red<50 & yellow, blue<50 & red, blue<50
DO drag
elseif distance red, blue<40
DO left click
elseif distance yellow, red<40
DO right click
elseif distance yellow, red<40, red-blue>120
DO scroll down
elseif distance blue-red>110:
DO scroll up
else setCursorPos()
5. RESULT AND DISCUSSION
5.1 Calibration
Each colour value is adjusted so that centroid of each colour is detected.
Fig. 2 Calibration
5.2 Centroid Detection
• Centers of yellow, red, blue are detected.
Fig. 3 Centroid Detection
5.2 Mouse Functions
a) Left Click
• When the Red and Blue tapes are brought together and cross a certain threshold distance left click action is performed.
Fig. 4 Hand gesture for Left click action
b) Right Click
• When the Red and Yellow tapes are brought together and cross a certain threshold distance right click action is performed.
Fig. 5 Hand gesture for Right click action
c) Drag and Select
• All the three tapes should be together for selection and dragging. The distance should be minimum between the centers of the colour.
Fig. 6 Hand gesture for Drag and Select operation
d) Scrolling Up
• Move the blue coloured finger in the downward direction to scroll up.
Fig. 7 Hand gesture for Scroll up operation
e) Scrolling Down
• Move the red coloured finger in the downward direction to scroll down.
Fig. 8 Hand gesture for Scroll down operation
6. FUTURE SCOPE:
Future work can involve introduction of an infrared sensor, so it can detect hands perfectly when the lighting conditions are not good. In progressive implementation, we can try implementing without using coloured tapes. The application can be further extended to gaming. Gestures for page zoom in and zoom out can be implemented. This technology has wide applications in the fields of augmented reality, biomedical instrumentation, computer graphics, prosthetics, and computer gaming.
7. CONCLUSION:
We developed a system to control the mouse cursor using a real-time camera. We implemented all mouse tasks such as left clicking, right clicking, and scrolling. In the future, we plan to add more features such as enlarging and shrinking windows, closing the window, etc. Our motive was to create this technology in the cheapest possible way and also to create it under a standardized operating system. Various application programs can be written exclusively for this technology to create a wide range of applications with the minimum requirement of resources.
8. REFERENCES:
[1] Chetana S. Ingulkar, A.N. Gaikwad; Hand Data Glove: A wearable real time device for human computer Interaction; J. International Journal of Science and Engineering, ISSN-2347-2200, Volume 1, Number 2; 2013.
[2] Zhi-hua Chen, Jung-Tae Kim, Jianning Liang, Jing Zhang, and Yu-Bo Yuan; Research Article Real-Time Hand Gesture Recognition Using Finger Segmentation; Department of Computer Science and Engineering, East China University of Science and Technology, Shanghai 200237, China;25 June 2014.
[3] Chu-Feng Lien; “Portable Vision-Based HCI – A Real time Hand Mouse System on Handheld Devices”; National Taiwan University, Computer Science and Information Engineering Department.
[4] Kamran Niyazi, Vikram Kumar, Swapnil Mahe and Swapnil Vyawahare; Mouse Simulation Using Two Coloured Tapes; Department of Computer Engineering, AISSMS COE, University of Pune, India International Journal of Information Sciences and Techniques (IJIST) Vol.2, No.2; March 2012.
[5] A. Erdem, E. Yardimci, Y. Atalay, V. Cetin; Computer vision-based mouse, A. E. Acoustics, Speech, and Signal Processing; Proceedings. (ICASS). IEEE International Conference;2002.
