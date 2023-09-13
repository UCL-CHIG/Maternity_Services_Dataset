# Maternity_Services_Dataset
Maternity Services Dataset (MSDS) v1.5 MySQL set up

MySQL code to import raw data files as received from NHS England

The data covers version 1.5 of the MSDS for four financial years 2015/16 to 2018/19

The data are received as flat tab delimited files (as some fields contain multiple pipe delimited dates) Plus a mother record_id to token person ID bridge file.

Files for each year + the bridge file are initially imported onto the MySQL server. Files for all financial years are then collated in one table. Before the final step of joining the tokenids for mothers from the bridge file into the overall MSDS table.

Indexes are created on the token person IDs to allow linkage to other NHS England datasets.

The data model for version 1.5 of the MSDS is availabe on the national archives website: https://webarchive.nationalarchives.gov.uk/20210104191559/https://digital.nhs.uk/binaries/content/assets/legacy/pdf/6/6/maternity_services_data_set_data_model_v1.5.pdf (although data are received as flat files, not a relational database)

The Technical output specification: https://digital.nhs.uk/binaries/content/assets/website-assets/data-and-information/data-sets/maternity-services/maternity_services_data_set_technical_output_specification_1.8.18.xlsx

User guidance: https://webarchive.nationalarchives.gov.uk/20210104191559/https://digital.nhs.uk/binaries/content/assets/legacy/pdf/6/n/maternity_services_data_set_user_guidance_v3.8.pdf

And technical guidance: https://webarchive.nationalarchives.gov.uk/ukgwa/20211206230532/https://digital.nhs.uk/binaries/content/assets/legacy/pdf/6/7/maternity_services_data_set_technical_guidance.pdf
