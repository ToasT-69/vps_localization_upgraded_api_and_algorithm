# vps_localization_upgraded_api_and_algorithm

## Overview
This repository is a fork and updated version of the original VPS_Localization project. It is currently experimental and has a number of rough edges, but serves as a foundation for testing indoor localization approaches where GPS is ineffective.

The system leverages annotated floor plans and the Gemini 2.5 API for position estimation. It uses OpenCV for landmark detection and supports both automatic and manual annotation to refine accuracy.

## Features
- Indoor localization using annotated digital floor plans  
- Integration with Gemini 2.5 API for position estimation  
- OpenCV-based landmark detection (shops, storefronts, etc.)  
- Manual annotation support for refining landmarks  
- Multiprocessing support with progress bars and logs for better visibility  
- Experimental: may contain incomplete or rough features  

## Tech Stack
- Python 3.10+  
- OpenCV – Image processing and annotation  
- tqdm – Progress visualization  
- Multiprocessing – Parallelized preprocessing  
- Gemini 2.5 API – Landmark-based position estimation  

## Data Structures Used
- Lists – Store detected landmarks and corridor points  
- Dictionaries – Map landmarks to coordinates and metadata  
- Tuples – Represent (x, y) coordinates  

## Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/vps_localization.git
   cd vps_localization
