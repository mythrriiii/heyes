#HEYES
![image](https://github.com/user-attachments/assets/5bbd0d40-3746-4f32-b3a7-d6c731ef5d9a)


# Inspiration
We noticed a problem. Even with more than 70 million people around the world using sign language to communicate, there is a disconnect between them and the “hearing” society. In the computational ethics class, we learned about the Americans with Disabilities Act along with the ACM honor code, both emphasizing that it is wrong to discriminate against people who are disabled or at a disadvantage to others. In reflection on both, we found that most technologies seemingly are not adapted for everyone and only consider the non-disabled majority as their target audience. Many times this discrimination is due to a lack of understanding and empathy between the parties. We wanted to find a way to bridge people with the least amount of effort on their part to eliminate any potential roadblocks between them. To do so, we created a visual-based dynamic application to ease communication between sign language and written languages that uses machine learning to improve its accuracy.

# What it does
Heyes uses your webcam to capture your signing and converts your gestures into statements. This can also be used to convert between different sign languages that each have their own specifications too!

# How we built it
We used Python interfaced with a Multilayer Perceptron (MLP) to test out an effective feedforward artificial neural network that can predict output with Kazuhito Takahashi’s open-sourced models. We used OpenCV to access real-time computer vision and train the application. Google MediaPipes converts the data collected into hand maps using different stick and dot designs. We placed an emphasis on training with a large dataset with a wide range of skin tones as historically, computer vision models have oftentimes been found to be biased against people of color. Utilizing 21 handmarks, MediaPipes is used in our training to recognize the patterns of the joints in our hands despite being at angles and different distances. TensorFlow is what helps us with logging information and training our program.

# Challenges we ran into
In developing this software, we started with a purely TensorFlow build. This created numerous integration errors as one of our laptops was running on an older computer and the other computer had issues downloading Python. Moreover, the results were not very accurate in different lighting and with different people, and the dataset that could be captured was very small. Upon noticing these errors, we changed the approach to utilize Google MediaPipe alongside TensorFlow to provide a program with higher accuracy. This project required several imports to run as we are using open-source software libraries, leading to us spending a considerable amount of time installing and updating software.

# Accomplishments that we're proud of
The fact that we discovered a way to make our inputs accurate is something we are very proud of. It made us understand that we can make a difference and have already taken a step towards it.

# What we learned
Our entire project resulted from attempting to empathize with people belonging to the sign language community. Working on this project greatly developed this sense of responsibility toward finding a solution to this divide. We improved a lot on teamwork and have surprisingly become pros at installing software and importing libraries. Working on two different platforms – Windows and Macbook – helped us learn and interact with the versatility of the software. Machine Learning plays a key role in our project. Our research into deep learning, MLP, feedforward prediction, and many such concepts was highly invigorating and kept us engaged.

# What's next for Heyes!
Heyes is a program that was created with a wide range of implementations and avenues for improvement. We are looking at being able to function as a full-fledged translator that can convert from one sign language to another. Accessibility is an extremely important aspect too, and we are looking toward adding a gesture-to-text component. In addition to translation, Heyes will expand to translate beyond the constraints of a desktop application. Heyes will be present in courtrooms to provide a cost-effective translator for those who communicate through sign language. Additionally, it will be implemented in hardware devices in schools to ease communication between peers and teachers, helping foster the next generation with a larger bridge between those who use sign language and those who use traditional vocal communication.

# Built With
- anaconda
- cv2
- jupyter-notebook
- keras
- mathplotlib
- mediapipes
- netron
- numpy
- python
- tensorflow
- vscode

# Try it out
- [www.figma.com](https://www.figma.com/proto/Ey6W2krAx9b54fd2ZCH4Fl/heyes-sign-language-interpretor?node-id=9-106&scaling=scale-down&page-id=0%3A1&starting-point-node-id=9%3A106)
