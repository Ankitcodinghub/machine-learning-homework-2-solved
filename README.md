# machine-learning-homework-2-solved
**TO GET THIS SOLUTION VISIT:** [Machine Learning Homework 2 Solved](https://www.ankitcodinghub.com/product/machine-learning-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;121230&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;6&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (6 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Machine Learning Homework 2  Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (6 votes)    </div>
    </div>
Machine Learning HW2

Outline

● Task Introduction

● Dataset &amp; Data Format

● Submission &amp; Grading

Task Introduction

Task Introduction

1. Data Preprocessing: Extract MFCC features from raw waveform (already done by TAs!)

2. Classification: Perform framewise phoneme classification using pre-extracted MFCC features

Task Introduction

Task: Multiclass Classification M M M AH AH SH SH IH IH IH N N N N …

Framewise phoneme prediction from speech.

What is a phoneme?

A unit of speech sound in a language that can serve to distinguish one word from the other.

● bat / pat , bad / bed

● Machine Learning → M AH SH IH N L ER N IH NG

Data Preprocessing

Data Preprocessing

Acoustic Features – MFCCs (Mel Frequency Cepstral Coefficients)

shape (n, 39) label

More Information About the Data

Since each frame only contains 25 ms of speech, a single frame is prev frames future frames unlikely to represent a complete phoneme

● Usually, a phoneme will span several frames

● Concatenate the neighboring phonemes for training

Finding testing labels or doing human labeling are strictly prohibited!

Introduction to Digital Speech Processing

Dataset &amp; Data Format

Dataset

LibriSpeech (subset of train-clean-100)

● Training: 4268 preprocessed audio features with labels (total 2644158 frames)

● Testing: 1078 preprocessed audio features (total 646268 frames)

● Label: 41 classes, each class represents a phoneme

train_split.txt train_labels.txt

Data Format

● Data Format (The TAs have already extracted the features) libriphone/ features: 39-dim MFCC w/ CMVN{filename}.pt for each utterance(audio)

– train_split.txt (train metadata)

– train_labels.txt (train labels)

– test_split.txt (test metadata) – feat/

– train/

– test/

Using additional data is prohibited. Your final grade will be multiplied by 0.9!

Data Format

● Each .pt file is extracted from one original wav file

● Use torch.load() to read in .pt files as torch tensors ● Each tensor has a shape of (T, 39)

39 dims

T frames

Submission &amp; Grading

Submission &amp; Grading

● Leaderboard (4%): Kaggle

● Code submission (2%): NTU COOL

● Report submission (4%): Gradescope

Kaggle Public Baselines

● (1%) Simple baseline: 0.45797 (sample code)

● (1%) Medium baseline: 0.69747 (concat n frames, add layers)

● (1%) Strong baseline: 0.75028 (concat n, batchnorm, dropout, add layers)

● (1%) Boss baseline: 0.82324 (sequence-labeling(using RNN))

For boss baseline, you can refer to pervious course recording of RNN: video 1 and video 2.

Kaggle Link: https://www.kaggle.com/c/ml2022spring-hw2

● Displayed name: &lt;student ID&gt;_&lt;anything&gt;

○ e.g. b06901020_puipui

● Up to 2 submissions will be considered for the private leaderboard.

Code Submission (2%)

● Compress your code and report, then submit it to NTU COOL.

&lt;student ID&gt;_hw2.zip

e.g. b06901999_hw2.zip

● We can only see your last submission.

● Do not submit your model or dataset.

● If your code is not reasonable, your final grade will be multiplied by 0.9!

Report Questions

1. (2%) Implement 2 models with approximately the same number of parameters, (A) one narrower and deeper (e.g. hidden_layers=6, hidden_dim=1024) and (B) the other wider and shallower (e.g. hidden_layers=2, hidden_dim=1700). Report training/validation accuracies for both models.

2. (2%) Add dropout layers, and report training/validation accuracies with dropout rates equal to (A) 0.25/(B) 0.5/(C) 0.75 respectively.

Report Submission

● Submit with gradescope, no need to upload any files.

● We can only see your last submission.

2. Entry Code: ZR2P36

Gradescope Registration

1.

3.

Gradescope Submission

Regulations (＊) Academic Ethics Guidelines for Researchers by the

Ministry of Science and Technology

● You should NOT plagiarize, if you use any other resource, you should cite it in the reference. (＊)

● You should NOT modify your prediction files manually.

● Do NOT share codes or prediction files with any living creatures.

● Do NOT use any approaches to submit your results more than 5 times a day.

● Do NOT use additional data or pre-trained models.

● Your assignment will not be graded and your final grade x 0.9 if you violate any of the above rules.

● Prof. Lee &amp; TAs preserve the rights to change the rules &amp; grades.

If you have any questions, you can ask us via…

● NTU COOL (recommended)

○ https://cool.ntu.edu.tw/courses/11666

● Email

○ The title should begin with “[hwX]” (X is the homework number)

○ TBD
