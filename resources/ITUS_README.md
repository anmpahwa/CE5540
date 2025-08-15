# Indian Time Use Survey - 2024

This sub-folder contains processed data from the 2024 Indian Time Use Survey conducted by the National Sample Survey Office (NSSO) under Ministry of Statistics and Programme Implementation (MoSPI), Government of India.

## Household Data

File: household.csv
Tag: Descriptive identification of sample households.
Columns:
- Unique_HH_ID: unique ids to identify each household(survey_year - fsu_serial_no - sector - nss_region - district - stratum - sub_stratum 
                                                      - sub_round - fod_sub_region - nsc - household_id)
- time_of_year: survey round
    - 1: jan - mar                                                                                              (q1)
    - 2: apr - jun                                                                                              (q2)
    - 3: jul - sep                                                                                              (q3)
    - 4: oct - dec                                                                                              (q4)
- day_of_week: survey day of the week
    - 1: monday                                                                                                 (weekday)
    - 2: tuesday                                                                                                (weekday)
    - 3: wednesday                                                                                              (weekday)
    - 4: thursday                                                                                               (weekday)
    - 5: friday                                                                                                 (weekday)
    - 6: saturday                                                                                               (weekend)
    - 7: sunday                                                                                                 (weekend)
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- region:
    - 1: north
    - 2: west
    - 3: central
    - 4: east
    - 5: north-east
    - 6: south
- distric_population: district population                                                                       (tier-I/II/III)
- gender_ratio: ratio of no. of female in the household to household size
- average_age: average age of household members
- marital_status: marital status of the household
    - 1: all are single                                                                                         (not_married)
    - 2: at least one individual is married                                                                     (married)
    - 3: others                                                                                                 (not_married)
- highest_edulevel: maximum education level in a household                                                      (not_literate/primary/secondary/graduate_&_above)
- employment_ratio: ratio of no of employed individuals in a household to household size
- family_structure: ratio of no. of individuals of age 18 and below in a household to household  size
- household_size: number of members of the household
- religion: household religion
    - 1: hinduism
    - 2: islam
    - 3: christianit
    - 4: sikhism
    - 5: jainism
    - 6: buddhism
    - 7: zoroastrianism
    - 9: others
- social_group
    - 1: scheduled tribe                                                                                        (disadvantaged)
    - 2: scheduled caste                                                                                        (disadvantaged)
    - 3: other backward class                                                                                   (disadvantaged)
    - 9: others                                                                                                 (not_disadvantaged)
- land_possessed
    - 99: 0.00 hectare                                                                                          (no_land)
    - 1: (0.00, 0.005) hectare                                                                                  (land_possessed)
    - 2: [0.005, 0.02) hectare                                                                                  (land_possessed)
    - 3: [0.02, 0.21) hectare                                                                                   (land_possessed)
    - 4: [0.21, 0.41) hectare                                                                                   (land_possessed)
    - 5: [0.41, 1.01) hectare                                                                                   (land_possessed)
    - 6: [1.01, 2.01) hectare                                                                                   (land_possessed)
    - 7: [2.01, 3.01) hectare                                                                                   (land_possessed)
    - 8: [3.01, 4.01) hectare                                                                                   (land_possessed)
    - 9: [4.01, 5.01) hectare                                                                                   (land_possessed)
    - 10: [5.01, 6.01) hectare                                                                                  (land_possessed)
    - 11: [6.01, 8.01) hectare                                                                                  (land_possessed)
    - 12: >= 8.01 hectare                                                                                       (land_possessed)
