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
