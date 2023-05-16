# What-Make-the-WPP-Prize---Analysis-of-WPP-Winning-Photos
# AIDM-7410

# Project Introduction

   This is the 7410 project of the Lord of Sham Shui Po, the following is a simple introduction
 
# Directory Structure Description
    ├── ReadMe.md           // help document
    
    ├── output    //  database files that need to be used 

        │   ├── dfimage    // Every photo's information with local storage path by year

    │   ├── dfimageurl    // Every photo's information with image url by year

    │   ├── database_photographer_all.csv   // Every photographer's official information stored in WPP's website combined

    │   ├── dfimageurlall.csv   // Every photo's information with image url combined

    │   ├── dfimageurlall_summerized.csv   // Every photo's information with shorten description

    │   ├── dfimageurlall_summerized_location.csv   // Every photo's information with shorten description and location

    │   ├── timeline   // Awards per country over time

    │   ├── new_df_country(3).csv  // Database for earth model establishment after manual correction of locations
    
    │   ├── photographer   // Top 10,Top 20 photographer 
    
    │   ├── prizegroup  // Distribution of awards for protest-related photos

        │   ├── dfphotographer.csv    // Every works' direct link of presentation page



    
    ├── code           // The core code part, including the basic implementation process of each part
	
    
    │   ├── ScrapeURL.ipynb    // Scrape all stored photos' information and photo url

        │   ├── ImageDownload.ipynb    // Download every photos to local for AI analysis

    │   ├── Summerization.ipynb    // Use pre-trained Flan-T5 model to shorten the description of photo stories

        │   ├── Location-detection.ipynb    // Use UIE base model in cooperation with Spacy and PyCountry library to extract the exact location of each photo where it was taken

    │   ├── Combine picture.ipynb    // Stitch pictures
    
    │   ├── country net.ipynb    // Extraction of the country where the photo was taken, analysis of the photographer's footprint
    
    │   ├── photographer.ipynb    // Recap of awards for all countries
    
 
