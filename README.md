# NetPractice

*This project has been created as a part of the 42 curriculum by alicigar.*

## Description

NetPractice is a practical introduction to computer networking. The goal is to solve 10 exercises by configuring simulated networks so that all devices can communicate with each other correctly.

To complete the exercises, you need to understand the following concepts:

## Instructions

How to run the training interface:

-Download the project files from the project page and extract them into a folder of your choice.

Open a terminal in that folder and run:

    ./run.sh

Then, your browser will open automatically. 

If it doesn't, you can start the server manually:

    python3 -m http.server 49242

Then open your browser and navigate to http://localhost:49242.
You may change the port number if needed — just make sure the URL matches the port you chose.

### How to use the interface:

- Enter your 42 intranet login in the field.

- Select **Training** to practice at your own pace, or **Evaluation** to generate a random configuration suitable for defense.

- Modify the white/unshaded fields to fix the network configuration.

- Click **Check again** to verify your solution.

- Once a level is completed, click **Get my config** to download your configuration file before moving to the next level.

### Submission requirements:

Complete all 10 levels and export one configuration file per level and place all 10 files at the root of your Git repository.

## Resources

The subject provided by 42 was used as a primary resource throughout the development process.

Additional external resources (such as tutorials and technical articles) were consulted to reinforce understanding and will be listed in this section:

-
-
-
-

During the development of this project, AI was used as a learning support tool, mainly to:

-Clarify theoretical concepts related to networking, such as TCP/IP addressing, subnetting, routing tables, and the OSI model.
-Assist in writing and improving the project documentation.
-Help formulate questions and understand how the exercises work, without generating or copying solutions directly.

All AI-assisted content was reviewed, fully understood and validated, and all final design and implementation decisions were made consciously and responsibly. The project's code was entirely written and tested by me.
