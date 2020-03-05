# LiveFaceNet
A live face detector application using the Inception Resnet V2 model(for blink detection).
And cv2's face_recognition library to detect faces.

A few tweaks made to the Inception Resnet V-2 algorithm:

- Dropout was removed to ensure better training and validation accuracy
- "he_normal" kernel_initializer was used in the convolutional blocks
- Since the classic Inception Resnet v-2 has multiple outputs and uses softmax classifier, "SIGMOID" activation was used here for binary blink detection instead

Train accuracy for Blink Detection Model: 93.84
Validation Accuraacy for Blink Detection Model: 92.50

Data for the blink detection was collected from:  http://parnec.nuaa.edu.cn/xtan/data/ClosedEyeDatabases.html (Raw face Image in the background)
