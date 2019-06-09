---
layout: single
author_profile: true
share: true
comments: true
permalink: /
header:
  image: /assets/images/Banner_v2.4.png
---
{% include feature_row %}

_**The style of texts also carries imformation.**_

## Project Introduction

OC(optical character recognition) technology for converting images and scanned documents into text is fairly mature with a high accuracy. It is also widely accessible to the pubilic as being embedded in softwares such as Adobe Acrobat. However, the font information is not preserved during the process, meaning users need to reformat the document from the scratch. This is inconvenient and can possibly introduce human errors in editing. Thus, we propose to use both supervised and unsupervised machine learning to recognize and distinguish typefaces of characters in scanned documents.

## Proposed Method

<img src="assets/images/method_diagram.png" alt="hi" class="inline"/>

The training sets consist of numbers of computer generated images of characters (A-to-Z) with different typefaces. This enables collecting a large amount of samples efficiently. to mimic the real-life data, which are scanned characters, random distortions and noises will be added when the images are generated. (Note that even though the training sets are software-generated, real-life data will be used to characterize the performance of the program.)

Both supervised and unsupervised methods are proposed. The goal of supervised machine learning will be to predict real-life scanned characters' typefaces. The goal of unsupervised machine learning will be to form clusters of characters with the same typeface.

Due to the complexity of the task, rather than targeting specific features set by researchers, neural networks will be used to figure out which features to look for.

## Anticipated Results

While computer generated images of characters in different typefaces (with noises and minor distortions) are used in the training phase, the final goal is to recognize or distinguish at least 3 typefaces from real-life images of characters taken from scanned documents.

- After unsupervised learning, we expect the program to be able to form clusters of scanned images of charaters based on the typefaces.

- After supervised learning, we expect the program to be able to give predictions of the typefaces of scanned images of charaters.

- High accuracies of both programs are expected. However, the accuracies of different letters are expected to be different as some letters are distinct among typefaces than others.

## Discussion
### Impact

The best outcome of this project would be a spin-off app that can recognize selected typefaces accurately from a scanned document. This would help many people who wants to recreate digital versions of scanned documents while the format needs to be preserved. We expect this program to be a crucial component for the future of historic preservation, publication, and even for computer vision.

### Next Steps

The project will lay solid fundation for future works. Some clear extensions that can be implemented are:

- Expanding to cover more typefaces;

- Adapting into plug-ins for exsiting softwares, such as Adobe Acrobat;

- Adding detections of other aspects of fonts, such as color, size, highlight, bold, italic, and underscore. 

## References

