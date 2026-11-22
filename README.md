# zindi-dischem-product-data-enrichment-challenge
Can you build an AI solution that makes product information more complete, consistent and reliable?

`unlabelled_data.csv`
This file contains 13,864 product records with source information and no expected output labels. The product descriptions and specifications are not masked. Use these records to understand the catalogue and develop an approach that works across products. This file is not a submission file.

`Test_Masked.csv`
This file contains 1,157 records for which you should prepare product content. Some source fields are blank or contain the marker [MASKED]. Keep each record_id unchanged and use it as the corresponding article_id in your submission. The do_not_predict_fields column contains a JSON array of output field names that do not apply to that product. Leave each corresponding submission cell blank. A blank cell is interpreted using that field’s empty value in submission_format.json. For example, a list field becomes [], while an object field uses its defined keys with empty values. Do not enter text such as N/A.

`template_input.csv`
This file contains 14 example product records. It shows the input format used for the test records.

`template.csv`
This file contains the expected structured outputs for the 14 records in template_input.csv. Match template_input.csv rows to this file using record_id and article_id. These are examples for learning the expected structure. Do not include them in your test submission.

`product_enrichment_guardrail.pdf`
This guide explains the content standards for product information. Use it when deciding what to include, how to handle uncertain information, and when to leave a field empty.

`SampleSubmission.csv`
This sample submission shows the required columns and cell format. Treat it as a format example, not as an additional source of product facts.

`columns.docx`
This companion file explains the input and output columns.*

`submission_format.json`
This companion file describes the expected submission columns and the structure of JSON values inside CSV cells.

`product_images.zip`
This archive contains downloadable product images for some records in the input files.

`image_mapping.xlsx`
Use this file to match each record_id to its image filename in product_images.zip. A record with multiple images appears on multiple rows. An empty img_filename means no image for that record is included in the archive.