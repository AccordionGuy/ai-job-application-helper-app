# AI Job Application Helper App

![](./images/build_ai_job_application_helper_app.png)

This is a Juypter Notebook created for the Tampa Bay AI Meetup session on Monday, March 17, 2025, where we presented the audience with an application that takes the following...

- The user’s résumé in Markdown format
- A job description

...and generates a new résumé and cover letter that’s fine-tuned to better match the job description.


## How to use this app

### 1. Install Python and Jupyter
To run this application, you need:

- [Python](https://www.python.org/), version 3.8 or later.
- [Jupyter Lab/Notebook(https://jupyter.org/)] or [Visual Studio Code](https://code.visualstudio.com/) with the [Jupyter plugin](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) installed.
- An [OpenAI API account](https://platform.openai.com/docs/overview) and an OpenAI API key, which this application will use.

### 2. Create an `.env` file
This application expects to read your OpenAI API key from an `.env` file located in its base directory. Create this file and enter the following into it...

```
OPENAI_API_KEY={your API key goes here}
```

...and replace `{your API key goes here}` with your API key.

### 3. Create the input files
The application uses two input files:

1. **Your résumé, in Markdown format.** The app expects to find your résumé in its base directory in a file named `reference_resume.md`. I’ve included a version of my own résumé so that you can run the app once you’ve created the `.env` file with your API key. **Replace the contents of this file with your own résumé in Markdown format.**
2. **The job description for the position you’re applying for, in Markdown format.** The app also expects to find a job description in its base directory in a file named `job_description.md`. I’ve included an example job description, and once again, it’s so that you can run the app as quickly as possible without having to find a job description. **Replace the contents of this file with the job description.**

### 4. Run the notebook!
Run the Notebook file — `resume fine-tuner.ipynb` —  by opening it in your Jupyter Notebook-running environment and run each cell.