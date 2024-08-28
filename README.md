# Job Posting JSON-LD Schema

## Overview

This repository contains a JSON-LD schema for structuring job posting data using the Schema.org vocabulary. This structured data helps search engines and other services better understand and display job postings.

## JSON-LD Script

The script provided in this repository uses JSON-LD to mark up job postings on your website. It helps improve the visibility of job listings in search engine results and provides detailed job information.

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "JobPosting",
  "title": {{Title | json}},
  "description": {{Description | json}},
  "identifier": {
    "@type": "PropertyValue",
    "name": "SmartRecruitments",
    "value": "1234567"
  },
  "datePosted": {{datePosted | json}},
  "applicantLocationRequirements": {
    "@type": "Country",
    "name": {{applicantLocationRequirements | json}}
  },
  "jobLocationType": {{jobLocationType | json}},
  "employmentType": {{employmentType | json}},
  "hiringOrganization": {
    "@type": "Organization",
    "name": "SmartRecruitments",
    "sameAs": "https://www.smart-recruitments.com",
    "logo": "https://framerusercontent.com/images/Z4KcBNbbNCdww7assUcUlcOHMz4.png?scale-down-to=512"
  },   
  "jobLocation": {
    "@type": "Place",
    "address": {
      "@type": "PostalAddress",
      "addressLocality": {{City | json}},
      "addressRegion": {{StateProvince | json}},
      "addressCountry": {{Country | json}}
    }
  },
  "baseSalary": {
    "@type": "MonetaryAmount",
    "currency": {{baseSalaryCurrency | json}},
    "value": {
      "@type": "QuantitativeValue",
      "value": {{baseSalary | json}},
      "unitText": "MONTH"
    }
  }
}
</script>
'''md

##Variables
The script contains placeholders for dynamic data. Replace the placeholders with actual values or variables as needed:

{{Title | json}}: The title of the job posting.
{{Description | json}}: A description of the job.
{{datePosted | json}}: The date the job was posted.
{{applicantLocationRequirements | json}}: The location requirement for the job.
{{jobLocationType | json}}: The type of job location (e.g., remote, on-site).
{{employmentType | json}}: The type of employment (e.g., full-time, part-time).
{{City | json}}: The city where the job is located.
{{StateProvince | json}}: The state or province where the job is located.
{{Country | json}}: The country where the job is located.
{{baseSalaryCurrency | json}}: The currency of the base salary.
{{baseSalary | json}}: The base salary amount.
Usage
Add the Script: Place the JSON-LD script within the <head> section of your HTML document.
Replace Placeholders: Substitute the placeholders with actual job posting data.
Validate: Use Google's Structured Data Testing Tool to ensure the JSON-LD markup is correctly implemented.
Contributing
Feel free to open issues or submit pull requests if you have improvements or suggestions. Contributions are welcome!

License
This project is licensed under the MIT License. See the LICENSE file for details.
