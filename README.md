# record-digitization

This github is in reference to Digitization and Data Frames for Card Index Records created by Someswar Amujala (Claremont McKenna College; samujala23@cmc.edu), Sanjiv R. Das (Santa Clara University; srdas@scu.edu), and Angela Vossmeyer (Claremont McKenna College & NBER; angela.vossmeyer@cmc.edu)

We develop a methodology for converting card index archival records into usable dataframes for statistical and textual analyses. Leveraging machine learning and  natural language processing tools from Amazon Web Services (AWS), we overcome hurdles associated with character recognition, inconsistent data reporting, column misalignment, and irregularnaming. This code is aimed to serve as a supplement for the paper which details the step-by-step conversion process and discusses remedies for common problems and edge cases, using historical records from the Reconstruction Finance Corporation.

The code for running the process outlined in the paper are located in "AWS_Code.ipynb".

## Code Instructions:
- The training data used to train the two custom comprehend models are provided in the "Training File" code. 
- The orginal pdf with card images has been uploaded as: "Cards_34.pdf"
- A sample CSV Output has been included within the "Sample CSV Output" folder, named "Cards_34.csv". If implemented correctly, the functions in "AWS_Code.ipynb" should yield an output file that is similar to the given output file. Small discrepencies may exist due to updates in packages and AWS.
- Sample AWS Textract files are also included for your reference. These files do not need to be used in any part of the file. Rather, if for some reason you get a different end CSV output, it may be helpful to compare your textract files to the ones supplied here. 
- The code assumes basic knowledge of AWS textract and AWS Comrephend API. If needed, documentation of these can be found here: 
       -  https://docs.aws.amazon.com/textract/latest/dg/async.html
       -  https://docs.aws.amazon.com/comprehend/latest/dg/functionality.html
       -  https://docs.aws.amazon.com/comprehend/latest/dg/auto-ml.html. 

## Notes:
- The code includes the following sections: Textract, Comprehend, Regex Functions, Combining Regex + Comprehend, and CSV Output
- A majority of these functions are used as helper functions. For parts where the functions need to be called, there will be a subheader starting with "RUN:"
- Similarily, where user input is needed, there will be a subheader starting with "INPUT:" 
- 
