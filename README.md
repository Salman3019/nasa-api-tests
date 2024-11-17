# Mars Rover Photos API
This project interacts with NASA's Mars Rover Photos API to fetch and analyze photos taken by the Curiosity and Opportunity rovers on Mars. The goal is to demonstrate how to retrieve images from the API based on different parameters such as sol (Martian day), camera type, and rover name.

## Overview
NASA's Mars Rover Photos API provides access to photos taken by the Mars rovers, including Curiosity, Opportunity, and others. You can retrieve photos based on specific days (sols) and the cameras used for taking the pictures. This project demonstrates two use cases for retrieving rover photos.

## Features
- Fetch photos from Curiosity rover for a given Martian day (sol).
- Fetch specific photos from Opportunity rover taken with the Panoramic Camera (PANCAM).
- Retrieve data about the cameras used and the number of photos taken.

## Example Use Cases
## 1. Fetching Photos from Curiosity Rover (Sol 1666)
This query retrieves all photos taken by the Curiosity rover on sol 1666 and lists the cameras used:
https://api.nasa.gov/mars-photos/api/v1/rovers/curiosity/photos?sol=1666&api_key=DEMO_KEY



- **Response Details:**
- Total photos: **54**
- Cameras used:
  - `NAVCAM`
  - `FHAZ`
  - `MARDI`
  - `RHAZ`
- The photos are available for download and analysis.

#### Additional Information (Manifest API)
To gather general rover data, such as the number of photos taken and the available cameras, you can use the Manifest API:
https://api.nasa.gov/mars-photos/api/v1/manifests/curiosity?api_key=DEMO_KEY


- **Response Details:**
- `total_photos`: **54**
- Cameras:
  - `CHEMCAM`
  - `FHAZ`
  - `MARDI`
  - `RHAZ`
### 2. Fetching Specific Photo from Opportunity Rover (Sol 1)
This query retrieves the photo with `id = 268034`, taken by the Opportunity rover on sol 1, using the Panoramic Camera (PANCAM).
https://api.nasa.gov/mars-photos/api/v1/rovers/opportunity/photos?sol=1&api_key=DEMO_KEY&camera=pancam


- **Response Details:**
- `id`: 268034
- `sol`: 1
- `camera`: `PANCAM` (Panoramic Camera)
## How to Use
1. Clone the repository:
 ```bash
 git clone https://github.com/yourusername/nasa-api-project.git


