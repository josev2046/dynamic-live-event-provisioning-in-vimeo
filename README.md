# Vimeo Live Event Provisioning Script

This repository contains a simple HTML and JavaScript script designed to provision a live event on Vimeo and display the necessary credentials and embed code.

## Overview

This script allows users to create a live event on Vimeo directly from a web page. It handles the API calls to Vimeo, retrieves the necessary streaming credentials, and embeds the live player into the page.

![dynamic_live_provisioning](https://github.com/user-attachments/assets/ba443121-576b-4832-b298-4b2a9e5449a0)


## Functionality

*  **Provision Live Event:**
    * Clicking the "Provision Live Event" button triggers the creation of a new live event on Vimeo.
    * The script uses the Vimeo Live API to create the event, providing details such as the event title, stream title, and privacy settings.
    * Upon successful creation, the script retrieves the streaming credentials and the embed code for the player.
*  **Display Credentials:**
    * The RTMP and RTMPS links, along with the stream key, are displayed on the page, allowing users to configure their streaming software (e.g., OBS).
*  **Embed Player:**
    * The embed code provided by Vimeo is used to display the live player directly on the web page.
*  **Refresh Player:**
    * A "Refresh Player" button is provided to re-embed the player, in case of issues.
*  **Status Updates:**
    * The script provides status updates throughout the process, indicating whether the event was created successfully, whether credentials were retrieved, and if any errors occurred.


## Potential Use Cases

This script can be integrated into Content Management Systems (CMS) or Learning Management Systems (LMS) to provide live streaming functionality.
