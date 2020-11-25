# Medical Image Datasets

The accuracy of a particular deep learning model is directly proportional to amount of data with which it is trained. However, acquiring medical imagesets can be particularly challenging and costly due to privacy measures and the time cost of annotating images.

Here, you can find a list medical image repositories sorted by imaging modality with which to use as in model training. Keep in mind that datasets may vary by annotation, location and pre-processing.

Make sure to thoroughly read any documentation available for each dataset.

**Important note: Many datasets must be opened with the [NBIA Data Retriever](https://wiki.cancerimagingarchive.net/display/NBIA/Downloading+TCIA+Images) with the dataset's respective TCIA or DICOM file.**

## Ultrasound Sonography

| Title | Description | Keywords | Source | Size |
| ----- | ----------- | -------- | ------ | ---- |
|       |             |          |        |      |

## X-Ray Radiography

| Title                                                        | Description                                                  | Keywords     | Source                                      | Size                    |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------ | ------------------------------------------- | ----------------------- |
| NIH Chest X-ray Dataset of 14 Common Thorax Disease Categories | <br /> Dataset composed of over 110000 frontal-view X-ray images of 30805 unique patients. Images are labelled using natural language processing algorithms and are expected to have accuracy of >90%.<br />You can use the batch_download_zips.py file in their repository to automate the download process.<br /> Labels used are listed below:<br />1. Atelectasis <br />2. Cardiomegaly <br />3. Effusion<br />4. Infiltration<br />5. Mass<br />6. Nodule<br />7. Pneumonia<br />8. Pneumothorax<br />9. Consolidation<br />10. Edema<br />11. Emphysema<br />12. Fibrosis<br />13. Pleural_Thickening<br />14. Hernia<br />Find more information [[HERE]](https://arxiv.org/abs/1705.02315) | X-Ray, chest | https://nihcc.app.box.com/v/ChestXray-NIHCC | 112120 images (45.6 GB) |

## MRI

| Title | Description                                                  | Keywords       | Source                                       | Size                   |
| ----- | ------------------------------------------------------------ | -------------- | -------------------------------------------- | ---------------------- |
| ISPY1 | Created to test MRI (utilizing tissue-based biomarkers) for ability to predict responce to treatment and risk-f-recurrence in patients with stage 2 or stage 3 breast cancer receiving neoadjuvant chemotherapy. Images and segmentations are available in addition to clinical and outcome data. | breast, cancer | http://doi.org/10.7937/K9/TCIA.2016.HdHpgJLK | 386528 images, 76.2 GB |

## PET/CT

| Title                                                       | Description                                                  | Keywords             | Source                                                       | Size                     |
| ----------------------------------------------------------- | ------------------------------------------------------------ | -------------------- | ------------------------------------------------------------ | ------------------------ |
| QIN-HeadNeck                                                | Contains multiple PET scans of 279 cancer patients before and after therapy. Follow up scans are also avilable where clinically required. Clinical data also provided as an XLSX file. | head, neck, cancer   | https://doi.org/10.7937/K9/TCIA.2015.K0F5CGLI                | 701002 images, 201.2 GB  |
| NSCLC-Radiomics                                             | Collection contains manually delineated pretreatment CT scans of 422 non-small cell lung cancer (NSCLC) patients. The delineation of 3D volume of the gross tumour volumes is provided in addition to clinic data from each patient in a CSV file. | lung, cancer         | https://doi.org/10.7937/K9/TCIA.2015.PF0M9REI                | 52073 images, 33 GB      |
| National Lung Screening Trial [LIMITED ACCESS]              | Dataset created during the NLST clinical trial of screening tests for lung cancer. Using data generated from approximately 54000 participants between August 2002 and April 2004. The study was designed to determine whether low-dose CT screening reduces lung cancer mortality rates relative to chest radiogaphy (x-ray). Clinical and outcome data is available. [Access to this dataset is limited and must be requested](https://biometry.nci.nih.gov/cdas/studies/nlst). After being granted, data can be downloaded using the TCIA Query Tool for NLST. | lung, cancer         | https://wiki.cancerimagingarchive.net/display/NLST/National+Lung+Screening+Trial#5800702d1a85fbd42314c9eb5cdaef39d568cb8 | 42165004 images, 11.3 TB |
| CT Images in COVID-19                                       | Unenhanced CT images from 632 patients with COVID-19 infections confirmed with RT-PCR to have presences of SARS-CoV-2 obtained within one day of their initial CT. | COVID-19, SARS-CoV-2 | https://www.nature.com/articles/s41467-020-17971-2#data-availability | 11.8 GB                  |
| Lung Image Database Consortium Image Colleciton (LIDC-IDRI) | Consisting of diagnostic and lung cancer screening thoracic CT scans with marked-up annotated lesions designed for development, training and evaluation of computer-assisted diagnosis. Contains data from 1018 cases with lesions classified into three categories.<br />1. nodule >= 3 mm<br />2. nodule < 3 mm<br />3. non-nodule >= 3mm | lung, cancer         | https://wiki.cancerimagingarchive.net/display/Public/LIDC-IDRI | 125 GB                   |

## Other

| Title                                                        | Description                                                  | Keywords                                   | Source                                            | Size                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------ | ------------------------------------------------- | ------------------------------------------------------------ |
| Chest Imaging with Clinical and Genomic Coorelates Representing a Rural COVID-19 Positive Population | A collection of x-ray and CT images from patients who test positive for COVID-19 which focuses on rural and underrespresented populations. Clinical data for each patient is also present as a CSV file in addition to two associated Genbank repositories. | X-ray, CT, COVID-19, SARS-CoV-2            | https://www.doi.org/10.7937/tcia.2020.py71-5978   | 31935 images, 19.0 GB                                        |
| Cancer Imaging Archive                                       | The Cancer Imaging Archive maintains a repository hosting over 125 of small-to-mid sized imagesets from various imaging modalities focusing on a variety of imaging locations and cancer types. Because many of these datasets contain images numbering in the hundreds to low thousands, **data augmentation may be necessary for your application**. Additionally, some datasets may be labelled but not segmented. Manual segmentation may be necessary to produce the proper training sets required for your application.<br />Data is sometimes designated as **limited acces** and requires additional permissions to obtain. | cancer, MRI, CT, PET, ultrasound, mamogram | https://www.cancerimagingarchive.net/collections/ | ranges from tens to hundreds-of-thousands of images, 100s of MB to multiple TB |

## Other Useful Links

| Title | Description |
| ----- | ----------- |
|       |             |









