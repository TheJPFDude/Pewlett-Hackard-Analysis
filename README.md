# Pewlett Hackard Analysis

## Overview

The purpose of this analysis was to help a fictional company Pewlett Hackard with creating a SQL database to keep track of employees to prepare for incoming retirements. Queries were also made to analyze the data and help the company prepare for the "silver tsunami".

## Results

From the analysis done, here are some of the findings:

- In total, there are 90,398 employees that will be retiring soon.
- There are many senior employees that will need to be replaced soon, based on the findings from Deliverable 1. Specifically, there are many senior engineeers and staff in particular, with around 57,000 of them to replace.

![Retirement by Title Count](/Images/image1.png)

- The good news is that there are only two managers to replace.
- There are 1,940 employees eligible for mentorship.

## Summary

- How many roles will need to be filled as the "silver tsunami" begins to make an impact?

As mentioned above, there are 90,398 roles that will need to be filled in the future. The query executed to get this information was `SELECT SUM(count) FROM retiring_titles;`

- Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

As there are 1,940 qualiied employees for mentorship to mentor the 90,000-ish roles that will be vacated, there are most likely not enough employees to mentor the next generation. The query exectued to get this information was `SELECT COUNT(*) FROM mentorship_eligibility;`
