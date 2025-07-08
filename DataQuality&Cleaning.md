# Data Quality & Cleaning

## Data Quality
- The degree to which data is fit for its intended use

- **Validity** Invalid data e.g. 45/03/205
- **Accuracy** Reflects the true value or a standard e.g. 30/04/1699
- **Completeness** Missing data information
- **Consistency** Contracditing information
- **Uniformity** Consistent format e.g. measurement system
- **Redundacny** Information of the same observation is held within the same data e.g. duplicates, multiple input

## Data Cleaning
- Organising and sorting data to achieve good data quality

- **Irrelevant Data** Data that is not needed or doesnt fit under the context of the problem
- **Duplicates** Data points that are repeated
- **Type Conversions** Numbers stored as numerical types, date stored as data object e.g. 5ft4 to 163cm
- **Padding** Strings and numbers can be padded with extra characters or digits to ensure they are a certian width e.g. ID_Numbers
- **Typos** Easy

---

- **Standardisation** Put each value in the same format, so that data is uniform e.g. strings, ints
- **Scailing** Scailing data values to a specfiic range
- **Normalisation** Type of scailing, re-scales the data values into a range between 0-1

---

### Missing Values

- **Drop** If most of the value are missing for the coloumn then drop (Have a criteria to go by to decide if to drop)
- **Impute** Calculate missing values based on other observations (Mean, Median)
- **Hot-Deck** Copying values from other similar records (Random, Sequential)
- **Flagging** Saying that data is missing is informative itself so the algorithim knows (Missing data can be flagged)