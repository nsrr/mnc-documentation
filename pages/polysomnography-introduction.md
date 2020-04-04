# Polysomnography introduction

Home sleep testing was performed using the Embletta-Gold device (Embla, Broomfield, CO) and was self-administered by the participant following nuMoM2b parent study visits 1 and 3. The pocket-sized device contains four recommended and validated sensors for measuring SDB parameters: a nasal pressure transducer (measuring nasal airflow and waveform, needed for detecting apneas and hypopneas and airflow limitation); thoracic and abdominal inductance plethysmography bands (XactTrace belts; measuring respiratory effort for distinguishing central from obstructive apneas and as a back-up for the nasal pressure signal); and finger pulse oximetry (to quantify level and duration of oxygen desaturation). In addition, bipolar ECG and body position were recorded.

Each unit used for collection was certified before use to maximize signal quality integrity throughout the EDF conversion and import into Compumedics Profusion software used for scoring.

Notes:

- [Montage and Sampling Rate Information](:pages_path:/montage-and-sampling-rate-information.md)
- [Sleep Breathing Substudy Manual of Operations](:files_path:/documentation/nuMoM2b-SBS-MOO.pdf)

## Signal and annotation files

[Raw polysomnography data](:files_path:/polysomnography) are available for 3,009 subjects at Visit 1 and 2,332 subjects at Visit 3. Each recording has a signal file (.EDF) and event scoring annotations (.XML).

1. **[EDF](:files_path:/polysomnography/edfs)** - Signal files in the [European Data Format](http://www.edfplus.info/) exported from Compumedics Profusion and processed in [Luna](http://zzz.bwh.harvard.edu/luna/)
2. **[XML (Profusion)](:files_path:/polysomnography/annotations-events-profusion)** - Annotation files exported from Compumedics Profusion. ([Learn more...](https://github.com/nsrr/edf-editor-translator/wiki/Compumedics-Annotation-Format))

## Known issues

- Raw and scoring data are not available for three (3) subjects present in the [Visit 1 dataset](:pages_path:/dataset-introduction.md) due to data loss.

## History / changelog

*April 2020*
- Data uploaded to sleepdata.org after exports from Compumedics Profusion

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
