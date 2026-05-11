[![DOI](https://img.shields.io/badge/DOI-10.82901%2Fnemar.nm000171-blue)](https://doi.org/10.82901/nemar.nm000171)

# BNCI 2014-002 Motor Imagery dataset

BNCI 2014-002 Motor Imagery dataset.

## Dataset Overview

- **Code**: BNCI2014-002
- **Paradigm**: imagery
- **DOI**: 10.1007/s00500-012-0895-4
- **Subjects**: 14
- **Sessions per subject**: 1
- **Events**: right_hand=1, feet=2
- **Trial interval**: [3, 8] s
- **Runs per session**: 8
- **File format**: MAT
- **Data preprocessed**: True

## Acquisition

- **Sampling rate**: 512.0 Hz
- **Number of channels**: 15
- **Channel types**: eeg=15
- **Channel names**: EEG1, EEG2, EEG3, EEG4, EEG5, EEG6, EEG7, EEG8, EEG9, EEG10, EEG11, EEG12, EEG13, EEG14, EEG15
- **Montage**: Laplacian
- **Hardware**: g.USBamp
- **Software**: BCI2000
- **Reference**: left mastoid
- **Ground**: right mastoid
- **Sensor type**: Ag/AgCl
- **Line frequency**: 50.0 Hz
- **Online filters**: 8th order Butterworth band-pass filters
- **Cap manufacturer**: Guger Technologies OG
- **Cap model**: g.LADYbird
- **Electrode type**: active
- **Electrode material**: Ag/AgCl

## Participants

- **Number of subjects**: 14
- **Health status**: healthy
- **Age**: min=20.0, max=30.0
- **BCI experience**: mixed
- **Species**: human

## Experimental Protocol

- **Paradigm**: imagery
- **Number of classes**: 2
- **Class labels**: right_hand, feet
- **Trial duration**: 5.0 s
- **Study design**: Two-class motor imagery: right hand and feet. Cue-guided Graz-BCI training paradigm with recording, training, and feedback within a single session.
- **Feedback type**: continuous
- **Stimulus type**: bar_graph
- **Stimulus modalities**: visual
- **Primary modality**: visual
- **Synchronicity**: synchronous
- **Mode**: online

## HED Event Annotations

Schema: HED 8.4.0 | Browse: https://www.hedtags.org/hed-schema-browser

```
  right_hand
    ├─ Sensory-event, Experimental-stimulus, Visual-presentation
    └─ Agent-action
       └─ Imagine
          ├─ Move
          └─ Right, Hand

  feet
    ├─ Sensory-event, Experimental-stimulus, Visual-presentation
    └─ Agent-action
       └─ Imagine, Move, Foot

```
## Paradigm-Specific Parameters

- **Detected paradigm**: motor_imagery
- **Imagery tasks**: right_hand, feet
- **Imagery duration**: 5.0 s

## Data Structure

- **Trials**: 160
- **Trials per class**: right_hand=80, feet=80
- **Blocks per session**: 8
- **Trials context**: total per subject

## Preprocessing

- **Data state**: minimally preprocessed (online filtered)
- **Preprocessing applied**: True
- **Steps**: bandpass filtering
- **Filter type**: Butterworth
- **Filter order**: 8

## Signal Processing

- **Classifiers**: Random Forest, Shrinkage LDA
- **Feature extraction**: CSP, DFT, Bandpower
- **Frequency bands**: alpha=[6, 14] Hz; beta=[14, 40] Hz
- **Spatial filters**: CSP, Laplacian

## Cross-Validation

- **Method**: train-test split
- **Evaluation type**: within_subject

## Performance (Original Study)

- **Accuracy**: 79.3%
- **Peak Accuracy**: 89.67
- **Median Accuracy**: 80.42

## BCI Application

- **Applications**: communication, control
- **Environment**: laboratory
- **Online feedback**: True

## Tags

- **Pathology**: Healthy
- **Modality**: Motor
- **Type**: Motor Imagery

## Documentation

- **DOI**: 10.1515/bmt-2014-0117
- **Associated paper DOI**: 10.3217/978-3-85125-378-8-61
- **License**: CC-BY-ND-4.0
- **Investigators**: David Steyrl, Reinhold Scherer, Oswin Förstner, Gernot R. Müller-Putz
- **Contact**: david.steyrl@tugraz.at; reinhold.scherer@tugraz.at; oswin.foerstner@student.tugraz.at; gernot.mueller@tugraz.at
- **Institution**: Graz University of Technology
- **Department**: Institute for Knowledge Discovery, Laboratory of Brain-Computer Interfaces
- **Country**: Austria
- **Repository**: BNCI Horizon
- **Publication year**: 2014
- **Funding**: FP7 BackHome (No. 288566); FP7 ABC (No. 287774)
- **Keywords**: brain-computer interfaces, machine learning, random forests, regularized linear discriminant analysis, sensorimotor rhythms

## References

Scherer, R., Faller, J., Balderas, D., Friedrich, E. V., & Müller-Putz, G. (2015). Brain-computer interfacing: more than the sum of its parts. Soft Computing, 19(11), 3173-3186. https://doi.org/10.1007/s00500-012-0895-4

Notes

.. note::

``BNCI2014_002`` was previously named ``BNCI2014002``. ``BNCI2014002`` will be removed in version 1.1.

.. versionadded:: 0.4.0

See Also

BNCI2014_001 : 4-class motor imagery (BCI Competition IV Dataset 2a) BNCI2014_004 : 2-class motor imagery (Dataset B)
Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Hochenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A. and Jas, M. (2019). MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis. Journal of Open Source Software 4: (1896). https://doi.org/10.21105/joss.01896

Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., Oostenveld, R. (2019). EEG-BIDS, an extension to the brain imaging data structure for electroencephalography. Scientific Data, 6, 103. https://doi.org/10.1038/s41597-019-0104-8

---
Generated by MOABB 1.5.0 (Mother of All BCI Benchmarks)
https://github.com/NeuroTechX/moabb
