## Web Scraping the Ryman Calendar

This exercise uses BeautifulSoup to obtain a dataset of upcoming events at the Ryman. This information is available at https://ryman.com/events/. The contents of this website are converted into a pandas DataFrame. Note: The website splits the events across multiple pages.

1. Used a web inspector to identify a tag that contains the names of all headliners (e.g. for Vince Gill, featuring Wendy Moten, only pull Vince Gill.) This was used to create a list containing the names of each inductee.

2. Found a tag that gives the date and time for each show. Extracted these into two lists, one containing the date and the other containing the time (e.g. THURSDAY, AUGUST 4, 2022 AT 8:00 PM CDT was split into August 4, 2022 and 8:00 PM CDT.)

3. Took these two lists and converted them into a pandas DataFrame.

4. Using a for-loop, applied the above code across the rest of the event pages to scrape all inductees.

5. Added the opening act for all shows that list an opener.

6. Retrieved ticket prices for each show, accounting for cases where the show was canceled or rescheduled.
