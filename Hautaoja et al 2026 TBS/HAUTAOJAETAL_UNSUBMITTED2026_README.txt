This readme file was generated on 2026-05-28 by Toni Hautaoja


GENERAL INFORMATION

Principal Investigator Information
Name: Tuomo Kujala
ORCID: 0000-0001-8222-8540
Institution: University of Jyväskylä
Address: Seminaarinkatu 15, PO Box 35, 40014 University of Jyväskylä
Email: tuomo.kujala@jyu.fi


- Date of data collection: The empirical data is from 2022, including driving simulator data from a curved and hilly road task and synchronized eye-tracking / area-of-interest data. Model simulation and training-output data were generated during model development and evaluation in 2026.
- Geographic location of data collection: Jyväskylä, Finland
- Information about funding sources that supported the collection of the data: This research was supported by Research Council of Finland [Appropriate Uncertainty in Manual and Automated Driving, grant 343259]. 


SHARING/ACCESS INFORMATION

- Licenses/restrictions placed on the data: CC BY-NC
- Links to publications that cite or use the data: Hautaoja, T., Han Wei, T., & Kujala, T. (unsubmitted manuscript). A hierarchical computational rationality model of visual sampling in lateral and longitudinal vehicle control.
- Recommended citation for this dataset:
Hautaoja, T., Han Wei, T., & Kujala, T. (unsubmitted manuscript). A hierarchical computational rationality model of visual sampling in lateral and longitudinal vehicle control.


DATA & FILE OVERVIEW

File List: 
ET_DATA.csv
ET_DATA_SUMMARY.csv
ET_DATA_SUMMARY_PERID.csv
SIM_DATA.csv
Model source code available: https://gitlab.com/toninikolaialeksanteri/driver-adaptability


METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:
Hautaoja, T., Han Wei, T., & Kujala, T. (unsubmitted manuscript). A hierarchical computational rationality model of visual sampling in lateral and longitudinal vehicle control.

Methods for processing the data:
Hautaoja, T., Han Wei, T., & Kujala, T. (unsubmitted manuscript). A hierarchical computational rationality model of visual sampling in lateral and longitudinal vehicle control.



DATA-SPECIFIC INFORMATION FOR: ET_DATA.csv

- Number of variables: 5 (key variables).

- Number of cases/rows: 458 026

- Variables included in this file:
ET_DATA.csv contains synchronized eye-tracking data for all participants after processing through Syncster. The key variables used for the model-fitting/background analyses were DS_mark_name, DS_mark_occluded, ET_Dikablis Glasses 3_Field Data_Scene Cam_Original_Lane / AoI_Lane, ET_Dikablis Glasses 3_Field Data_Scene Cam_Original_Speed / AoI_Speed, and ET_rec_time.

- Description:
Synchronized eye-tracking data used to derive area-of-interest (AoI) ratios for Lane, Speed, and None. These ratios were used as empirical background for fitting and evaluating the attention-allocation behavior of the model.


DATA-SPECIFIC INFORMATION FOR: ET_DATA_SUMMARY.csv

- Number of variables: 5

- Number of cases/rows: 3

- Variables included in this file:
subject_id, category, n_rows, percent, source_file

- Description:
Summary file of eye-tracking AoI ratios. Each participant has separate rows for the Lane, Speed, and None categories, describing the proportion of observations belonging to each attention/AoI category.


DATA-SPECIFIC INFORMATION FOR: ET_DATA_SUMMARY_PERID.csv

- Number of variables: 5

- Number of cases/rows: 81

- Variables included in this file:
subject_id, category, n_rows, percent, source_file

- Description:
Participant-level eye-tracking AoI summary file. This file contains the same key AoI-ratio structure as ET_DATA_SUMMARY.csv, organized per participant for Lane, Speed, and None comparisons.


DATA-SPECIFIC INFORMATION FOR: SIM_DATA.csv

- Number of variables: 53

