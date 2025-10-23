## Data Summary
The City of Charlottesville Parking Tickets dataset is a public collection of 506,311  official records detailing parking violations issued by the city's Parking Division. The dataset spans over two decades, running from 1999 up to the present day, and includes key features like the date and time the ticket was issued, the street name where the ticket was issued, and a description of the violation (e.g., "Overtime Parking," "No Parking"). There are also columns that track the administrative process (status of appeals and waivers). This data is openly hosted on the Charlottesville Open Data Portal at https://opendata.charlottesville.org/datasets/0ae373f4c2884abbb296500125bb9d8a_7/explore, where it can be directly previewed, filtered, and downloaded in various formats. It provides researchers with a rich source for urban studies, policy evaluation, and time-series analysis of enforcement patterns.

## Provenance
The Charlottesville Parking Tickets dataset is an authoritative public resource sourced directly from the operational records of the City of Charlottesville's Parking Division, and distributed through its Open Data portal. It comprises 506,311 entries, each representing an official, timestamped record generated during the municipal enforcement process. The data documents parking violations issued within the city from 1999 up to the present, including key details such as the violation type, time of issuance, location, and administrative statuses for waivers and appeals. Its origin ensures that every data point is grounded in real-world enforcement activity, making it a valuable resource for studying urban mobility, public policy, and administrative processes.

## License
This parking ticket data uses a Creative Commons Attribution license. This is a very open license, letting you share and adapt the data for any purpose, including commercially. The only mandatory term is that you must clearly credit the City of Charlottesville, link to the license, and note any changes you make. You cannot impose any new restrictions on others using the data. (https://creativecommons.org/licenses/by/4.0/)

## Ethical Statements
The Charlottesville Parking Tickets dataset is a highly objective resource derived directly from enforcement records, which limits the scope of ethical concerns compared to behavioral or demographic datasets. The primary consideration revolves around privacy and re-identification risk. While license plates are anonymized, the combination of geographic and temporal data could potentially be linked with external public records. This combination raises a concern about the potential for surveillance or tracking of frequent offenders. Researchers must be careful not to facilitate re-identification and should utilize the data strictly to analyze policy effectiveness.

## Data Dictionary
| Column              | Description                                                                 | Potential Responses                                                                                   |
|----------------------|------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------|
| RecordID             | A unique identifier for each row                                            | 1, 2, 999                                                                                              |
| TicketNumber         | The official parking ticket number assigned                                 | "59212", "10517"                                                                                       |
| DateIssued           | The date and time when the ticket was issued                                | "2015/10/30 04:00:00+00", "2021/03/15 13:13:08+00"                                                     |
| StreetName           | The name of the street where the ticket was given                           | "W WATER ST", "400 1ST ST N"                                                                           |
| TimeIssued           | The specific time of day (HH:MM) the ticket was issued                      | "9:58", "15:14"                                                                                        |
| StreetNumber         | The street address number where the violation occurred                      | "100", "300", "0"                                                                                      |
| LicenseState         | The U.S. state where the vehicle’s license plate is registered              | "VA", "NJ"                                                                                             |
| WaiverRequestDate    | Date when the vehicle owner requested a waiver for the ticket               | "02/11/2022", "10/15/2025"                                                                             |
| WaiverGrantedDate    | Date when a waiver was approved (if applicable)                             | "03/12/2005", "11/08/2023"                                                                             |
| AppealDate           | Date when the ticket was appealed                                           | "05/21/2020", "09/18/2009"                                                                             |
| AppealGrantedDate    | Date when the appeal was granted (if successful)                            | "02/11/2022", "10/15/2025"                                                                             |
| ViolationDescription | A text description of the violation                                         | "Void", "No Parking any time", "Curb Painted Yellow", "Overtime Parking", "Permit Zone w/o Permit"     |
| AppealStatus         | The status of the appeal                                                    | "n/a", "granted", "denied", "pending"                                                                  |
| Location             | Combined string of the address (Street Number + Street Name)                | "100 W WATER ST", "1609 UNIVERSITY AVE"                                                                |
| LicensePlateAnon     | An anonymized numeric code representing the license plate                   | "24,050", "122,369"                                                                                    |
| WaiverStatus         | Outcome/status of the waiver request                                        | "Granted", "Denied", "Pending"                                                                         |

## Exploratory Plots
![Tickets by Day of Week and Hour](Tickets%20by%20Hour.png)
![Number of Tickets Over Time](Number%20of%20Tickets.png)
