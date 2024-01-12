# C-SLAKE Dataset

Here we made  the C-SLAKE publicly. 
The motivation for this dataset is to ensure the robustness of our model . We extend the publicly available Med-VQA dataset [Slake](http://www.med-vqa.com/slake.) 
to a  consistent Med-VQA dataset C-SLAKE for further consistency assessment.

The dadaset can be used for  general Med-VQA task, and also for testing model consistency.

### Folder structure

This is  the folder structure of the dataset:

**📦C-SLAKE**\
 ┣**📂[imgs](https://drive.google.com/drive/my-drive)**\
 ┃┗*Contains images and corresponding question and answer pairs.*\
 ┣**📂train**\
 ┃┗*Contains train question answer pairs.*\
 ┣**📂validate**\
 ┃┗*Contains validate question answer pairs.*\
 ┣**📂test**\
 ┃┗*Contains test question answer pairs.*

You can download the image from the above link and put it in the C-SLAKE folder.
### Question types
The questions in our dataset are selected from the Slake dataset. We conducted role-tag annotation humanly to establish connections
between interconnected question-answer pairs corresponding to the identified medical images. Diagnostic question-answer pairs are categorized into three distinct roles. The distribution of role-type questions
is presented in the following table.

**Statistics of question in different role types over training, validation, and testing sets:**

| Role-type | train | Val | Test | Total |
|-----------|-------|-----|------|-------|
| Main      | 1222  | 237 | 246  | 1705  |
| Context   | 814   | 158 | 170  | 1142  |
| Ind       | 2294  | 514 | 508  | 3316  |
| Overall   | 4330  | 909 | 924  | 6163  |

The  C-SLAKE dataset encompasses a diverse array of medical materials,including Computed
Tomography (CT) scans, Magnetic Resonance Imaging (MRI)scans, and X-Ray images. The distribution of it is presented in the following table:

**The distribution of diverse array of medical materials**

| Modality-type | nums | 
|---------------|------|
| CT            | 282  | 
| MRI           | 181  | 
| X-Ray         | 179  | 
| Overall       | 642  | 

## Acknowledgement
This dataset was extended by [Slake](http://www.med-vqa.com/slake). We thank the original authors for their work and open source dataset.

[//]: # (generate Slake-C dataset by manually annotating the Slake dataset.)

[//]: #
[//]: # (In our dataset, the questions are related because in the Slake dataset )

[//]: # (there are interrelated low-level questions similar to high-level questions asking )

[//]: # (about medical conditions and corresponding answers leading to high-level questions)

[//]: # (questions are related because there is a high-level question about the DME grade of the image, )

[//]: # (and associated low-level questions that can lead to the answer of the high-level question. )

[//]: # (This allows to study the consistency of a VQA model i.e. how often the model produces contradictory answers to questions about a given image. )

[//]: # (Questions about regions are also a novel feature of this dataset.)