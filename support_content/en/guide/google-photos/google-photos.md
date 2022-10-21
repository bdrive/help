# API limits and quotas

All requests sent to the Google Photos Library API are counted toward a quota. We put these limits in place to protect the system and its users.

Access to the API requires OAuth client credentials from a Google developers project. This project must have the Library API enabled as described in Get started.

To learn more about appropriate use of this API, see the Acceptable use policy.

## General quota limits

The quota limit for requests to the Library API is 10,000 requests per project per day. This includes all API requests, such as uploading, listing media, and applying filters, but not accessing media bytes from a base URL.

The quota limit for requests to access media bytes (by loading a photo or video from a base URL) is 75,000 requests per project per day.

In addition to these limits there are other quotas that exist to protect the reliability and integrity of our systems. If you receive a 429 error, you've likely hit one of these quotas. If you receive one of these errors, reduce the number of requests you are making over a given time period. For more information, refer to retrying failed requests and exponential backoff.

## Checking quota usage

To see how much of your available quota you have used, and to view or change usage limits for your project, visit the Quotas page in the Google API Console and select Photos Library API.

## Exceeding quota limits

If the quota of requests to the Library API is exceeded, the API returns an error code 429 and a message that the project has exceeded the quota. For more information, see the Terms of Service.

## Photo storage and quality

All media items uploaded to Google Photos using the API are stored in full resolution at original quality. They count toward the user's storage.
