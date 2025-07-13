# Indian Time Use Survey - 2024

This sub-folder contains processed data from the 2024 Indian Time Use Survey conducted by the National Sample Survey Office (NSSO) under Ministry of Statistics and Programme Implementation (MoSPI), Government of India.

## Household Data

File: household.csv
Tag: Descriptive identification of sample households.
Columns:
- Unique_HH_ID: unique ids to identify each household(survey_year - fsu_serial_no - sector - nss_region - district - stratum - sub_stratum 
                                                      - sub_round - fod_sub_region - nsc - household_id)
- day_of_week: survey day of the week
    - 1: monday
    - 2: tuesday
    - 3: wednesday
    - 4: thursday
    - 5: friday
    - 6: saturday
    - 7: sunday
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- district_population: district population
- gender ratio: ratio of no. of female in the household to household size
- average_age: average age of household members
- marital_status: marital status of the household
    - 1: all are single
    - 2: if at least one individual is married
    - 3: others
- highest_edulevel: maximum education level in a household
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
    - 1: scheduled tribe
    - 2: scheduled caste
    - 3: other backward class
    - 9: others
- land_possessed
    - 99: 0.00 hectare
    - 1: (0.00, 0.005) hectare
    - 2: [0.005, 0.02) hectare
    - 3: [0.02, 0.21) hectare
    - 4: [0.21, 0.41) hectare
    - 5: [0.41, 1.01) hectare
    - 6: [1.01, 2.01) hectare
    - 7: [2.01, 3.01) hectare
    - 8: [3.01, 4.01) hectare
    - 9: [4.01, 5.01) hectare
    - 10: [5.01, 6.01) hectare
    - 11: [6.01, 8.01) hectare
    - 12: >= 8.01 hectare 
- total_expenditure: total monthly expenditure
- dwelling_structure: type of the structure of the dwelling unit
    - 1: kutcha
    - 2: semi pucca
    - 3: pucca
    - 9: no dwelling
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
- day_of_week: survey day of the week
    - 1: monday
    - 2: tuesday
    - 3: wednesday
    - 4: thursday
    - 5: friday
    - 6: saturday
    - 7: sunday
- sector: whether fsu falls within rural or urban
    - 1: rural
    - 2: urban
- district_population: district population
- gender: individual's gender
    - 1: male
    - 2: female
    - 3: transgender
- age: individual's age
- marital_status: individual's martial status
    - 1: never married
    - 2: currently married
    - 3: widowed
    - 4: divorced/separated
- education_level: individual's education level
    - 1: not literate
    - 2: literate: below primary
    - 3: primary
    - 4: upper primary/middle
    - 5: secondary
    - 6: higher secondary
    - 7: diploma /certificate course (up to secondary)
    - 8: diploma/certificate course (higher secondary)
    - 9: diploma/certificate course (graduation & above)
    - 10: graduate
    - 11: post graduate and above
- employment_status: individual's employment status
    - 11: working as own account worker in household enterprise
    - 12: working as employer in household enterprise
    - 21: working as helper in household enterprise (unpaid family worker)
    - 31: working as regular salaried/wage employee
    - 41: working as casual wage labour in public works
    - 51: working as casual wage labour in other types of work
    - 81: did not work but was seeking and/or available for work
    - 91: attending educational institution
    - 92: attending domestic duties only
    - 93: attending domestic duties and is also engaged in unpaid household enterprise for household use
    - 94: rentiers, pensioners, remittance recipients, etc.
    - 95: not able to work due to disability
    - 97: others (including begging, prostitution, etc.)
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
    - 1: scheduled tribe
    - 2: scheduled caste
    - 3: other backward class
    - 9: others
- land_possessed
    - 99: 0.00 hectare
    - 1: (0.00, 0.005) hectare
    - 2: [0.005, 0.02) hectare
    - 3: [0.02, 0.21) hectare
    - 4: [0.21, 0.41) hectare
    - 5: [0.41, 1.01) hectare
    - 6: [1.01, 2.01) hectare
    - 7: [2.01, 3.01) hectare
    - 8: [3.01, 4.01) hectare
    - 9: [4.01, 5.01) hectare
    - 10: [5.01, 6.01) hectare
    - 11: [6.01, 8.01) hectare
    - 12: >= 8.01 hectare 
- total_expenditure: total monthly expenditure
- dwelling_structure: type of the structure of the dwelling unit
    - 1: kutcha
    - 2: semi pucca
    - 3: pucca
    - 9: no dwelling
- weight: survey weight assigned to the individual
- shopping_choice: choice of shopping channel by the household
    - 0: no shopping
    - 1: in-store shopping
    - 2: online shopping
    - 3: both in-store and online shopping

#### Note
All missing data is represented by 9999.

---