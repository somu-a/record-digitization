# record-digitization

This GitHub is in reference to the article “Digitization and Data Frames for Card Index Records” by Someswar Amujala (Claremont McKenna College; samujala23@cmc.edu), Sanjiv R. Das (Santa Clara University; srdas@scu.edu), and Angela Vossmeyer (Claremont McKenna College & NBER; angela.vossmeyer@cmc.edu).
We develop a methodology for converting card index archival records into usable data frames for statistical and textual analyses. Leveraging machine learning and natural language processing tools from Amazon Web Services (AWS), we overcome hurdles associated with character recognition, inconsistent data reporting, column misalignment, and irregular naming. This code is aimed to serve as a supplement for the paper which details the step-by-step conversion process and discusses remedies for common problems and edge cases, using historical records from the Reconstruction Finance Corporation.


## File Details:
- AWS_Code.ipynb is the main coding file.
- Cards_34.pdf is a sample of RFC card index records to be converted with this code.
- The “Training” subfolder contains the text and CSV files necessary to train the two custom Comprehend models.
- The “Sample CSV Output” subfolder contains the final CSV output that is associated with Cards_34.pdf. If implemented correctly, the functions in AWS_Code.ipynb should yield an output file that is similar to Card_34.csv. Small discrepancies may exist due to updates in packages and AWS.
- The "Sample Textract Files" subfolder contains the Textract-produced text files that are associated with the Cards_34.pdf and the Cards_34.csv. 
- Detailed_Instructions.pdf provides step-by-step instructions on how to execute the code.
- VossmeyerAmujalaDas_EXEH.pdf is the academic article associated with this project. 


## Notes:
- The code includes the following sections: Textract, Comprehend, Regex Functions, Combining Regex + Comprehend, and CSV Output.
- The sections of the code that require user input are labeled with an “INPUT” subheader.
- The functions that need to be called are labeled with a "RUN" subheader. Most of the functions in the code are helper functions and do not need to be called (though they need to be compiled). 
- The code assumes basic knowledge of AWS Textract and AWS Comrephend API. If needed, documentation of these can be found here:
       - https://docs.aws.amazon.com/textract/latest/dg/async.html
       - https://docs.aws.amazon.com/comprehend/latest/dg/functionality.html
       - https://docs.aws.amazon.com/comprehend/latest/dg/auto-ml.html.

