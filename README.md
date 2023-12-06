# CARMELA API

This API provides endpoints for accessing sentiment analysis data extracted by CARMELA, a component of the PACO and CARMELA project ([Original Repository](https://github.com/Kohkitos/paco_and_carmela/tree/main)).

## Overview

The CARMELA API offers endpoints to retrieve sentiment analysis data obtained from live YouTube video comments. It enables users to access sentiment analysis results processed by CARMELA in real-time during the live video streams.

## Usage

### Retrieve Messages from Day 15
```bash
curl TBD
```
Retrieves messages from day 15 based on the specified sentiment, start timestamp, and end timestamp.

### Retrieve Messages from Day 16
```bash
curl TBD
```
Retrieves messages from day 16 based on the specified sentiment, start timestamp, and end timestamp.

### Param Format for `15_` and `16_` Endpoints

The `15_` and `16_` endpoints accept parameters in the following format:

- **SENT-start_timestamp-end_timestamp**
  - **SENT**: A string with POS, NEG, and NEU in any combination (e.g., POSNEG, NEGPOS, POSNEGNEU).
  - **start_timestamp**: The starting timestamp in minutes.
  - **end_timestamp**: The ending timestamp in minutes.

Example: `POS-20-25`
- Retrieves positive messages on day 15 from minute 20 to 25.


### Retrieve Day-wise Timestamps
```bash
curl TBD
```
Retrieves start and end timestamps for each day within a specified date range.

### Calculate Max and Min Comments Timestamps
```bash
curl TBD
```
Calculates the timestamp with the maximum and minimum number of comments within a specified timestamp range.

## License

This API is available under the [MIT License](LICENSE).
