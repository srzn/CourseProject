# CourseProject

Project Proposal.pdf is the Project Proposal Document

progressreport.pdf is Project Progress Report as of 11/29/2020 9:00 PM ET
==========For running the code=================

All the software content is in the file Code.zip. When you uncompress Code.zip you'll have two folders - train and test. Please do not delete any file. Important files are illustrated below 

---train---

queryextr.py

uidmap.py

convert-dat1.py

search-eval.py

---test---

queryextr.py

uidmap.py

convert-dat1.py

search_test.py

predictgen.py

====Usage===

If you're skipping the training, run the following from "test" folder on your command prompt:

python search_test.py config-test.toml 'Option'
  
where 'Option' can take any integer value between 0 and 5. Please refer the documentation to know more about each choice. 

For example, if you chose Option 0 then you'll run  

python search_test.py config-test.toml 0

And then run,

python predictgen.py

The above code must be executed to obtain the final predictions in a text file. If you chose Option 0 you would obtain "prediction0.txt" as your final predictions for all the queries capping at 1000 top documents per query.

If you want use the training phase:

From "train" folder, run

python search_eval.py config.toml 'Option'

where 'Option' has the same range as described above. You'll obtain a text file "Option0.txt" (if you chose Option 0). Please copy this file over to the "test" folder and repeat the instructions above to obtain final predictions. 
  
---End
