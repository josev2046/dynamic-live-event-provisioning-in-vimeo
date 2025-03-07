# Vimeo Live Event Provisioning Script

This repository contains a simple HTML and JavaScript script designed to provision a live event on Vimeo and display the necessary credentials and embed code.

## Overview

This script allows users to create a live event on Vimeo directly from a web page. It handles the API calls to Vimeo, retrieves the necessary streaming credentials (RTMP/RTMPS links, stream key), and embeds the live player into the page.

![dynamic_live_provisioning](https://github.com/user-attachments/assets/ba443121-576b-4832-b298-4b2a9e5449a0)


## Functionality

1.  **Provision Live Event:**
    * Clicking the "Provision Live Event" button triggers the creation of a new live event on Vimeo.
    * The script uses the Vimeo API to create the event, providing details such as the event title, stream title, and privacy settings.
    * Upon successful creation, the script retrieves the streaming credentials and the embed code for the player.
2.  **Display Credentials:**
    * The RTMP and RTMPS links, along with the stream key, are displayed on the page, allowing users to configure their streaming software (e.g., OBS).
3.  **Embed Player:**
    * The embed code provided by Vimeo is used to display the live player directly on the web page.
4.  **Refresh Player:**
    * A "Refresh Player" button is provided to re-embed the player, in case of issues.
5.  **Status Updates:**
    * The script provides status updates throughout the process, indicating whether the event was created successfully, whether credentials were retrieved, and if any errors occurred.

## Usage

1.  **Replace Placeholders:**
    * In the JavaScript code, replace `{TOKEN}` with your Vimeo access token.
    * Replace `{USER}` with your Vimeo user ID.
2.  **Open in Browser:**
    * Open the `index.html` file in a web browser.
3.  **Provision Event:**
    * Click the "Provision Live Event" button.
4.  **Configure Streaming Software:**
    * Use the displayed RTMP/RTMPS links and stream key to configure your streaming software.
5.  **Start Streaming:**
    * Begin streaming from your software.
6.  **Watch Live Stream:**
    * The live stream will appear in the embedded player on the web page.
7. **Refresh Player:**
    * Click the "Refresh Player" button to refresh the embedded player.

## Code Explanation

* **HTML Structure:**
    * The HTML includes buttons for provisioning the event and refreshing the player, as well as divs for displaying status messages, credentials, and the embedded player.
* **JavaScript Logic:**
    * The JavaScript code uses the `fetch` API to make requests to the Vimeo API.
    * It handles the creation of the live event, retrieval of credentials, and embedding of the player.
    * Error handling is included to display error messages to the user.
* **Vimeo API:**
    * The script uses the Vimeo API to create live events and retrieve event details.
    * It utilises the POST method to create events and the GET method to retrieve event details.
    * The Accept header specifies the API version.

## Potential Use Cases

This script can be integrated into Content Management Systems (CMS) or Learning Management Systems (LMS) to provide live streaming functionality.
