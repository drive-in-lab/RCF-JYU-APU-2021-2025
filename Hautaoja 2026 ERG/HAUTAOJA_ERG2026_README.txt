This readme file was generated on 2026-05-28 by Toni Hautaoja


GENERAL INFORMATION

Principal Investigator Information
Name: Tuomo Kujala
ORCID: 0000-0001-8222-8540
Institution: University of Jyväskylä
Address: Seminaarinkatu 15, PO Box 35, 40014 University of Jyväskylä
Email: tuomo.kujala@jyu.fi


- Date of data collection: The two empirical driving-simulator experiments between 2021-2022 and model simulations between 2024-2025. NOTE: Experiment 1 corresponds to the previously published dataset reported by Grahn et al. (2024), Experiment 2 was used as an independent validation dataset, and model simulation data were generated during model development and evaluation.
- Geographic location of data collection: Jyväskylä, Finland
- Information about funding sources that supported the collection of the data: This research was supported by Research Council of Finland [Appropriate Uncertainty in Manual and Automated Driving, grant 343259]. 


SHARING/ACCESS INFORMATION

- Licenses/restrictions placed on the data: CC BY-NC
- Links to publications that cite or use the data: https://doi.org/10.1080/00140139.2026.2654083
- Recommended citation for this dataset:
Hautaoja, T. (2026). Predicting driver adaptability: A computational rationality model for attention allocation in lateral vehicle control. Ergonomics, Early online. https://doi.org/10.1080/00140139.2026.2654083


DATA & FILE OVERVIEW

File List: 
EXP1&2_SUMMARY.csv
EXP1&2_SUMMARY_SDLP.csv
EXP1_MO.csv
EXP1_SO.csv
EXP2_MO.csv
EXP2_SO.csv
Model source code available: https://gitlab.com/toninikolaialeksanteri/driver-adaptability


METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:
Hautaoja, T. (2026). Predicting driver adaptability: A computational rationality model for attention allocation in lateral vehicle control. Ergonomics, Early online. https://doi.org/10.1080/00140139.2026.2654083

Methods for processing the data:
Hautaoja, T. (2026). Predicting driver adaptability: A computational rationality model for attention allocation in lateral vehicle control. Ergonomics, Early online. https://doi.org/10.1080/00140139.2026.2654083



DATA-SPECIFIC INFORMATION FOR: EXP1&2_SUMMARY.csv

- Number of variables: 15

- Number of cases/rows: 210

- Variables included in this file:
id, OT, occ_total, l_exc_occ, l_exc_nonocc, steering_amp, TLC_model_ALL, TLC_before_occ, TLC_after_occ, OTTLC, occ_per_10sec, l_exc_10sec, speed, group, filter_$

- Description:
Aggregated model and human summary data used for the main model-comparison figures and analyses. The main paper-level comparison variables in this file are occlusion time, TLC-related values, occlusion frequency, lane excursions, steering amplitude, speed, and group.

- File-specific filter information:
filter_$ indicates the applied filter in SPSS. In this file, speed = 2 was used as the filter.


DATA-SPECIFIC INFORMATION FOR: EXP1&2_SUMMARY_SDLP.csv

- Number of variables: 10

- Number of cases/rows: 60

- Variables included in this file:
id, avg.offset.sd, experiment, t_mean, t_distance_in_m, avg_OT, o_distance_in_m, sdlp_per_m, avg_sdlp_ot, avg_sdlp_od

- Description:
Participant-level summary file for Experiment 1 and Experiment 2. This file contains SDLP-related measures, occlusion duration, occlusion distance, and SDLP normalized by time or distance. In the publication, these values were used to examine whether Experiment 2 participants differed from Experiment 1 participants in lateral control accuracy under occlusion.


DATA-SPECIFIC INFORMATION FOR: EXP1_MO.csv

- Number of variables: 31

- Number of cases/rows: 3575

