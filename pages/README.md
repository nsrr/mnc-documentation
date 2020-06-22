# About

The Mignot Nature Communications (MNC) dataset contains raw polysomnography data from an automated sleep staging project using neural networks. The [piece was published in Nature Communications](https://pubmed.ncbi.nlm.nih.gov/30523329/) and the abstract is below.

> Analysis of sleep for the diagnosis of sleep disorders such as Type-1 Narcolepsy (T1N) currently requires visual inspection of polysomnography records by trained scoring technicians. Here, we used neural networks in approximately 3,000 normal and abnormal sleep recordings to automate sleep stage scoring, producing a hypnodensity graph—a probability distribution conveying more information than classical hypnograms. Accuracy of sleep stage scoring was validated in 70 subjects assessed by six scorers. The best model performed better than any individual scorer (87% versus consensus). It also reliably scores sleep down to 5 s instead of 30 s scoring epochs. A T1N marker based on unusual sleep stage overlaps achieved a specificity of 96% and a sensitivity of 91%, validated in independent datasets. Addition of HLA-DQB1*06:02 typing increased specificity to 99%. Our method can reduce time spent in sleep clinics and automates T1N diagnosis. It also opens the possibility of diagnosing T1N using home sleep studies.

The National Sleep Research Resource is grateful to Emmanual Mignot for sharing these data.

## Citation and acknowledgement

When using this dataset, please cite the following:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
>
> [Stephansen JB, Olesen AN, Olsen M, Ambati A, Leary EB, Moore HE, Carrillo O, Lin L, Han F, Yan H, Sun YL, Dauvilliers Y, Scholz S, Barateau L, Hogl B, Stefani A, Hong SC, Kim TW, Pizza F, Plazzi G, Vandi S, Antelmi E, Perrin D, Kuna ST, Schweitzer PK, Kushida C, Peppard PE, Sorensen HBD, Jennum P, Mignot E. Neural network analysis of sleep stages enables efficient diagnosis of narcolepsy. Nat Commun. 2018 Dec 6;9(1):5229. doi: 10.1038/s41467-018-07229-3. PMID: 30523329; PMCID: PMC6283836.](https://pubmed.ncbi.nlm.nih.gov/30523329/)

Please include the following text in the Acknowledgements:

> The Mignot Nature Communications research was mostly supported by a grant from Jazz Pharmaceuticals to E.M. Additional funding came from: NIH grant R01HL62252 (to P.E.P.); Ministry of Science and Technology 2015CB856405 and National Foundation of Science of China 81420108002,81670087 (to F.H.); H. Lundbeck A/S, Lundbeck Foundation, Technical University of Denmark and Center for Healthy Aging, University of Copenhagen (to P.J. and H.B.D.S). Additional support was provided by the Klarman Family, Otto Mønsted, Stibo, Vera & Carl Johan Michaelsens, Knud Højgaards, Reinholdt W. Jorck and Hustrus and Augustinus Foundations (to A.N.O.). The National Sleep Research Resource was supported by the National Heart, Lung, and Blood Institute (R24 HL114473, RFP 75N92019R002).

## Polysomnography data

The NSRR team harmonized the [publicly available EDF and staging data](https://stanfordmedicine.app.box.com/s/r9e92ygq0erf7hn5re6j51aaggf50jly) using the [Luna software package](http://zzz.bwh.harvard.edu/luna/) to make future analyses simpler. The [montage and sampling rate information page](:pages_path:/montage-and-sampling-rate-information.md) details the harmonized EDF channel labels. We converted manual sleep staging data into two different formats: .eannot and .xml. Some cohorts did not include manual sleep staging data.

The .eannot files contain rows corresponding to 30-second epochs. Coding information is as follows:

- CNC/SSC staging: 0 Wake; 1 N1; 2 N2; 3 N3; 4 N4; 5 REM; 7 Unknown
- DHC staging: 1 Wake; 0 REM; -1 N1; -2 N2; -3 N3

The .xml staging files adhere to [the NSRR XML annotation format](https://github.com/nsrr/edf-editor-translator/wiki/Physiomimi-Format) used across many datasets.

To access the NSRR harmonized versions of the MNC data, [complete a new data request](https://staging.partners.org/sleepdata.org/data/requests/mnc/start). Once the NSRR team approves your access, [click here to browse and download files](:files_path:).

## Subject data (cohorts_deid.xlsx)

The [**cohorts_deid.xlsx** file](:files_path:) was presented with the manuscript for matching case and control subjects from the various cohorts.  It matches individual subject IDs with their corresponding cohort, a narcolepsy or control diagnosis, and which part or parts of the analysis their sleep study was used for (e.g. training, testing, validation).

CSF refers to cerebrospinal fluid, and if there is a numeric value it would be in reference to how much hypocretin was found there.  It is used as a final indicator for narcolepsy.

DB0602 is in reference to the allele HLA-DQB1*06:02; which is relatively common in the general population, and extremely common among those diagnosed as narcoleptic. In other words, most people who are DQB0602 positive do not have narcolepsy, while almost all people with narcolepsy are DQB0602 positive.

## Related links

- [Stanford STAGES automated sleep scoring software (github.com)](https://github.com/stanford-stages/stanford-stages)
- [Anonymized data on public Box share](https://stanfordmedicine.app.box.com/s/r9e92ygq0erf7hn5re6j51aaggf50jly)

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
