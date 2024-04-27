# San Francisco Big Query
## Relations
### 311 Service Requests
| Field Name | Type | Description |
| ---------- | -----| ------------|
| unique_key |  INT | Case id|
| created_date | TIMESTAMP | Date/time when service was requested|
| closed_date | TIMESTAMP | Date/time service was closed|
| resolution_action_date | TIMESTAMP | Date/time when service was last modified|
| status | STRING | Current status of the service request |
| status_notes | STRING | Explanation of why status was changed to current status|
| agency_name | STRING | The agency responsible for fulfilling the request| 
| category | STRING | The Human readable name of request type|
| complaint_type | STRING | More specific description of the problem related to the Category|
| descriptor |  STRING | More specific description of the problem related to Request Type|
| incident_address | STRING | Human readable address or description of location |
| supervisor_district| INT | - |
| neighborhood | STRING | - |
| location | STRING | Latitude and longitude|
| source | STRING | How was the service request was made|
| latitude | FLOAT | Latitude |
| longitude | FLOAT | Longitude |
| police_district | STRING | - |

### Bikeshare Stations
| Field Name | Type | Description |
| ---------- | -----| ------------|
| station_id | INT | Station id number|
| name | STRING | Name of station|
| latitude | FLOAT | Latitude |
| longitude | FLOAT | Longitude |
| dockcount | INT | Number of total docks at station |
| landmark | STRING | City |
| installation_date | DATE | Original date that station was installed |

### Bikeshare Status
| Field Name | Type | Description |
| ---------- | -----| ------------|
| station_id | INT | Station ID number |
| bikes_available | INT | Number of available bikes |
| docks_available | INT | Number of available docks |
| time | TIMESTAMP | Date/time, PST|

### Bikeshare Trips
| Field Name | Type | Description |
| ---------- | -----| ------------|
| trip_id | INT | Bike trip ID|
| duration_sec | INT | Time of trip in seconds |
| start_date | TIMESTAMP | Start date/time of trip|
| start_station_name | STRING| Station name of start station|
| start_station_id | INT | Numeric reference for start station |
| end_date | TIMESTAMP | End date/time of trip|
| end_station_name| STRING | End station name |
| end_station_id | INT | End station ID|
| bike_number | INT | ID of bike used |
| zip_code | STRING | Home zip code of subscriber| 

### Film Locations
| Field Name | Type | Description |
| ---------- | -----| ------------|
| title | STRING | - |
| release_year | INT | - |
| locations | STRING | - |
| production_company | STRING | - | 
| director | STRING | - |
| writer | STRING | - |
| actor_1 | STRING | - |
| actor_2 | STRING | - |

### SFFD Service Calls
| Field Name | Type | Description |
| ---------- | -----| ------------|
| call_number | INT | Unique 9-digit number assigned by the 911 Dispatch Center to this call |
| unit_id | STRING | Unit ID |
| incident_number | INT | Unique 8-digit number to this Fire incident |
| call_type | STRING | Type of call |
| call_date | DATE | Date the call is received at the 911 Dispatch|
| response_timestamp | TIMESTAMP | Date/time response unit is en route to the location of the call|
| on_scene_timestamp | TIMESTAMP | Date/time the unit arrives to the location of incident|
| address | STRING | Address of the incident reported |
| city | STRING | City of the incident |
| zipcode_of_incident| STRING | Zip code of incident |
| station_area | STRING | Fire Station Firest Response Area associated with the address of incident |

### SFPD Incidents
| Field Name | Type | Description |
| ---------- | -----| ------------|
| unique_key | INT | Incident ID number |
| category | STRING| - |
| descript | STRING | -| 
| dayofweek | STRING | - |
| pddistrict | STRING | Police Department district |
| resolution | STRING | Whether there was an arrest, citation, booking, etc |
| address | STRING | - |
| latitude | FLOAT | - |
| longitude | FLOAT | - |
| timestamp | TIMESTAMP| - |

