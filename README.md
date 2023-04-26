# MEGHACK_2023_spring

## Location info
https://megcore.nih.gov/index.php/MEG_Hackathon_2023

# Ideas
## Eyetracking v ground truth
Co-Leads: Rohini Kumar and Sebastion Montesinos <br>
-- Eye tracking data will be collected in the next week or two <br>
-- Objective - Minimize the average error between the on-screen eye fixation mark and calculated eye location <br>
-- Fork this repository: https://github.com/nih-megcore/nih_to_mne.git <br>
---- Use this as a base file for ideas: nih2mne/eyetracking_preprocessing.py <br>

## Epilepsy spike spread vs white matter connectivity
Lead: Price Withers
-- ...

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






