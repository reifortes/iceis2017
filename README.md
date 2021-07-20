
# Fortes et al. (ICEIS'2017)

Dataset used in **Fortes et al.**, *A Multicriteria Evaluation of Hybrid Recommender Systems: On the usefulness of Input Data Characteristics*. In Proceedings of the 19th International Conference on Enterprise Information Systems - Volume 2: ICEIS, ISBN 978-989-758-248-6, pages 623-633. DOI: 10.5220/0006315406230633. Porto, Portugal. April, 2017.

Datasets contain data processed from the original datasets, freely available on the Internet, as described in the article. Use licenses must follow the original data licenses.

# File structure


The files are structured into three individually compressed folders:

-   **data**: contains the ratings and attributes of users and items:
    -   _Sample*.txt_: files composed of one or more folds used as input for _training_ / _validation_ / _testing_, numbers indicate the folds used in the composition of the files.
    -   _TuningSample*.txt_: contains the extracted samples for tuning the individual algorithms.
    -   _u.item.attributes_: contains attributes of items processed from its content to be used in MyMediaLite content-aware algorithms.
    -   _u.user.attributes_: contains user attributes processed from its content to be used in MyMediaLite content-aware algorithms (only for ML1M, generated from the original database).
    -   Folds composition: file ***[folds.xls](folds.xlsx)***
-   **meta-features**: contains the computed _meta-features_ for each fold:
    -   The values are normalized.
    -   Negative values characterize _missing values_, which are treated as ZERO in the composition of features.
    -   Separate files for users' meta-features and items' meta-features.
-   **features**: contains the features calculated for the hybrid methods (HR, FWLS and STREAM) for all experimental scenarios (S1, S2, and S3) that serve as input to the Scikit-learn.
    -   Folds _F[12345]_: training files for each fold.
    -   Folds _F[12345]-T_: testing files for each fold.
    -   Fold _Tuning_: files used for tuning composed of the individual algorithms tuning files.
    -   Fold _keys_: contains the user / item keys related to each line.

# Downloadable Files

-   **Bookcrossing dataset**
    -   [data](https://drive.google.com/file/d/12UualNof3f6bwreAJNFLQdpJzVk0U0Zp/view?usp=sharing).
    -   [meta-features](https://drive.google.com/file/d/1CtJPpZ1Fmg_aj30SCugwFDp4FHxuRerX/view?usp=sharing).
    -   [features](https://drive.google.com/file/d/1J1cPVzu0C6JflIE9ROC84YpMd5no9rws/view?usp=sharing).
-   **Jester dataset**
    -   [data](https://drive.google.com/file/d/1SHycMtE6m8LxhWRmzWEIWAf5_nA5HPzG/view?usp=sharing).
    -   [meta-features](https://drive.google.com/file/d/188Op6KcgxI6kM3Un42ZKnalyAucGxXFp/view?usp=sharing).
    -   [features](https://drive.google.com/file/d/1rZ1sA3tkjSnaahy4MM-CAP2DNhb1RcKw/view?usp=sharing).
-   **Movielens (1M) dataset**
    -   [data](https://drive.google.com/file/d/1jJE-joIV-TX5kpiar9vo8SCaXFZ9JOyu/view?usp=sharing).
    -   [meta-features](https://drive.google.com/file/d/1ONlgf3zJ9NwVvIouLOU4VQT6VEfpDCb2/view?usp=sharing).
    -   [features](https://drive.google.com/file/d/1QR6tO4Kh-ltDC9DAn-SwudVDGiFwpuQj/view?usp=sharing).