- Variables included in this file:
id, t, drive, speed.kmh, occ_nr, x, y, yaw, steer, off, speed, leftTLC, rightTLC, report, OT, OTTLC, true.TLC, FADE1.leftTLC, FADE1.rightTLC, FADE1.off, FADE1.TLC.min, FADE0.TLC.min, steer.ampl, steer.min, steer.max, steer.avg, steer.sd, offset.min, offset.max, offset.avg, offset.sd

- Description:
Unfiltered Experiment 1 multiple-occlusion event-level data. These data document occlusion-level driving events and simulator-state summaries for the multiple-occlusion task.

- File-specific filter information:
The following filter was used for the analyses based on this data:
OTTLC < 70 & OTTLC > 0 & steer.ampl.450 < 15 & FADE1.TLC.min < 70 & FADE1.TLC.min > 0 & FADE1.off.changed75.abs < 7 & last_FADE0.off.changed75.abs < 7


DATA-SPECIFIC INFORMATION FOR: EXP1_SO.csv

- Number of variables: 31

- Number of cases/rows: 1499

- Variables included in this file:
id, t, drive, speed.kmh, occ_nr, x, y, yaw, steer, off, speed, leftTLC, rightTLC, report, OT, OTTLC, true.TLC, FADE1.leftTLC, FADE1.rightTLC, FADE1.off, FADE1.TLC.min, FADE0.TLC.min, steer.ampl, steer.min, steer.max, steer.avg, steer.sd, offset.min, offset.max, offset.avg, offset.sd

- Description:
Unfiltered Experiment 1 single-occlusion event-level data. These data document occlusion-level driving events and simulator-state summaries for the single-occlusion task.

- File-specific filter information:
The following filter was used for the analyses based on this data:
last_FADE0.off.changed75 < 7


DATA-SPECIFIC INFORMATION FOR: EXP2_MO.csv

- Number of variables: 31

- Number of cases/rows: 2030

- Variables included in this file:
id, t, drive, speed.kmh, occ_nr, x, y, yaw, steer, off, speed, leftTLC, rightTLC, report, OT, OTTLC, true.TLC, FADE1.leftTLC, FADE1.rightTLC, FADE1.off, FADE1.TLC.min, FADE0.TLC.min, steer.ampl, steer.min, steer.max, steer.avg, steer.sd, offset.min, offset.max, offset.avg, offset.sd

- Description:
Unfiltered Experiment 2 multiple-occlusion event-level data. These data document occlusion-level driving events and simulator-state summaries for the independent validation experiment.

- File-specific filter information:
The following filter was used for the analyses based on this data:
OTTLC < 70 & OTTLC > 0 & steer.ampl.450 < 15 & FADE1.TLC.min < 70 & FADE1.TLC.min > 0 & FADE1.off.changed75.abs < 7 & last_FADE0.off.changed75.abs < 7


DATA-SPECIFIC INFORMATION FOR: EXP2_SO.csv

- Number of variables: 31

- Number of cases/rows: 894

- Variables included in this file:
id, t, drive, speed.kmh, occ_nr, x, y, yaw, steer, off, speed, leftTLC, rightTLC, report, OT, OTTLC, true.TLC, FADE1.leftTLC, FADE1.rightTLC, FADE1.off, FADE1.TLC.min, FADE0.TLC.min, steer.ampl, steer.min, steer.max, steer.avg, steer.sd, offset.min, offset.max, offset.avg, offset.sd

- Description:
Unfiltered Experiment 2 single-occlusion event-level data. These data document occlusion-level driving events and simulator-state summaries for the independent validation experiment.

- File-specific filter information:
The following filter was used for the analyses based on this data:
last_FADE0.off.changed75 < 7


- Variable List:

The variables below include both main paper-level analysis variables and intermediate simulator/log-processing variables. The main paper-level comparison variables are OT, TLC/OTTLC, occlusion frequency, speed, group, lane excursions, steering amplitude, and SDLP/m. Other variables are included to document the event-level simulator data and filtering/reconstruction pipeline.

