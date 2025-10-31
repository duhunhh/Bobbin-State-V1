Bobbin-State-V1 Dataset

"Bobbin-State-V1" is an industrial image dataset built specifically for bobbin status detection. All images were acquired via an online image acquisition system deployed in the test workshop of a modern textile factory, ensuring the data's authenticity and scene relevance.

1. Dataset Construction

Data Scale: After filtering and cleaning, the dataset contains a total of 13,972 high-quality images.

Data Split: The dataset is divided into training, validation, and test sets according to an 8:1:1 ratio.

Training Set: 11,178 images

Validation Set: 1,398 images

Test Set: 1,398 images

2. Annotation and Classes

Based on the practical requirements of the spinning process, the dataset strictly defines three industrial states, which are inferred from two basic detection classes.

Industrial States (3 types):

No Bobbin

Empty Bobbin

Yarn Bobbin

Basic Detection Classes (2 types):

Bobbin

Yarn

3. State Mapping Logic

The three industrial states are determined by the combination of the basic detection classes:

No Bobbin: The model detects no target (corresponding to unlabeled images).

Empty Bobbin: The model detects only the "Bobbin" target.

Yarn Bobbin: The model detects both "Bobbin" and "Yarn" targets.

4. Data Statistics

The statistics for annotated targets in the dataset are as follows:

Class

Total Instances

Bobbin

12,267

Yarn

6,535

Note: The dataset also includes 1,705 unlabeled images, which correspond to the "No Bobbin" state.

5. Dataset Download

In addition, our dataset is too large for you to download directly. We provide you with the following two download methods.

Quark Netdisk

URL: https://pan.quark.cn/s/fb9977b1d2b3

Extraction code: hEQP

Baidu Netdisk

URL: https://pan.baidu.com/s/1laSbixrVfpY8rlt0Zl8eTg?pwd=egcf

Extraction code: egcf

6. Contact

If you have any problem, please contact me by email: 2024487434@qq.com.
