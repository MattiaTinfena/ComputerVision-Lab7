# ComputerVision-Lab7
## Motion Detection, Optical Flow and Tracking

MATLAB experiments comparing motion-detection methods and tracking a selected target in video sequences.

### Experiments

- Compare static-background subtraction with an adaptive running-average model.
- Compare running-average change detection with Lucas–Kanade optical flow.
- Segment and track a target in a separate video sequence.
- Visualise flow magnitude and direction.

### Requirements

MATLAB with Image Processing Toolbox and support for reading the supplied MP4 videos.

### Run

```bash
git clone https://github.com/MattiaTinfena/ComputerVision-Lab7.git
```

Set the repository root as MATLAB’s current folder and run:

```matlab
main
```

The main script processes `videos/luce_vp.mp4`, `videos/tennis.mp4` and `videos/DibrisHall.mp4`. Keep these paths available and follow any interactive selection requested by the tracking routine.

### Main files

- `compareCDAlgo.m`: comparison of background models.
- `compareCDOF.m`: change detection and optical-flow comparison.
- `LucasKanade.m`, `ComputeDerivatives.m`: optical-flow computation.
- `segmentAndTrack.m`: target segmentation and tracking.
- `convertToMagDir.m`: flow visualisation.

Parameters are selected for the supplied videos. Different scenes may require changes to thresholds, background adaptation and window sizes. This repository derives from course project material; retain the existing upstream attribution and history.