- Number of cases/rows: 3240

- Variables included in this file:
t, id, drive, speed.kmh, occ_nr, x, y, yaw, steer, off, speed, speed.min, speed.max, mean_speed_kmh, median_speed_kmh, leftTLC, rightTLC, OT, OTTLC, true.TLC, FADE1.leftTLC, FADE1.rightTLC, FADE1.off, FADE1.speed, FADE1.TLC.min, FADE0.TLC.min, steer.ampl, steer.min, steer.max, steer.avg, steer.sd, offset.min, offset.max, offset.avg, offset.sd, occluded_now, deviation_counting_active, speed_oob_now, speed_deviation_event, occ_speed_deviation_event, vis_speed_deviation_event, total_speed_deviation_event_total, occ_speed_deviation_event_total, vis_speed_deviation_event_total, lane_oob_now, lane_deviation_event, occ_lane_deviation_event, vis_lane_deviation_event, total_lane_deviation_event_total, occ_lane_deviation_event_total, vis_lane_deviation_event_total, steer.ampl.450, FADE1.off.abs

- Description:
Driving simulator data from the curved and hilly road task used as empirical background for modeling speed management, lane keeping, multitasking, and attention allocation under occlusion. The file includes event-level driving measures, occlusion-related measures, TLC and offset variables, steering summaries, speed summaries, and lane/speed deviation indicators. Not all variables are central paper-level outcomes; several are included to document the simulator-event reconstruction and filtering pipeline.


- Variable List:

The variables below include both main paper-level analysis variables and intermediate simulator/log-processing variables. The main paper-level comparison variables are AoI ratios for Lane, Speed and None, OT, TLC/OTTLC, speed maintenance, lane and speed deviations, steering amplitude, offset, and attention allocation state. Other variables are included to document the event-level simulator data and filtering/reconstruction pipeline.

Eye-tracking and AoI variables:

DS_mark_name: Syncster/data-stream marker name indicating when occlusion event has started or ended. The marker refers to FADE0/unocclusion or FADE1/occlusion.

DS_mark_occluded: Occlusion-state marker. Values: 0 = unoccluded, 1 = occluded. This variable was used to calculate attention/AoI ratios.

ET_Dikablis Glasses 3_Field Data_Scene Cam_Original_Lane: Eye-tracking area-of-interest indicator for the lane/road area.

ET_Dikablis Glasses 3_Field Data_Scene Cam_Original_Speed: Eye-tracking area-of-interest indicator for the speedometer/speed area.

ET_rec_time: Eye-tracker timestamp.

subject_id: Participant identifier in eye-tracking summary files.

category: AoI category. Values: lane, speed, none.

n_rows: Number of rows/observations belonging to the AoI category.

percent: Percentage of rows/observations belonging to the AoI category. This is used as the empirical AoI ratio.

source_file: Original source file from which the participant/category summary was derived.

Core driving simulator and model-comparison variables:

id: Participant identifier.

t: Time variable.

drive: Drive or trial identifier.

speed.kmh: Driving speed in kilometers per hour.

speed: Vehicle speed in the simulator/log data.

mean_speed_kmh: Mean speed in kilometers per hour.

median_speed_kmh: Median speed in kilometers per hour.

speed.min: Minimum speed during the relevant event/window.

speed.max: Maximum speed during the relevant event/window.

occ_nr: Running occlusion number.

OT: Occlusion time; occlusion-event duration in seconds.

OTTLC: OT + TLC. This represents occlusion-time-plus-time-to-line-crossing performance.

true.TLC: Actual time-to-line-crossing during the occlusion. A value of 0 indicates that the vehicle did not leave the lane during the occlusion.

leftTLC: Time-to-line-crossing to the left lane boundary.

rightTLC: Time-to-line-crossing to the right lane boundary.

off: Offset when occlusion ends.

steer.ampl: Steering amplitude during occlusion, calculated as the range between minimum and maximum steering values.

