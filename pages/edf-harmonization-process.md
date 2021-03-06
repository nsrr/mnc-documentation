# EDF Harmonization Process

### Signal harmonization

- Using Luna, a list of all channel names were extracted from the EDFs for the Mignot Nature Communication cohorts. Subsequently, the channel names in EDF files were changed to a new set of standardized channel names listed on the [montage page] (:pages_path:/montage-and-sampling-rate-information.md) under "EDF Label".
- The DHC cohort provided recordings in .mat format, these were converted to EDF
- A few EDFs contained additional EEG channels Fz_M1, Fz_M2, and M1_M2, these were removed.
- Polarity checks were performed via Luna. EEG traces in the DHC cohort were flipped to correct polarity, with upwards deflections indicating negative polarity.
- Several EEG channels were recorded in mV, they were changed to uV.
- Finally, canonical channels cs_EEG, cs_EMG, and cs_EEG were generated at a sample rate of 100Hz and added to each EDF. The table below lists the channels used as input by Luna.

| TYPE | CHANNEL  | REF       | SAMPLING RATE  | NOTES            |
|------|----------|-----------|----------------|------------------|
| EEG  | C4       | M1        | 100            |                  |
| EEG  | C4       | .         | 100            |                  |
| EMG  | rchin    | lchin     | 100            |                  |
| EMG  | chin     | .         | 100            | Using linked EMG |
| EMG  | cchin_l  | .         | 100            | Using linked EMG |
| ECG  | ECG1     | ECG2,ECG3 | 100            |                  |
| ECG  | ECG,ECG2 | .         | 100            |                  |
| ECG  | ECG1_2   | .         | 100            | Using linked ECG |

### Annotation harmonization

- 3 cohorts provided scoring annotations: SSC, CNC, and DHC.
- SSC and CNC annotations were converted from .sta format to Luna's .eannot format
- DHC annotations were converted from .mat format to Luna's .eannot format
- .eannot files were then harmonized. Stage N4 was changed to N3. All .eannot files now have the following staging encoding: wake, N1, N2, N3, REM, unscored
