# Dream Team MIST 4610 Group Project 1

## Team Name 
_The_ Dream Team

## Team Members 
1. Vivian Aguirre @vivianyaguirre
2. Lindsey Rubury @lindseyrubury
3. Ronit Subramanian @ronsub101
4. Lance Moxley @lcm85000

## Problem Description:
This database supports the organization of a sample Pet Adoption System. It covers many Pet Adoption operations including Adopting, Fostering, Pet Care, Adoption Center Supply Management, Adoption Events, Employee Supervision etc. Queries can be conducted on this database to provide managerial insight on process operations. Furthermore, through this project, we would like to perform queries on the data model in order to prove why Managers would care about this database, and how they can utilize it to improve their operational efficiency. 


## Data Model 
Explanation of the Data Model:

Our model is based on the operations of a hypothetical Pet Adoption Agency. The Shelter Locations are the main part of the data model, where many of the different aspects of a pet adoption agency are located.The ShelterLcoation entity contains the unique identifier along with its name, address, email, and assigned supervisor. A single shelter location can have many employees, as represented by a one to many relationship between the ShelterLocations and Employees entities. Each employee has its own unique identifier along with their name, role, email, what shelter they work for, and what supervisor they report to. A shelter location will have one shelter supervisor that oversees operations at the shelter and is in charge of many employees.

Arguably the most important part of a pet shelter is that they house many pets within each of their facilities, as represented by the one to many relationship between ShelterLocations and Pets. Each pet has a unique id and various identifing information is recorded for each pet, most notably, their health status and adoption status. Each pet's home shelter is also recorded in this data entity. Pets can either be adopted or fostered and is represented by a one to many relationship from the Pets entity to the FosterRecord and Adopted entities. The FosterRecord entity contains the starting and ending date for the fostering period and the Adopted entity contains a follow-up date for after a pet has been adopted. Both of these entites contain the pet that was fostered/adopted and who fostered/adopted the pet. At the bottom left corner of the model, there is an Adopters entity which has a one to many relationship between the FosterRecord and Adopted entities, meaning that one adopter can foster/adopt multiple pets. Each adopter has a unique identifier, as well as their name, address, email, and how many adoptions they have completed. 

For the pets that require medicical attention, we created an entity called PetMedications, that tracks the medication name, purpose, and potential side effects. Each pet medication can be potentially used for many different treatments. Each treatment has a unique identifier, along with the dosage, date of treatment, what medication was used, and which pet was administered the medicine. Treatments are performed for pets that have a 'Unhealthy' health status.

One supplier provides many supplies and is indicated by a one to many relationship between the Suppliers and Supplies entities. Suppliers have a unique identifier, along with the name of their business and their contact information. Supplies also have unique identifiers and record the name of the supply, type of supply, quanity of the supply, and what supplier was the source. Shelters have many supply lists that contain many different supplies. For the purposes of this data model, we generally assume that one shelter sticks to buying supplies from one supplier. 

Lastly, a single location can host many different events and is signified with a one to many relationship between the ShelterLocations and the Events entity. A single location can also have many volunteers, as there yet another one to many relationship between the ShelterLocations and the Volunteers entities. There is another entity that we named EventVolunteerRoster, which has a many to many relationship between Events and Volunteers, which means that there can be many volunteers for many different events. Each event has its own identifier, name, location, date, and which shelter is hosting the event. Each volunteer also has a unique identifier, their name, assigned role, email, and the shelter that the represent. 





![pet-eer](https://github.com/user-attachments/assets/ee5abaf2-832e-4053-b8b0-7ee07b7c0317)

## Data Dictionary 
![image](https://github.com/user-attachments/assets/8ede5bf4-c3b9-4237-b0c0-c5eadb5178f6)
![image](https://github.com/user-attachments/assets/66474dc0-bd61-47c9-a967-4f19e10fcf52)
![image](https://github.com/user-attachments/assets/c3d3b127-e313-4c56-b321-96a9bc30aa71)
![image](https://github.com/user-attachments/assets/a69e0064-e8bf-42c7-b8a2-751e8399b243)
![image](https://github.com/user-attachments/assets/dc38b102-9d49-4966-a55e-a51f9bb7f82b)
![image](https://github.com/user-attachments/assets/a162d556-3080-44ac-8263-48925b5369ba)
![image](https://github.com/user-attachments/assets/ec351849-6b58-4366-94b4-29d3203b0ef0)
![image](https://github.com/user-attachments/assets/04d80a75-e822-4991-9478-3da09f71cba1)
![image](https://github.com/user-attachments/assets/76c8096f-cedc-46ea-b1c4-4f64cc9d7e5d)
![image](https://github.com/user-attachments/assets/9707be35-6fa5-4146-a37b-293f81a386d1)
![image](https://github.com/user-attachments/assets/7bd27824-2022-4494-8ed0-674ffb0a32ef)
![image](https://github.com/user-attachments/assets/2024f8ec-079b-45a2-b82f-1e415066e99c)
![image](https://github.com/user-attachments/assets/4a4d2ac4-cd79-405d-9d80-c2ef5b55eb82)
![image](https://github.com/user-attachments/assets/414d6e87-04f1-4abe-b7ba-f92d63a1409c)

## Queries 
 ![image](https://github.com/user-attachments/assets/75509222-3188-4f22-8777-84274ed7e9b2)


Query 1: Retrieve a summary of pets with health issues. Include the shelter name and the number of pets with health issues per shelter. Additionally, list their health statuses and adoption statuses in the output. 

<img width="628" alt="Q1" src="https://github.com/user-attachments/assets/db3e2509-808a-457f-a8ba-431d3184e7f6">

Q1 Managerial Perspective: This query generates a summary of pets with health issues across various shelters. It provides the shelter name, the count of pets that are classified as unhealthy, their current health status, and their adoption status. This information can be used to monitor shelters with a higher concentration of pets that require medical attention, potentially identifying shelters that may need additional resources or support. Additionally, the adoption status data helps track the outcomes for pets with health issues, offering insights into how effectively shelters are managing the adoption process for animals with medical concerns.


Query 2: Find pets and their foster records that occured during 2024. This query finds pets and their foster records for those who were fostered between specific dates.

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

Q9 Managerial Perspective: This query provides a clear overview of employees along with their current supervisors, enhancing organizational transparency and accountability. It includes essential information about both the employee and supervisor, such as their names and the locations where they work. By displaying this hierarchical structure, the query helps to clarify reporting relationships within the organization, making it easier for team members to understand their points of contact and lines of communication. Additionally, this information can assist management in evaluating team dynamics and ensuring that employees have access to appropriate support and guidance from their supervisors. Overall, the query serves as a valuable resource for improving communication and collaboration within the workplace.



Query 10: This query gathers current contact information for employees at all of the shelters. 

<img width="630" alt="Q10" src="https://github.com/user-attachments/assets/e3ab1bd8-9750-4603-b060-3c0c06ede16d">


Q10 Managerial Perspective: This query focuses on collecting up-to-date contact information for employees working at all shelters, which is crucial for effective communication and operational efficiency. By aggregating details such as phone numbers and email addresses, the query ensures that management and team members can easily reach out to one another as needed. Having current contact information enhances coordination between shelters and facilitates quick responses to various situations, including emergencies or staffing changes. Furthermore, this data is essential for maintaining an organized communication system, enabling seamless collaboration among employees. Overall, this query plays a vital role in fostering a well-connected and responsive workforce across all shelter locations.

 

## Database Information
Name of the database: cs_vya95458