Core analysis and model-comparison variables:

id: Participant or model-run identifier.

group: Group/category label. Values include model1, model2, human exp 1, and human exp 2.

experiment: Experiment identifier.

speed: Speed condition or speed variable. In aggregated data, this refers to the speed condition of 60 km/h or 100 km/h.

speed.kmh: Driving speed in kilometers per hour.

OT: Occlusion time. In aggregated files, this is average occlusion duration; in event-level files, this is occlusion-event duration. Unit: seconds.

OTTLC: OT + TLC. This represents occlusion-time-plus-time-to-line-crossing performance.

true.TLC: Actual time-to-line-crossing during the occlusion. A value of 0 indicates that the vehicle did not leave the lane during the occlusion.

TLC_model_ALL: Time-to-line-crossing averaged over all TLC values of the episode. MODEL DATA ONLY.

TLC_before_occ: Time-to-line-crossing averaged before occlusion. MODEL DATA ONLY.

TLC_after_occ: Time-to-line-crossing averaged after occlusion. MODEL DATA ONLY.

occ_total: Total number of occlusions.

occ_per_10sec: Occlusions per 10 seconds. Calculated as (occ_total / driving time) * 10. Driving time was 124.12 s at 100 km/h and 210.15 s at 60 km/h.

l_exc_occ: Lane excursions during occlusion.

l_exc_nonocc: Lane excursions during attention / non-occluded periods.

l_exc_10sec: Lane deviations per 10 seconds.

steering_amp: Average steering amplitude during occlusions.

steer.ampl: Steering amplitude during occlusion, calculated as the range between minimum and maximum steering values.

sdlp_per_m: SDLP per meter during occlusion, calculated per participant.

Event/log reconstruction variables:

t: Time variable.

drive: Drive or trial identifier.

occ_nr: Running occlusion number.

x: Vehicle x-coordinate in the simulator/log data.

y: Vehicle y-coordinate in the simulator/log data.

yaw: Vehicle heading/yaw angle.

steer: Steering value at the logged time point or event.

off: Offset when occlusion ends.

leftTLC: Time-to-line-crossing to the left lane boundary.

rightTLC: Time-to-line-crossing to the right lane boundary.

report: Report or event marker variable from the processed driving log.

Derived occlusion-start/end variables:

FADE1.leftTLC: Left TLC at the beginning of occlusion.

FADE1.rightTLC: Right TLC at the beginning of occlusion.

FADE1.off: Offset at the beginning of occlusion.

FADE1.TLC.min: Shortest TLC at the beginning of occlusion, based on left/right TLC.

FADE0.TLC.min: Shortest TLC at the end of occlusion, based on left/right TLC.

Steering and offset summary variables:

steer.min: Minimum steering value during occlusion.

steer.max: Maximum steering value during occlusion.

steer.avg: Average steering value during occlusion.

steer.sd: Standard deviation of steering during occlusion.

offset.min: Largest offset value to the left during occlusion.

offset.max: Largest offset value to the right during occlusion.

offset.avg: Average offset during occlusion.

offset.sd: Standard deviation of offset during occlusion.

avg.offset.sd: Standard deviation of lane position during occlusion, averaged per participant.

avg_sdlp_ot: Average SDLP divided by OT for each participant.

avg_sdlp_od: Average SDLP divided by occlusion distance for each participant.

Other participant-level summary variables:

t_mean: Average total drive duration per participant.

t_distance_in_m: Average drive duration expressed as driven distance in meters per participant.

avg_OT: Average occlusion time per participant over 30 occlusions.

o_distance_in_m: Occlusion distance per participant over 30 occlusions.

Processing/filter variables:

filter_$: SPSS/R-style filter indicator. E.g., in EXP1&2_SUMMARY.csv, this indicates the applied speed filter.

- Missing data codes: space/NaN
