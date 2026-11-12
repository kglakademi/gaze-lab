# Gaze lab

Webcam eye tracking in the browser for student projects at the Royal Danish Academy.

Open https://kglakademi.github.io/gaze-lab/ in Chrome or Edge on a computer with a webcam. Enter a participant ID, the viewing distance and the screen width, select images or videos, and follow the calibration. At the end the page offers a gaze table, a session file, overlay videos, heatmaps, scanpaths and a fixation table for download.

The camera video and the gaze data never leave the participant's computer. Everything runs in the browser.

You can draw rectangular areas of interest on each stimulus, either on the start page right after selecting the images or on the analysis page after a session. Export AOI table saves the areas as `aois.csv` with pixel coordinates of the original image, and Import AOI table applies such a table again whenever an image with the same file name is used. The analysis adds the area to every fixation and produces an area summary with fixation count, dwell time, share of dwell time, time to first fixation and number of visits per participant.

On the analysis page you can also replace the background of the plots with your own version of a stimulus. Besides the still scanpath, each participant gets a scanpath video per stimulus in which time is cut into bins of 500 ms that fade into each other. "Analyse saved recordings" on the start page pools gaze tables from several participants.

Fixations are detected from median-smoothed gaze. A fixation lasts as long as gaze stays within 3 degrees of its centre, must last at least 200 ms, and is merged with the next one when both lie within 3 degrees. All three values can be changed on the analysis page.

Gaze estimation uses WebGazer.js 3.5.3 by the Brown WebGazer Team (Papoutsaki et al., 2016), included here under the GPLv3 licence, see WEBGAZER-LICENSE.md. Webcam eye tracking typically has an accuracy of several degrees of visual angle, so results support statements about larger regions of an image, not small details.
