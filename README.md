### Documentation of the Web Scraping Task By 
## Md Ayyan - mdayyan698@gmail.com  - 8130510698

1. **Task Overview**: Scrape clinic data (name, address, contact number, website) from Yellow Pages for Queensland general practices.

2. Imported `selenium`, `pandas`. Initialized Edge WebDriver.

3.  Used  Yellow Pages search page for general practice clinics in Queensland.

4. Created empty lists: `Clinic_name`, `Address`, `Website`, `Contact_number`.

5.  Loop through the first 35 pages; used `WebDriverWait` to ensure elements loaded.

6. Extracted:
   - **Clinic Name**: From `h3` tags.
   - **Address**: From `p` tags.
   - **Contact Number**: From anchor tags with "tel:" links.
   - **Website**: From anchor tags with website links.

7.  Implemented logic to navigate to the next page, handling button clicks.

8. **Error Handling**: Managed exceptions for window closures and timeouts.

9.  Compiled the scraped data into a pandas DataFrame.

10.  Used `pd.DataFrame.to_excel()` to save the DataFrame as an Excel file named ----QNS_Clinic detail.xlsx

11  Ensured WebDriver closed properly in the `finally` block.

