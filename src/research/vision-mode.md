---
title: Reconfiguring the Imaging Pipeline for Computer Vision
layout: layout.html
section: Research
---
# Reconfiguring the Imaging Pipeline for Computer Vision

Advancements in deep learning have ignited an explosion of research on efficient hardware for embedded computer vision. Hardware vision acceleration, however, does not address the cost of capturing and processing the image data that feeds these algorithms. We examine the role of the image signal processing (ISP) pipeline in computer vision to identify opportunities to reduce computation and save energy. The key insight is that imaging pipelines should be be configurable: to switch between a traditional photography mode and a low-power vision mode that produces lower-quality image data suitable only for computer vision. We use eight computer vision algorithms and a reversible pipeline simulation tool to study the imaging system’s impact on vision performance. For both CNN-based and classical vision algorithms, we observe that only two ISP stages, demosaicing and gamma compression, are critical for task performance. We propose a new image sensor design that can compensate for these stages. The sensor design features an adjustable resolution and tunable analog-to-digital converters (ADCs). Our proposed imaging system’s vision mode disables the ISP entirely and configures the sensor to produce subsampled, lower-precision image data. This vision mode can save ~75% of the average energy of a baseline photography mode with only a small impact on vision task accuracy.

TODO: Figures; main findings.

## Publication

Mark Buckler, Suren Jayasuriya, and Adrian Sampson.
Reconfiguring the Imaging Pipeline for Computer Vision.
In the IEEE International Conference on Computer Vision (ICCV), 2017.

[preprint PDF][paper], [supplementary material PDF][supp]

    @inproceedings{buckler-iccv2017,
        author = {Mark Buckler and Suren Jayasuriya and Adrian Sampson},
        title = {Reconfiguring the Imaging Pipeline for Computer Vision},
        booktitle = {The IEEE International Conference on Computer Vision (ICCV)},
        year = {2017},
    }

[paper]: /pubs/visionmode-iccv2017.pdf
[supp]: /pubs/visionmode-iccv2017-supplemental.pdf

## Code

## Results