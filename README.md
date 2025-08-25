# EYE-EEG0.99
Version 1.0 of the EYE-EEG extension for EEGLAB

For more information on this software, visit https://www.eyetracking-eeg.org

This fork takes most of the feedback variables that are usually just shown in the console, and additionally stores them in EEG.etc and ET.etc so they can be better processed in bulk. Logged metrics include:

parsesmi.m

- File successfully read and parsed?
- Other/unexpected messages found?

checksync.m

- Pearson correlation coefficient between both signals at zero lag
- Lag that maximizes cross-correlation (in samples)

rej_eyecontin.m

- Number of out-of-range samples found
- Number of bad intervals

synchronize.m

- Number of EEG and ET samples
- Estimated sampling rates
- Number of pauses
- Number of unmatched events
- Number of events within +-4 samples of perfect sync
- Mean absolute sync error (in ms)

detecteyemovements.m

- Number of fixations / saccades
- Mean Velocity thresholds used (L/R, Hor./Vert.)
- Saccade median amplitude: 
- Saccade median duration:  
- Saccade median peak veloc.
- Fixation median duration
- Fixation median position (L/R, Hor./Vert.)
