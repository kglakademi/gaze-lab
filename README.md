# Gaze lab

Webcam eye tracking in the browser for student projects at the Royal Danish Academy.

Open https://kglakademi.github.io/gaze-lab/ in Chrome or Edge on a computer with a webcam. Enter a participant ID, the viewing distance and the screen width, select images or videos, and follow the calibration. At the end the page offers a gaze table, a session file, overlay videos, heatmaps, scanpaths and a fixation table for download.

The camera video and the gaze data never leave the participant's computer. Everything runs in the browser.

After a session, or under "Analyse saved recordings" for several participants at once, you can draw rectangular areas of interest on each stimulus. The analysis then adds the area to every fixation and produces an area summary with fixation count, dwell time, share of dwell time, time to first fixation and number of visits per participant. Areas can be saved as an AOI file and loaded again, so a group can share the same areas.

Gaze estimation uses WebGazer.js 3.5.3 by the Brown WebGazer Team (Papoutsaki et al., 2016), included here under the GPLv3 licence, see WEBGAZER-LICENSE.md. Webcam eye tracking typically has an accuracy of several degrees of visual angle, so results support statements about larger regions of an image, not small details.
