# Aigeon AI Google Images Light API

## Project Description

The Aigeon AI Google Images Light API is a Python-based server application designed to facilitate advanced image searches using Google's image search capabilities. This project leverages the SerpAPI service to perform detailed and customizable image queries, providing users with a powerful tool to retrieve images based on a wide range of parameters.

## Features Overview

- **Advanced Image Search**: Perform image searches with a variety of customizable parameters such as location, language, image size, color, type, and more.
- **Flexible Query Parameters**: Utilize numerous parameters to refine search results, including date ranges, aspect ratios, and licenses.
- **Integration with SerpAPI**: Seamlessly integrates with SerpAPI to fetch image search results, ensuring accurate and up-to-date data retrieval.
- **Environment Configuration**: Utilizes environment variables for secure API key management.

## Main Features and Functionality

The core functionality of this project revolves around the `search_images_light` function, which is a tool registered with the FastMCP server. This function allows users to perform highly customizable image searches by specifying various parameters. Below are some of the key features:

- **Query Customization**: Users can define search queries using typical Google search operators such as `inurl:`, `site:`, and `intitle:`.
- **Location and Language Options**: Specify the origin of the search and the language to tailor results to specific regions or languages.
- **Date Range Filtering**: Limit search results to specific time periods using start and end dates or relative time periods.
- **Image Attributes**: Filter images by size, aspect ratio, color, and type to find exactly what you need.
- **Licensing and Safety**: Control the scope of image licenses and the level of safe search filtering.
- **Pagination and Device Simulation**: Manage result pagination and simulate searches from different devices like desktops, tablets, or mobile phones.

## Main Function Description

### `search_images_light`

This function is the primary tool for conducting image searches. It accepts a variety of parameters that allow for detailed customization of search queries:

- **`q`**: The main query string for the image search.
- **`location`**: Specifies the geographic location from which the search should originate.
- **`uule`**: Encoded location parameter for Google searches.
- **`google_domain`**: Defines the Google domain to use, defaulting to `google.com`.
- **`gl`**: Country code for the search.
- **`hl`**: Language code for the search.
- **`cr`**: Restricts search to specific countries.
- **`period_unit` and `period_value`**: Define the time period for recent images.
- **`start_date` and `end_date`**: Specify the date range for the search.
- **`tbs`**: Advanced search parameters.
- **`imgar`, `imgsz`, `image_color`, `image_type`**: Define image attributes like aspect ratio, size, color, and type.
- **`licenses`**: Specify the scope of image licenses.
- **`safe`**: Set the level of filtering for adult content.
- **`nfpr`**: Exclude results from auto-corrected queries.
- **`filter`**: Enable or disable filters for similar and omitted results.
- **`start`**: Result offset for pagination.
- **`device`**: Simulate search from different devices.
- **`no_cache`**: Force fresh results from SerpAPI, bypassing cache.

This function is designed to provide a comprehensive and flexible interface for users to perform image searches tailored to their specific needs.