- total_expenditure: total monthly expenditure                                                                  (low/medium/high income
- dwelling_unit: type of dwelling unit
    - 1: owned
    - 2: hired
    - 3: no dwelling unit                                                                                       (no_dwelling)
    - 9: others
- dwelling_structure: type of the structure of the dwelling unit
    - 1: kutcha                                                                                                 (kutcha)
    - 2: semi pucca                                                                                             (pucca)
    - 3: pucca                                                                                                  (pucca)
- weight: survey weight assigned to the household
- shopping_choice: choice of shopping channel by the household
    - 0: no shopping
    - 1: in-store shopping
    - 2: online shopping
    - 3: both in-store and online shopping

#### Note
All missing data is represented by 9999.

---

## Individual Data

File: individual.csv
Tag: Demographic particulars of all the household members.
Columns:
- Unique_ID: unique ids to identify each household(survey_year - fsu_serial_no - sector - nss_region - district - stratum - sub_stratum 
                                                      - sub_round - fod_sub_region - nsc - household_id - individual_id)
- Unique_HH_ID: unique ids to identify each household(survey_year - fsu_serial_no - sector - nss_region - district - stratum - sub_stratum 
                                                      - sub_round - fod_sub_region - nsc - household_id)
- time_of_year: survey round
    - 1: jan - mar                                                                                              (q1)
    - 2: apr - jun                                                                                              (q2)
    - 3: jul - sep                                                                                              (q3)
    - 4: oct - dec                                                                                              (q4)
- day_of_week: survey day of the week
    - 1: monday                                                                                                 (weekday)
    - 2: tuesday                                                                                                (weekday)
    - 3: wednesday                                                                                              (weekday)
    - 4: thursday                                                                                               (weekday)
    - 5: friday                                                                                                 (weekday)
    - 6: saturday                                                                                               (weekend)
    - 7: sunday                                                                                                 (weekend)
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- region:
    - 1: north
    - 2: west
    - 3: central
    - 4: east
    - 5: north-east
    - 6: south
- distric_population: district population                                                                       (tier-I/II/III)
- gender: individual's gender
    - 1: male
    - 2: female
    - 3: transgender
- age: individual's age                                                                                         (gen_alpha/gen_z/millenials/gen_x/baby_boomers/silent)
- marital_status: individual's martial status
    - 1: never married                                                                                          (not_married)
    - 2: currently married                                                                                      (married)
    - 3: widowed                                                                                                (not_married)
    - 4: divorced/separated                                                                                     (not_married)
- education_level: individual's education level
    - 1: not literate                                                                                           (not_literate)
    - 2: literate: below primary                                                                                (primary)
    - 3: primary                                                                                                (primary)
    - 4: upper primary/middle                                                                                   (primary)
    - 5: secondary                                                                                              (secondary)
    - 6: higher secondary                                                                                       (secondary)
    - 7: diploma /certificate course (up to secondary)                                                          (secondary)
    - 8: diploma/certificate course (higher secondary)                                                          (secondary)
    - 9: diploma/certificate course(graduation & above)                                                         (graduation_&_above)
    - 10: graduate                                                                                              (graduation_&_above)
    - 11: post graduate and above                                                                               (graduation_&_above)
- employment_status: individual's employment status
    - 11: working as own account worker in household enterprise                                                 (employed)
    - 12: working as employer in household enterprise                                                           (employed)
    - 21: working as helper in household enterprise (unpaid family worker)                                      (employed)
    - 31: working as regular salaried/wage employee                                                             (employed)
    - 41: working as casual wage labour in public works                                                         (employed)
    - 51: working as casual wage labour in other types of work                                                  (employed)
    - 81: did not work but was seeking and/or available for work                                                (unemployed)
    - 91: attending educational institution                                                                     (nilf)
    - 92: attending domestic duties only                                                                        (nilf)
    - 93: attending domestic duties and is also engaged in unpaid household enterprise for household use        (nilf)
    - 94: rentiers, pensioners, remittance recipients, etc.                                                     (nilf)
    - 95: not able to work due to disability                                                                    (nilf)
    - 97: others (including begging, prostitution, etc.)                                                        (nilf)
- family_structure: ratio of no. of individuals of age 18 and below in a household to household  size 
- household_size: number of members of the household
- religion: household religion
    - 1: hinduism
    - 2: islam
    - 3: christianit
    - 4: sikhism
    - 5: jainism
    - 6: buddhism
    - 7: zoroastrianism
    - 9: others
- social_group
    - 1: scheduled tribe                                                                                        (disadvantaged)
    - 2: scheduled caste                                                                                        (disadvantaged)
    - 3: other backward class                                                                                   (disadvantaged)
    - 9: others                                                                                                 (not_disadvantaged)
- land_possessed
    - 99: 0.00 hectare                                                                                          (no_land)
    - 1: (0.00, 0.005) hectare                                                                                  (land_possessed)
    - 2: [0.005, 0.02) hectare                                                                                  (land_possessed)
    - 3: [0.02, 0.21) hectare                                                                                   (land_possessed)
    - 4: [0.21, 0.41) hectare                                                                                   (land_possessed)
    - 5: [0.41, 1.01) hectare                                                                                   (land_possessed)
    - 6: [1.01, 2.01) hectare                                                                                   (land_possessed)
    - 7: [2.01, 3.01) hectare                                                                                   (land_possessed)
    - 8: [3.01, 4.01) hectare                                                                                   (land_possessed)
    - 9: [4.01, 5.01) hectare                                                                                   (land_possessed)
    - 10: [5.01, 6.01) hectare                                                                                  (land_possessed)
    - 11: [6.01, 8.01) hectare                                                                                  (land_possessed)
    - 12: >= 8.01 hectare                                                                                       (land_possessed)
- total_expenditure: total monthly expenditure                                                                  (low/medium/high income
- dwelling_unit: type of dwelling unit
    - 1: owned
    - 2: hired
    - 3: no dwelling unit                                                                                       (no_dwelling)
    - 9: others
- dwelling_structure: type of the structure of the dwelling unit
    - 1: kutcha                                                                                                 (kutcha)
    - 2: semi pucca                                                                                             (pucca)
    - 3: pucca                                                                                                  (pucca)
- weight: survey weight assigned to the individual
- shopping_choice: choice of shopping channel by the household
    - 0: no shopping
    - 1: in-store shopping
    - 2: online shopping
    - 3: both in-store and online shopping

#### Note
All missing data is represented by 9999.

---