**Automated Flight Ticket Finder and Email Notification**

This project was developed by me and four of my teammates as a collaborative effort to explore the potential of automation in solving practical problems. The project idea was inspired in part by the video "UiPath | Travel Buddy Robot | Flight Booking Automation Use Case" on YouTube, which provided valuable insights into automating flight-related tasks. Building on this inspiration, our team customized the approach and functionality to focus specifically on identifying and notifying users of the cheapest flight options on Traveloka.

The bot automates the process of navigating the Traveloka website, extracting flight details using UiPath’s Data Scraping functionality, and processing the data to identify the cheapest flight options. Key information captured includes the airline name, ticket price, departure time, and arrival time. To handle potential changes in Traveloka’s website structure, the workflow uses dynamic selectors for robustness and adaptability.

After extracting the data, the bot processes it using UiPath’s Sort Data Table and Filter Data Table activities. It sorts flight ticket prices in ascending order and extracts the top 3 or 5 cheapest flights, based on user requirements. During this process, unnecessary text such as “/khách” or “VND” is removed from the price data for clarity and consistency. The filtered data is temporarily stored in an Excel file for backup purposes, which is automatically cleared after the email is successfully sent.

The email notification is dynamically composed to include all relevant flight details, such as airline name, ticket price (formatted neatly), departure time, and arrival time. The bot uses the Send SMTP Mail Message activity to deliver the email to the specified recipient. The recipient email address, email subject, and number of results included in the email can all be easily configured. This makes the tool flexible and adaptable to various user needs.

Our team’s approach was unique in integrating multiple technologies and workflows. UiPath was the primary tool for automation, handling web scraping, data processing, and email notifications. Excel was used for temporary data storage and served as a backup system for extracted data. The SMTP email service enabled secure and reliable delivery of the notifications. Each team member contributed to the design, implementation, and debugging of various components of the workflow.

The project, while influenced by the mentioned YouTube video, incorporates several enhancements and customizations. For example, our bot includes additional filtering logic, automated Excel clearing, and email formatting tailored to the user’s preferences. In the future, we plan to expand its capabilities to support multiple travel platforms, offer advanced filtering options (e.g., by airline, layovers, or departure times), and provide a user interface for easier configuration.

This project showcases the power of teamwork and automation tools like UiPath to simplify everyday tasks. By combining inspiration from external sources with our own innovations, we created a reliable and efficient solution for flight ticket discovery and notification.

For future enhancements, this project can be extended to support other travel booking platforms such as Agoda, Expedia, or Skyscanner. Advanced filtering options, like specifying preferred airlines or excluding flights with long layovers, can also be added. Additionally, the project could include a user interface for setting dynamic preferences and options, making it even more user-friendly.

Overall, this project highlights the power of automation in reducing repetitive tasks, improving accuracy, and enhancing user convenience. It serves as a great example of how UiPath can be used to simplify a common process and deliver significant value to its users.
This project i
