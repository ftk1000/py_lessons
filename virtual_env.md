2023.11.17

https://platform.openai.com/docs/quickstart?context=python

# Setup a virtual environment (optional)

Once you have Python installed, it is a good practice to create a virtual python environment to install the OpenAI Python library. Virtual environments provide a clean working space for your Python packages to be installed so that you do not have conflicts with other libraries you install for other projects. You are not required to use a virtual environment, so skip to step 3 if you do not want to set one up.
To create a virtual environment, Python supplies a built in venv module which provides the basic functionality needed for the virtual environment setup. Running the command below will create a virtual environment named "openai-env" inside the current folder you have selected in your terminal / command line:

          python -m venv openai-env

Once you’ve created the virtual environment, you need to activate it. On Windows, run:

          openai-env\Scripts\activate

On Unix or MacOS, run:

          source openai-env/bin/activate

You should see the terminal / command line interface change slightly after you active the virtual environment, it should now show "openai-env" to the left of the cursor input section. For more details on working wit virtual environments, please refer to the official 
[Python documentation https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments](https://docs.python.org/3/tutorial/venv.html#creating-virtual-environments).

# =========


# syntax=docker/dockerfile:1
FROM python:3.9


docker build -t my-python .
