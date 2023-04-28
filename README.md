# MEGHACK_2023_spring

## Location info
https://megcore.nih.gov/index.php/MEG_Hackathon_2023

### Github SSH key setup
https://github.com/nih-megcore/MEGHACK_2023_spring/wiki/Connect-To-A-Github-Repository-Using-SSH

# Ideas
## Eyetracking v ground truth
Co-Leads: Rohini Kumar and Sebastion Montesinos <br>
https://github.com/sebmonte/MEG-Hackathon/tree/main <br>
-- Eye tracking data will be collected in the next week or two <br>
-- Objective - Minimize the average error between the on-screen eye fixation mark and calculated eye location <br>
-- Fork this repository: https://github.com/nih-megcore/nih_to_mne.git <br>
---- Use this as a base file for ideas: nih2mne/eyetracking_preprocessing.py <br>

## Epilepsy spike spread vs white matter connectivity
Lead: Price Withers <br>
- Goal: Replicate figures 3A-B and 4A-B from [_Integration of white matter architecture to stereo-EEG better describes epileptic spike propagation_](https://doi.org/10.1016/j.clinph.2022.10.012) using MEG data <br>
- Dataset: 10-15 MEG patients w/ and w/out patient-specific DTI data. Spikes have been marked ahead of time and SC matrices have been created in advance. <br>
- 2 group members will determine latencies between "Propagation Pairs". The initial spiking region from averaged IEDs will have a latency of 0ms and all other regions which show significant activation will have their own latency at the time of activion. Goal output: 1 vector of size n_parcels per patient with latencies of spiking. Majority of values will be NaN and timings will range from 0ms to ~100ms.
- 2 group members will write code to convert latency vectors and DWI connectivity matrices into figures 3A-B and 4A-B. Since this will not be available until end of day, they can use random vectors until data are prepared. Additional analyses can be prepared to incorporate pre- and post-operative DWI data and seizure free/persist outcomes.

## Statistical Group analysis
(No Lead Currently) <br>
-- Use the HV data: https://openneuro.org/datasets/ds004215/versions/1.0.2  <br>
-- Some of the datasets will be pre-processed to source activations <br>
-- Use the online pages to calculate group statistics on the data: https://mne.tools/stable/statistics.html <br>

## Reaction time v activation
(No Lead) <br>
-- HV data can be used and will be prepped <br>
-- Assess reaction time versus stimulus time <br>
-- Regress stimulus time versus activation over group data <br>

## Harmonization Procedures for consortium data
Allison Nugent <br>
-- Use combat/covbat/etc on initial open MEG data from the Enigma MEG Project

## Effects of ICA group based initial conditions versus random start
Jeff Stout <br>
-- ICA is typically started from a random seed <br>
-- Use group ICA to generate average topographies <br>
-- Set average topos as starting conditions prior to iteration <br>
-- Assess stability of resulting ICAs and number of components used per artifact <br>






