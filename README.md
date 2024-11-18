**Automated Flight Ticket Finder and Email Notification**

This project is built using UiPath to automate the process of searching for the cheapest flight tickets on Traveloka and notifying the user of the best options via email. 

The primary goal is to streamline the manual effort of searching for affordable flights, enabling users to receive top results quickly and accurately without browsing through numerous options.

The bot begins by navigating to the Traveloka website and extracting flight details using UiPath’s Data Scraping functionality. It captures key details such as airline name, ticket price, departure time, and arrival time. To ensure flexibility, the workflow dynamically handles changes in the website’s structure using adaptable selectors. Once the data is extracted, it is stored in a DataTable for further processing.

The data is then processed to identify the cheapest options. The workflow sorts the extracted flight data by price in ascending order using Sort Data Table, and it filters the top N options (e.g., 3 or 5) as per user requirements. During this process, any unnecessary formatting (like “/khách” or “VND” in ticket prices) is removed to maintain clean and accurate data. The workflow also validates the extracted data to handle issues like missing or duplicate entries. The processed data is temporarily stored in an Excel file for backup purposes and is cleared automatically after email delivery.

The notification email is composed with all relevant details such as airline, ticket price, departure and arrival times. Using the Send SMTP Mail Message activity, the bot sends this email to the specified recipient. The email content is formatted in plain text, ensuring readability and clarity. The recipient email address, email subject, and number of flights included in the email can all be configured by the user. This flexibility allows the bot to cater to various preferences and scenarios.

The project uses several technologies to achieve its objectives. UiPath handles the automation of web scraping, data processing, and email sending. Excel is integrated for temporary data storage and acts as a backup system for the extracted flight data. The SMTP email service ensures seamless and secure delivery of notifications. The bot is designed to run reliably, even in cases of minor webpage changes, thanks to its robust selectors and error handling mechanisms.

For future enhancements, this project can be extended to support other travel booking platforms such as Agoda, Expedia, or Skyscanner. Advanced filtering options, like specifying preferred airlines or excluding flights with long layovers, can also be added. Additionally, the project could include a user interface for setting dynamic preferences and options, making it even more user-friendly.

Overall, this project highlights the power of automation in reducing repetitive tasks, improving accuracy, and enhancing user convenience. It serves as a great example of how UiPath can be used to simplify a common process and deliver significant value to its users.