steer.ampl.450: Steering-amplitude-related filtering/summary variable used in the processing pipeline.

occluded_now: Current occlusion state in the simulator/log data.

Lane and speed deviation variables:

deviation_counting_active: Indicator for whether deviation counting was active at the current time/event.

speed_oob_now: Indicator for whether speed is currently outside the target speed band.

speed_deviation_event: Indicator for a speed deviation event.

occ_speed_deviation_event: Indicator for a speed deviation event occurring during occlusion.

vis_speed_deviation_event: Indicator for a speed deviation event occurring during visual sampling/attention.

total_speed_deviation_event_total: Cumulative total number of speed deviation events.

occ_speed_deviation_event_total: Cumulative number of speed deviation events during occlusion.

vis_speed_deviation_event_total: Cumulative number of speed deviation events during visual sampling/attention.

lane_oob_now: Indicator for whether the vehicle is currently outside the lane.

lane_deviation_event: Indicator for a lane deviation event.

occ_lane_deviation_event: Indicator for a lane deviation event occurring during occlusion.

vis_lane_deviation_event: Indicator for a lane deviation event occurring during visual sampling/attention.

total_lane_deviation_event_total: Cumulative total number of lane deviation events.

occ_lane_deviation_event_total: Cumulative number of lane deviation events during occlusion.

vis_lane_deviation_event_total: Cumulative number of lane deviation events during visual sampling/attention.

Event/log reconstruction variables:

x: Vehicle x-coordinate in the simulator/log data.

y: Vehicle y-coordinate in the simulator/log data.

yaw: Vehicle heading/yaw angle.

steer: Steering value at the logged time point or event.

report: Report or event marker variable from the processed driving log.

Derived occlusion-start/end variables:

FADE1.leftTLC: Left TLC at the beginning of occlusion.

FADE1.rightTLC: Right TLC at the beginning of occlusion.

FADE1.off: Offset at the beginning of occlusion.

FADE1.off.abs: Absolute offset at the beginning of occlusion.

FADE1.speed: Speed at the beginning of occlusion.

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

Model training and simulation output variables / labels:

EP: Training episode number.

R: Undiscounted episode reward.

Disc.R: Discounted episode reward.

AVG_TLC: Average time-to-line-crossing during the episode.

AVG_SPEED: Average speed during the episode.

ATT(lane/speed/none): Attention allocation ratios for lane, speed, and none during training.

AVG_NONE: Average duration of none/occluded attention periods.

DUR: Episode duration.

PHASE: Training phase label.

DONE: Episode termination reason, for example completion.

v: Vehicle speed in simulation console output.

l.exc_o: Lane excursions during occlusion in simulation console output.

l.exc_all: Total lane excursions in simulation console output.

s.exc_o: Speed deviations during occlusion in simulation console output.

s.exc_all: Total speed deviations in simulation console output.

tlc: Time-to-line-crossing in simulation console output.

r: Per-step reward in simulation console output.

a: Model action vector in simulation console output; includes speed/acceleration, steering, and attention-action components depending on the simulation configuration.

head: Vehicle heading in simulation console output.

pos: Vehicle position in simulation console output.

elev: Road elevation in hilly-road simulation output.

att: Attention state in simulation output. Expected values include lane, speed, and none.

Total reward: Total reward accumulated during a simulation episode.

Total time: Total duration of a simulation episode.

Done reason: Reason why the simulation episode ended, for example completion.

AoI Ratios: Model attention allocation ratios for Speed, Lane, and None.

lane_sampling_events N: Number of lane sampling events during simulation.

AVG_TLC_at_lane_sample: Average true TLC at lane sampling events.

lane_devs(total): Total number of lane deviations during simulation.

speed_devs(total): Total number of speed deviations during simulation.

occlusions(none) N: Number of none/occlusion periods during simulation.

occlusions(none) AVG_DUR: Average duration of none/occlusion periods during simulation.

- Missing data codes: space/NaN
