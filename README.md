<h1>
    <img src="./public/favicon.ico" alt="Data Formulator icon" width="28"> <b>Data Formulator: Create Rich Visualizations with AI</b>
</h1>

<div>
    

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)&ensp;
[![YouTube](https://img.shields.io/badge/YouTube-white?logo=youtube&logoColor=%23FF0000)](https://youtu.be/3ndlwt0Wi3c)&ensp;
[![build](https://github.com/microsoft/data-formulator/actions/workflows/python-build.yml/badge.svg)](https://github.com/microsoft/data-formulator/actions/workflows/python-build.yml)


</div>

Transform data and create rich visualizations iteratively with AI 🪄. Try Data Formulator now!

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/microsoft/data-formulator?quickstart=1)

<kbd>
  <a target="_blank" rel="noopener noreferrer" href="https://codespaces.new/microsoft/data-formulator?quickstart=1" title="open Data Formulator in GitHub Codespaces"><img src="public/data-formulator-screenshot.png"></a>
</kbd>

## Overview


Data Formulator is an AI-powered tool for analysts to iteratively create rich visualizations. Unlike most chat-based AI tools where users need to describe everything in natural language, Data Formulator combines *user interface interactions (UI)* and *natural language (NL) inputs* for easier interaction. This blended approach makes it easier for users to describe their chart designs while delegating data transformation to AI. 

## Get Started

Play with Data Formulator with one of the following options:

- **Option 1: Install via Python PIP**
  
  Use Python PIP for an easy setup experience, running locally (recommend: install it in a virtual environment).
  
  ```bash
  # install data_formulator
  pip install data_formulator

  # start data_formulator
  data_formulator 
  
  # alternatively, you can run data formulator with this command
  python -m data_formulator
  ```

  Data Formulator will be automatically opened in the browser at [http://localhost:5000](http://localhost:5000).

  *Update: you can specify the port number (e.g., 8080) by `python -m data_formulator --port 8080` if the default port is occupied.*

- **Option 2: Codespaces (5 minutes)**
  
  You can also run Data Formulator in Codespaces; we have everything pre-configured. For more details, see [CODESPACES.md](CODESPACES.md).
  
  [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/microsoft/data-formulator?quickstart=1)

- **Option 3: Working in the developer mode**
  
  You can build Data Formulator locally if you prefer full control over your development environment and the ability to customize the setup to your specific needs. For detailed instructions, refer to [DEVELOPMENT.md](DEVELOPMENT.md).


## Using Data Formulator

Once you've completed the setup using either option, follow these steps to start using Data Formulator:

### The basics of data visualization
* Provide OpenAI keys and select a model (GPT-4o suggested) and choose a dataset.
* Choose a chart type, and then drag-and-drop data fields to chart properties (x, y, color, ...) to specify visual encodings.

https://github.com/user-attachments/assets/0fbea012-1d2d-46c3-a923-b1fc5eb5e5b8


### Create visualization beyond the initial dataset (powered by 🤖)
* You can type names of **fields that do not exist in current data** in the encoding shelf:
    - this tells Data Formulator that you want to create visualizations that require computation or transformation from existing data,
    - you can optionally provide a natural language prompt to explain and clarify your intent (not necessary when field names are self-explanatory).
* Click the **Formulate** button.
    - Data Formulator will transform data and instantiate the visualization based on the encoding and prompt.
* Inspect the data, chart and code.
* To create a new chart based on existing ones, follow up in natural language:
    - provide a follow up prompt (e.g., *``show only top 5!''*),
    - you may also update visual encodings for the new chart.

https://github.com/user-attachments/assets/160c69d2-f42d-435c-9ff3-b1229b5bddba

https://github.com/user-attachments/assets/c93b3e84-8ca8-49ae-80ea-f91ceef34acb

Repeat this process as needed to explore and understand your data. Your explorations are trackable in the **Data Threads** panel. 




