# Sec.py
Scrape SEC rule comments
## The use of these files for mirrulations.

If you're using sec.py, you can begin by scraping initial data and saving it to the Mirrulations dataset as raw data. When you run the url command at scale, you can create a docket record. Then, by running a looped scrape on the file_links array, you can collect all the raw comments, including HTML, PDF, and other formats, for a specific SEC rule. In short, this script is a foundational tool for helping Mirrulations gather and organize data related to SEC comments.

File sec.py is a basic file where you can type in the sec rule comment page and it will output the docket ID and description. via command python3 sec.py [url]

## Full list can be found: 
- https://www.sec.gov/rules-regulations/rulemaking-activity
- Single Rule: https://www.sec.gov/rules-regulations/2025/06/s7-11-23#34-103320final
- comments for single rule: https://www.sec.gov/comments/s7-11-23/s71123.htm

## How to use:
Run the command `python3 sec.py https://www.sec.gov/comments/s7-11-23/s71123.htm`

## Sample Output
```
{
  "id": "s7-11-23",
  "title": "Comments on Daily Computation of Customer and Broker-Dealer Reserve Requirements under the Broker-Dealer Customer Protection Rule",
  "file_data": [
    {
      "link": "/comments/s7-11-23/s71123-580435-1668442.pdf",
      "meta": "Text Meta"
    }
  ]
}
```
