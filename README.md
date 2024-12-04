# LLM-Observability---LLM-Regression-Testing

# LLM regression testing 
Regression testing is a quality assurance technique used in software development. It ensures that changes to code don't mess things up.
How does this translate to LLM applications? When you change prompts, models, or retrieval strategies, you still need to test your software: nothing new here. But you also must test the generative part – the one that produces text, code, or content in response to user input. 
And here is the rub: unlike traditional software functions, LLM outputs can have many acceptable answers for the same input. You can't simply look for an exact match for your unit tests. And if you try to describe what makes a good answer, you end up with qualities like "neutral tone" or "relevant response." How do you check for these? 

It starts with the test cases.

Test cases are sample inputs that represent what users do with your application. For a Q&A system, these could be typical questions. You can collect them from real user interactions, write them yourself, or even ask an LLM to brainstorm them. You also need example answers, at least for some inputs. If your app isn't live yet, you can approve or edit some test completions or ask domain experts to do that. 

# Steps of Implementation 

## Step 1 : Import necessary libraries and instantiate Open AI Key

## Step 2 : Setup connection to Evidently Cloud

## Step 3 : Prepare the dataset and do baseline EDA and visualization

![image](https://github.com/user-attachments/assets/1b708194-cc88-4e2f-9046-f5ece3855aab)

![image](https://github.com/user-attachments/assets/a6e0b7ff-684d-4d80-b524-4ab037051d4b)

## Step 4 : Generate new responses

![image](https://github.com/user-attachments/assets/3435d8e0-6166-4418-8e3f-5105f52fd573)

## Step 5 : Design the test suite ( criteria of evaluation )
         a. Length check
         b. Correctness
         c. Style

## Define the following judges : 
         a. Correctness LLM judge : Binary classification ( correct / incorrect ) based on semantic similarity
         b. Style LLM judge 
              Consider the following STYLE attributes:
              - tone (friendly, formal, casual, sarcastic, etc.)
              - sentence structure (simple, compound, complex, etc.)
              - verbosity level (relative length of answers)
              - and other similar attributes that may reflect difference in STYLE.

## Step 6 : Create a test suite

## Step 7 : Run regression test , please find below sample output screenshots

![image](https://github.com/user-attachments/assets/c0cd7ab5-3dad-4687-a75a-dab9ca2f4858)

![image](https://github.com/user-attachments/assets/b404e410-c1b4-4475-957a-8fbd249adad0)

## Step 8 : Log the results in Evidently cloud and explore it

## Step 9 : Change the output response and test again

![image](https://github.com/user-attachments/assets/7f297a0d-16e4-43bc-ba5b-e032be7e772e)

![image](https://github.com/user-attachments/assets/c250c104-cb1b-4266-8bab-48668cdde942)

![image](https://github.com/user-attachments/assets/3222730d-bc75-4b11-91c0-9f350c51aef6)

## Step 10 : Create the dashboards in Evidently cloud

![image](https://github.com/user-attachments/assets/80ebac4a-b8d7-46f5-b893-6b9697768912)

![image](https://github.com/user-attachments/assets/2db189fb-6aa4-407a-addb-fee33deb7a78)











