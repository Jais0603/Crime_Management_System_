This  project revolves around the development of a Criminal Database Management System (CDMS). This system aims to provide a comprehensive platform for law enforcement agencies to efficiently manage and access information related to police stations, officers, criminals, and victims. By organizing data in a structured manner, the CDMS facilitates the effective coordination of law enforcement efforts, aiding in maintaining public safety and upholding justice.

**Functionality and Key Components:**

1. **Police Station Table (Policestation):** This table serves as the foundation of the system, containing crucial information about various police stations. The attributes include:
   - `stationID` (Primary Key): A unique identifier for each police station.
   - `stationName`: The name of the police station.
   - `address`: The physical address of the station.
   - `city`: The city in which the station is located.
   - `State`: The state where the station operates.
   - `PhoneNo`: Contact phone number for the station.
   - `email`: Contact email address for the station.
   - `chiefOfficer`: Name of the chief officer in charge.
   - `officerCount`: The count of officers stationed at the location.

2. **Officers Table (Officers):** This table stores information about law enforcement officers assigned to various stations. Attributes include:
   - `OfficersID` (Primary Key): A unique identifier for each officer.
   - `FirstName`: First name of the officer.
   - `middleName`: Middle name of the officer.
   - `LastName`: Last name of the officer.
   - `position`: The officer's position or rank.
   - `Badgenumber`: A unique badge number for identification.
   - `department`: The department the officer belongs to.
   - `stationID` (Foreign Key): Links the officer to a specific police station.

3. **Criminal Table (Criminal):** This table holds information about criminals and their associated records. Attributes include:
   - `criminalID` (Primary Key): A unique identifier for each criminal.
   - `FirstName`: First name of the criminal.
   - `MiddleName`: Middle name of the criminal.
   - `LastName`: Last name of the criminal.
   - `Gender`: Gender of the criminal.
   - `DateOfBirth`: Date of birth of the criminal.
   - `Nationality`: Nationality of the criminal.
   - `Height`: Height of the criminal.
   - `Weight`: Weight of the criminal.
   - `EyeColor`: Eye color of the criminal.
   - `HairColor`: Hair color of the criminal.
   - `TattoosAndScars`: Description of any tattoos or scars.
   - `Address`: Address of the criminal.
   - `City`: City where the criminal resides.
   - `State`: State where the criminal is located.
   - `ArrestDate`: Date of the criminal's arrest.
   - `ArrestingOfficerID` (Foreign Key): Refers to the arresting officer's ID.
   - `crime`: Description of the crime committed.
   - `punishment`: Details of the criminal's punishment.

4. **Victim Table (Victim):** This table stores information about the victims of crimes. Attributes include:
   - `victimID` (Primary Key): A unique identifier for each victim.
   - `FirstName`: First name of the victim.
   - `MiddleName`: Middle name of the victim.
   - `LastName`: Last name of the victim.
   - `Gender`: Gender of the victim.
   - `DateOfBirth`: Date of birth of the victim.
   - `Nationality`: Nationality of the victim.
   - `Address`: Address of the victim.
   - `City`: City where the victim resides.
   - `State`: State where the victim is located.
   - `PhoneNo`: Contact phone number for the victim.
   - `Email`: Contact email address for the victim.
   - `IncidentDate`: Date of the incident involving the victim.
   - `ReportingOfficerID` (Foreign Key): Refers to the officer reporting the incident.
   - `CriminalID` (Foreign Key): Links to the associated criminal, if applicable.
   - `crime_happened`: Description of the crime against the victim.

**Keys:**

- **Primary Key (PK):** A unique identifier for each record in the table.
- **Foreign Key (FK):** A field in a table that is linked to the primary key of another table. It establishes relationships between tables.

In summary, this Criminal Database Management System is designed to streamline the management of crucial data related to law enforcement. It enables efficient tracking of criminals, victims, officers, and police stations, enhancing collaboration and decision-making within law enforcement agencies. The project aims to contribute to public safety by providing a reliable and structured platform for managing criminal information.
