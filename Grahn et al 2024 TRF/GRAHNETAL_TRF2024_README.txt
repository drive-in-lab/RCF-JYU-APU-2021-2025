This README file was generated on 2026-05-28 by Tuomo Kujala

Dataset README for:
Grahn, H., Kujala, T., Hautaoja, T., & Salvucci, D. D. (2024). Investigating the situational dynamics of visual information sampling in lateral vehicle control: Subjective vs. objective estimates of spare visual capacity. Transportation Research Part F: Traffic Psychology and Behaviour, 107, 98–114. https://doi.org/10.1016/j.trf.2024.08.034


GENERAL INFORMATION

Title of dataset:
Data associated with “Investigating the situational dynamics of visual information sampling in lateral vehicle control: Subjective vs. objective estimates of spare visual capacity”

Principal Investigator Information
Name: Tuomo Kujala
ORCID: 0000-0001-8222-8540
Institution: University of Jyväskylä
Address: Seminaarinkatu 15, PO Box 35, 40014 University of Jyväskylä
Email: tuomo.kujala@jyu.fi

Corresponding author of the publication
Name: Hilkka Grahn
Institution: University of Jyväskylä, Faculty of Information Technology
Email: hilkka.grahn@jyu.fi

Authors of the publication:
Hilkka Grahn, Tuomo Kujala, Toni Hautaoja, and Dario D. Salvucci

- Date of data collection: 2021
- Geographic location of data collection: University of Jyväskylä driving simulator laboratory, Jyväskylä, Finland.
- Information about funding sources that supported the collection of the data: This research was funded by the Academy of Finland / Research Council of Finland [Appropriate Uncertainty in Manual and Automated Driving, grant 343259].


SHARING/ACCESS INFORMATION

- Licenses/restrictions placed on the data: CC BY-NC.
- Links to publications that cite or use the data: https://doi.org/10.1016/j.trf.2024.08.034
- Recommended citation for this dataset:
  Grahn, H., Kujala, T., Hautaoja, T., & Salvucci, D. D. (2024). Investigating the situational dynamics of visual information sampling in lateral vehicle control: Subjective vs. objective estimates of spare visual capacity. Transportation Research Part F: Traffic Psychology and Behaviour, 107, 98–114.


DATA & FILE OVERVIEW

File List:
demographics.csv
SO.csv
MO.csv

METHODOLOGICAL INFORMATION

Description of methods used for collection/generation of data:
Grahn, H., Kujala, T., Hautaoja, T., & Salvucci, D. D. (2024). Investigating the situational dynamics of visual information sampling in lateral vehicle control: Subjective vs. objective estimates of spare visual capacity. Transportation Research Part F: Traffic Psychology and Behaviour, 107, 98–114.

Methods for processing the data:
Grahn, H., Kujala, T., Hautaoja, T., & Salvucci, D. D. (2024). Investigating the situational dynamics of visual information sampling in lateral vehicle control: Subjective vs. objective estimates of spare visual capacity. Transportation Research Part F: Traffic Psychology and Behaviour, 107, 98–114.


DATA-SPECIFIC INFORMATION FOR: demographics.csv

- Number of variables: 5
- Number of cases/rows: 32
- Variable List: ID (participant ID), age (age), gender (values: 1 = male, 2 = female), driving.experience.years (driving experience in years), km.per.year (self-estimated kilometers per year), lifetime.km (self-estimated lifetime kilometers)
- Missing data codes: space

DATA-SPECIFIC INFORMATION FOR: SO.csv

- Number of variables: 10
- Number of cases/rows: 1500
- Variable List: id (participant id), off (offset when occlusion ended), OT (occlusion time), TLC (time-to-line crossing), FADE1.TLC.min (shortest TLC when occlusion started right/left), last_OT (previous occlusion’s occlusion time), last_FADE0.off.abs (offset at the end of previous occlusion), steer.ampl (steering amplitude), true.TLC.1.0 (lane crossings, values 0 = no crossing, 1 = crossing), offset.sd.avg.100.so (average standard deviation of the offset)
- Missing data codes: space

DATA-SPECIFIC INFORMATION FOR: MO.csv

- Number of variables: 14
- Number of cases/rows: 3575
- Variable List: id (participant id), drive (values: MO_60 = drive with 60 km/h, MO_100 = drive with 100 km/h), speed.kmh (speed kilometers per hour), occ_nr (occlusion’s number), off (offset when occlusion ended), OT (occlusion time), TLC (time-to-line crossing), FADE1.TLC.min (shortest TLC when occlusion started right/left), last_OT (previous occlusion’s occlusion time), last_FADE0.off.abs (offset at the end of previous occlusion), steer.ampl (steering amplitude), true.TLC.1.0 (lane crossings, values 0 = no crossing, 1 = crossing), offset.sd.avg.100.so (average standard deviation of the offset), ratio_OT_TLC (ratios of OTs and TLCs)
- Missing data codes: space