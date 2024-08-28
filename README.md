# Job Posting JSON-LD Schema

## Overview

This repository contains a JSON-LD schema for structuring job posting data using the Schema.org vocabulary. This structured data helps search engines and other services better understand and display job postings.

## JSON-LD Script

The script provided in this repository uses JSON-LD to mark up job postings on your website. It helps improve the visibility of job listings in search engine results and provides detailed job information.

## Variables

The script contains placeholders for dynamic data. Replace the placeholders with actual values or variables as needed:

- `{{Title | json}}`: The title of the job posting.
- `{{Description | json}}`: A description of the job.
- `{{datePosted | json}}`: The date the job was posted.
- `{{applicantLocationRequirements | json}}`: The location requirement for the job.
- `{{jobLocationType | json}}`: The type of job location (e.g., remote, on-site).
- `{{employmentType | json}}`: The type of employment (e.g., full-time, part-time).
- `{{City | json}}`: The city where the job is located.
- `{{StateProvince | json}}`: The state or province where the job is located.
- `{{Country | json}}`: The country where the job is located.
- `{{baseSalaryCurrency | json}}`: The currency of the base salary.
- `{{baseSalary | json}}`: The base salary amount.

## Usage

1. **Add the Script**: Place the JSON-LD script within the `<head>` section of your HTML document.
2. **Replace Placeholders**: Substitute the placeholders with actual job posting data.
3. **Validate**: Use Google's [Structured Data Testing Tool](https://search.google.com/structured-data/testing-tool) to ensure the JSON-LD markup is correctly implemented.

## Contributing

Feel free to open issues or submit pull requests if you have improvements or suggestions. Contributions are welcome!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
