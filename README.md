# getting-started-with-apollo-csharp

This provides the front end for the Apollo Getting Started application.

## Objectives
A short bulleted list of what the reader is expected to learn through this example

## Setup and Running

### Prerequisites

* node v8.1.0

### Running

A `.env` file is required before you can build the application.  This file needs to be added to the root of the project and called `.env`.  This file
contains all the environment variables required for the application.  Currently there is only one required entry:

```BASE_ADDRESS=http://localhost:5000/api```

This value is where you put the relative address of the api.

In order to start this application you need to run:

`npm install` 

and then


`npm run start`

If you would like to build this for deployment then this can be accomplished using:

`npm run build`

## How this Sample Works

This is am example UI which connects to an Apollo database.

Upon entering the application you will be prompted to add your credentials for the Apollo database you want to connect to.

Once you have entered your credentials you will be given the option of either creating a new journey or replaying an existing one.

If you create a new journey, you will enter a name for it.  Once you click launch the system will generate 1000 random sensor readings for each of the 4 sensors displayed (pressure, temperature, speed, location).  These sensor readings will be written to the database.  After the writes have begun the application will begin to read the sensors back in a paged manner and once data has been returned to the UI the system will begin the playback.

If you choose to replay an existing journey once you click on the journey to replay the application will begin to read the sensors back in a paged manner and once data has been returned to the UI the system will begin the playback.

Attribution
Created and Maintained by [bechbd](https://github.com/bechbd)