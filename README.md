# detector
detector stuff: tests, examples, etc...

SIMPLE LARGE BB REGRESSION

1. the file detector_bbox_regression.ipynb:
is a simple regression example. The network is a simple resnet with a custom head that produces
4 + num_class outputs (4 BB and 21 classes).

2. In order to do that the input is an image with its corresponding large BB with corresponding classe.

3. To resume:
INPUT: Image + Largest BB in Image + Corresponding class --------> OUTPUT: 4 (BB corners) + 21 probabilies 

4. So there is two loss a L1 loss on the BB and cross_entropy loss on the classe
