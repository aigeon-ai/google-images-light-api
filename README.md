# Aigeon AI Google Images Light API

## Project Description

The **Aigeon AI Google Images Light API** is a Python-based server application designed to facilitate lightweight and efficient image searches using Google's image search capabilities. By leveraging the SerpAPI, this project provides a streamlined interface for querying Google Images with a variety of customizable parameters, allowing users to tailor their search results according to specific requirements such as location, language, image size, and more.

## Features Overview

- **Customizable Search Queries**: Users can define search queries with a wide range of parameters to refine their image search results.
- **Location and Language Support**: The API supports searches from specific locations and in various languages, simulating real user searches.
- **Advanced Filtering Options**: Includes filters for image aspect ratio, size, color, type, and licenses, among others.
- **Time-Based Search**: Allows searches to be limited to specific time periods or date ranges.
- **Pagination and Device Emulation**: Supports pagination of results and emulation of different device types (desktop, tablet, mobile).

## Main Features and Functionality

1. **Search Images Light Functionality**:
   - The primary function, `search_images_light`, allows users to perform Google Images searches with a variety of parameters.
   - Parameters include query terms, location, language, image size, color, type, and more, providing extensive control over the search results.

2. **Parameter Customization**:
   - **Query (`q`)**: Define the search query using standard Google search operators.
   - **Location (`location`)**: Specify the origin of the search to simulate user location.
   - **Language (`hl`)**: Choose the language for the search results.
   - **Image Attributes**: Filter images by aspect ratio (`imgar`), size (`imgsz`), color (`image_color`), and type (`image_type`).
   - **Licensing (`licenses`)**: Restrict search results to images with specific usage rights.
   - **Time Constraints**: Limit searches to specific periods using `period_unit`, `period_value`, `start_date`, and `end_date`.

3. **Advanced Search Options**:
   - **Safe Search (`safe`)**: Control the level of adult content filtering.
   - **Pagination (`start`)**: Manage result pagination for large sets of search results.
   - **Device Emulation (`device`)**: Specify the type of device to emulate during the search.

## API Endpoints or Main Functions Description

### `search_images_light`

The `search_images_light` function is the core of the API, providing a comprehensive interface for performing image searches. Below is a detailed description of its parameters:

- **`q`**: The search query string. It supports Google search operators for refined searches.
- **`location`**: Optional parameter to specify the search's geographic origin.
- **`uule`**: Google encoded location for search, mutually exclusive with `location`.
- **`google_domain`**: Specifies the Google domain to use (e.g., google.com).
- **`gl`**: Country code for the search.
- **`hl`**: Language code for the search.
- **`cr`**: Restricts search to specific countries.
- **`period_unit` & `period_value`**: Define the time period for recent images.
- **`start_date` & `end_date`**: Specify a date range for the search.
- **`tbs`**: Advanced search parameters.
- **`imgar`**: Aspect ratio of images.
- **`imgsz`**: Size of images.
- **`image_color`**: Color of images.
- **`image_type`**: Type of images.
- **`licenses`**: Licensing scope of images.
- **`safe`**: Level of adult content filtering.
- **`nfpr`**: Exclude results from auto-corrected queries.
- **`filter`**: Enable or disable filters for similar and omitted results.
- **`start`**: Result offset for pagination.
- **`device`**: Device type for search results.
- **`no_cache`**: Force fresh results from SerpAPI.

This API is designed to provide users with a powerful tool for conducting detailed and specific image searches, making it ideal for applications that require precise image retrieval capabilities.