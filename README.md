# Turf_Scrapping
This project focuses on the automated extraction and structuring of horse racing data from the Hipódromo de Palermo, aiming to build a solid foundation for future analysis or development. It combines techniques such as web scraping, DataFrame handling, PDF document processing, and data export to reusable formats like CSV and Excel.

_What does this program do?_

* **Web Scraping of Completed Races:**
The system iterates over a range of IDs on the official website of the Hipódromo de Palermo (https://www.palermo.com.ar/es/turf/ver-carrera/{ID}), extracting detailed information about each completed race. The data is parsed, cleaned, and stored in a structured format. This robust web page parsing allows raw race data (HTML) to be transformed into usable records.

* **Processing of Upcoming Races from PDFs:**
It uses specific coordinates to read designated sections of PDF files that contain schedules of upcoming races. This automated reading extracts information such as race entries, participating horses, and schedules—without manual intervention—by directly accessing predefined sections within the PDF.

* **Data Export to Excel:**
In addition to CSV and TXT storage, the program includes functionality to convert the generated databases into Excel format (.xlsx), making them easier to use in administrative environments or for quick reference.

* **Process Control and Error Tolerance:**
The system saves backups, logs errors, and allows the user to decide whether to retry downloading failed races. It also implements flags to ensure continuity of the process in the event of connection issues or other transient errors, and automatically triggers the recovery process on the next execution—guaranteeing data consistency.

**IMPORTANT**: In the version containing example data, please note that the database will not match the existing txt files, this is due to GitHub upload limitations, as there are more than 4000 txt files that should be uploaded to the repository in order to match the database.
