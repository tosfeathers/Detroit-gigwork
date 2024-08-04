### Introduction

This was a project for the Columbia University Graduate School of Journalism's Lede Program. It uses undocumented APIs to gather data about gigworkers on Care.com and Taskrabbit and demonstrate that gigworkers who care for seniors and people with special needs often make less than workers performing other tasks, such as cleaning or waiting in lines.

### Methodology

I found undocumented APIs on Care.com and Taskrabbit that allowed me to gather data about how much individual workers charged for different tasks, and in the case of Care.com, how many hours per week they were available for work.

I wanted to examine how the hourly rates for gigwork might differ based on the neighborhood in which the work was performed, so I gathered a random sample of 200 addresses in Detroit using the [United States Places Sampler](https://usps.biglocalnews.org/).

To gather the data, I created functions based on the undocumented Care.com and Taskrabbit APIs that simulated an employer searching for a gigworker. I used those functions to gather hourly wage data for cleaning and waiting in line tasks from Taskrabbit at each of the 200 addresses and for senior care, special needs care, and pet care jobs on Care.com.

The data returned from the Care.com API needed to be cleaned to convert it from string like "$20-35/hr" into a more useable format, so I created nested functions that cleaned the API responses and calculated the median hourly rate for jobs at each address and median number of hours worked by the gigworkers available at each address.

Charts were made using Datawrapper.
