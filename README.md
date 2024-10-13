# Dream Team MIST 4610 Group Project 1

## Team Name 
Dream Team

## Team Members 
1. Vivian Aguirre @vivianyaguirre
2. Lindsey Rubury @lindseyrubury
3. Ronit S
4. Lance Moxley @lcm85000

## Problem Description:
This database supports the organization of a sample Pet Adoption System. It covers many Pet Adoption operations including Adopting, Fostering, Pet Care, Adoption Center Supply Management, Adoption Events, Employee Supervision etc. Queries can be conducted on this database to provide managerial insight on process operations. Furthermore, through this project, we would like to perform queries on the data model in order to prove why Managers would care about this database, and how they can utilize it to improve their operational efficiency. 


## Data Model 
![pet-eer](https://github.com/user-attachments/assets/ee5abaf2-832e-4053-b8b0-7ee07b7c0317)

## Data Dictionary 

## Queries 
 INSERT QUERY TABLE HERE !!!!!

Query 1: Retrieve a summary of pets with health issues. Include the shelter name and the number of pets with health issues per shelter. Additionally, list their health statuses and adoption statuses in the output. 

<img width="628" alt="Q1" src="https://github.com/user-attachments/assets/db3e2509-808a-457f-a8ba-431d3184e7f6">

Q1 Managerial Perspective: This query generates a summary of pets with health issues across various shelters. It provides the shelter name, the count of pets that are classified as unhealthy, their current health status, and their adoption status. This information can be used to monitor shelters with a higher concentration of pets that require medical attention, potentially identifying shelters that may need additional resources or support. Additionally, the adoption status data helps track the outcomes for pets with health issues, offering insights into how effectively shelters are managing the adoption process for animals with medical concerns.


Query 2: Find Pets and Their Foster Records that occured during 2024. This query finds pets and their foster records for those who were fostered between specific dates.

<img width="628" alt="Q2" src="https://github.com/user-attachments/assets/18f94468-229c-4ab1-98b6-1f389a3a769d">

Q2 Managerial Perspective: This query identifies pets and their foster records from 2024, focusing on those placed in foster care within specific start and end dates. By tracking the duration and number of foster placements for each pet, management can monitor foster program activity and assess how effectively pets are being matched with foster families. This data helps identify pets with extended foster stays or multiple placements, which may signal a need for additional resources or better matching strategies. It also supports more efficient resource allocation, ensuring pets and foster families receive the appropriate level of support. Ultimately, these insights can guide improvements in the foster care process and help increase adoption rates.


Query 3: Find out which shelters have administered the highest number of different medications to their pets. 

<img width="628" alt="Q3" src="https://github.com/user-attachments/assets/61eae06d-5fb1-4665-9a5c-1b0c73d6444b">

Q3 Managerial Perspective: This query identifies shelters that have administered the highest number of different medications to their pets. It focuses on the distribution of medications across shelters, giving insight into which shelters may have more complex or varied medical needs among their animal populations. The results can help shelter managers understand where the heaviest medical intervention is occurring and may highlight shelters that require additional medical supplies, support, or funding. This information is essential for resource allocation and ensuring that shelters can continue to provide the necessary care for their animals.


Query 4: This query calculates the average age of pets adopted from each shelter.

<img width="628" alt="Q4" src="https://github.com/user-attachments/assets/23bfeae0-ee25-424d-a5e4-3d60e8fec4df">

Q4 Managerial Perspective: This query calculates the average age of pets adopted from each shelter, providing insight into adoption trends related to pet age. Shelters can use this information to understand whether younger or older pets are more frequently adopted, which can inform strategies for promoting the adoption of different age groups. Knowing the average age of adopted pets may also help shelters tailor their care and outreach efforts, ensuring they meet the needs of both younger and older pets to improve overall adoption rates. This data is valuable for making informed decisions on how to market pets for adoption.


Query 5: This query shows the most common pet breeds across all shelters, grouped by breed and ordered by the number of adoptions in descending order.

<img width="628" alt="Q5" src="https://github.com/user-attachments/assets/d4c4acee-8499-48d3-b359-3624d089ec0c">

Q5 Managerial Perspective: This query identifies the most common pet breeds across all shelters, grouped by breed and ranked by the number of adoptions in descending order. By revealing which breeds are adopted most frequently, shelters can adjust their resources and promotional efforts based on breed popularity. This information can be useful for targeting potential adopters who are interested in specific breeds and for planning future intakes. Additionally, shelters can analyze trends in breed adoptions to better meet the preferences of their communities and manage breed-specific needs more effectively.


Query 6: Select average quantity of the supplies per shelter, along with a total count of supplies of each type available at each shelter.

<img width="630" alt="Q6" src="https://github.com/user-attachments/assets/33af0548-e79d-47b4-bdd6-e83c5c27be93">

Q6 Managerial Perspective: This query retrieves the average quantity of supplies available per shelter, along with a total count of each type of supply at each shelter. By providing insights into the distribution and availability of supplies, shelter managers can better understand which locations may need restocking or redistribution of resources. The data can also help identify shelters that manage their supplies more efficiently or those that may require additional support. This information is critical for maintaining smooth shelter operations and ensuring that each location has the necessary resources to care for its animals effectively.


Query 7: This query tracks volunteer involvement through the events they have participated in by shelter.
<img width="630" alt="Q7" src="https://github.com/user-attachments/assets/1be17f7d-7e4d-437b-ab88-c98a1aa09338">

Q7 Managerial Perspective: This query tracks the involvement of volunteers across various shelters by monitoring the events they have participated in. It provides valuable insights into volunteer engagement at each shelter, allowing shelter managers to assess participation levels and identify which events attract the most volunteer support. This information can help in planning future events, ensuring optimal volunteer utilization, and recognizing active volunteers. Understanding volunteer involvement is crucial for maintaining efficient shelter operations, as volunteers often play a key role in providing care and support for the animals.



Query 8: Provide a detailed list of all pets currently availible for adoption. Include pet and shelter id, name, species, breed, age, sex.

<img width="630" alt="Q8" src="https://github.com/user-attachments/assets/fc180368-634f-47d3-a3ba-ac002baf4fc5">

Q8 Managerial Perspective: This query generates a comprehensive list of all pets currently available for adoption, presenting essential details to facilitate the adoption process. It includes vital information such as the pet ID and shelter ID, as well as the pet's name, species, breed, age, and sex. This detailed data is instrumental for potential adopters, as it enables them to make informed decisions when selecting a pet that fits their preferences and lifestyle. Additionally, the query assists shelter staff in managing their adoption records effectively, ensuring that all available pets are accurately represented. By providing this information, the query supports the goal of connecting pets with loving homes, ultimately enhancing the adoption experience for both pets and prospective owners.



Query 9: This query lists employees and their current supervisor. Additionally, it shows which location the employee and supervisor work at.

<img width="630" alt="Q9" src="https://github.com/user-attachments/assets/b8d3a403-81b0-427d-b533-724969c3f1ef">

Q9 Managerial Perspective: 


Query 10: This Query gathers current contact information for employees at all of the shelters. 

<img width="630" alt="Q10" src="https://github.com/user-attachments/assets/e3ab1bd8-9750-4603-b060-3c0c06ede16d">


Q10 Managerial Perspective: 

 

## Database Information



