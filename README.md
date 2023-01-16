# Extended GPT2 Output Detector

The project is currently running at: https://michaelgithubhype.github.io/Extended-GPT2-Output-Detector/
Related blog: TODO 

## Background 
This project extends the [GPT-2 Output Detector](https://github.com/openai/gpt-2-output-dataset/tree/master/detector) made by OpenAI. I added two features on top of the original detector:

* No token limit. This version splits tokens into batches and then computes the average accuracy across the batches. 
* Zip file support. The app can run through multiple submissions and compute a real probability for each one. 



## Disclaimers 

* This project is simply my changes to the GPT-2 Output Detector. You can find out more about how the original project works in the [GitHub repository](https://github.com/openai/gpt-2-output-dataset/tree/master/detector).
* It's possible that splitting the main text into batches would lower the accuracy of the tool in some cases. While this tool is a convenient way to identify potential AI content, you shouldn't blindly rely on this tool. Especially if the subject is students.
* I did not deploy the backend of the program. I am currently simply sending requests in batches to the [GPT-2 Output Detector](https://openai-openai-detector.hf.space/). If that site goes down, this application would also stop working.
* Like the original program, this model only supports text. Submissions that contain code may fail to complete.
