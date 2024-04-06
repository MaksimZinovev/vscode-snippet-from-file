
# VS Code Prompt Snippet Editor 📝  

Add you text files with AI prompts to VS Code snippets. 
  
## Naming Conventions

Use case 1

`/prompt/output/minimal`

I want to insert

- complete prompt template

So that I can

- reuse it as is or make minor changes

Use case 2

`&template/output/minimal`

I want to insert

- blank prompt template

So that I can

- add all details from scratch

Use case 3

`$block/output/minimal`

I want to insert

- a building block

So that I can

- build complete prompt faster

## Structure

Top 5 building blocks

1. Prompt
   1. Prefix: "/"
   2. Title example: "text/create_summary"
   3. Description: A complete prompt template.
2. Identity and Purpose
   1. Prefix: "@"
   2. Title example: "text/expert at interpreting, answering"
   3. Description: Standard block of prompt containing description of assistant's identity and purpose. Character description.
   4. Allowed values. See below in "Identity and Purpose (Characters)" section
3. Steps
   1. Prefix: "#"
   2. Title example: "summarize/Create short summary in 3-5 Markdown bullets of 10 words each"
   3. Description: Standard block of prompt containing description of assistant's identity and purpose. Character description.
   4. Allowed values. See below in "Task Types"
4. Output Instructions
   1. Prefix: "$"
   2. Title example: "bullets/bullets"
   3. Description: Standard block of prompt containing description of output instructions.
5. Techniques
   1. Prefix: "%"
   2. Title example: "Create short summary in 3-5 Markdown bullets of 10 words each"
   3. Description: Standard block of prompt containing description of assistant's identity and purpose. Character description.

## Identity and Purpose (Characters)

1. AI Art
2. Business
3. Social Media
4. Music
5. Video
6. Writing
7. Gaming
8. Education
9. Finance
10. Productivity
11. Humor
12. Travel
13. Food & Drink
14. Developer Tools
15. Design
16. Health & Fitness
17. Philosophy & Self-Improvement
18. Security
19. Lifestyle
20. News
21. Reference
22. Sports
23. Chat
24. CustomGPTs Security
25. Contributing

## Task Types (Steps)

1. Analyze
2. Check
3. Clean
4. Compare
5. Create
6. Explain
7. Extract
8. Find
9. Improve
10. Classify, label and rate
11. Rate
12. Summarize
13. Write
14. Code
15. Evaluate
16. Generate image
17. Mathematics
18. Answer question
19. Reason

## Output Instructions  

1. Markdown bullets
2. Markdown table
3. Numbered list
4. Short paragraph. Max 150 characters including spaces.
5. Medium length paragraph. Max 250 characters including spaces.
6. Large paragraph. Max 500 characters including spaces.
7. Two paragraphs. Each paragraph max 200 characters including spaces.

## Techniques

1. Zero-shot Prompting
2. Few-shot Prompting
3. Chain-of-Thought Prompting
4. Self-Consistency
5. Generate Knowledge Prompting
6. Prompt Chaining
7. Tree of Thoughts
8. Retrieval Augmented Generation
9. Automatic Reasoning and Tool-use
10. Automatic Prompt Engineer
11. Active-Prompt
12. Directional Stimulus Prompting
13. Program-Aided Language Models
14. ReAct
15. Reflexion
16. Multimodal CoT
17. Graph Prompting

## Roadmap

- [ ] Fork extension `snippet-from-file`
- [ ] Rename extension to `prompt-snippet-editor`
- [ ] Install and run extension
- [ ] Command: `Prompt Snippet Editor: Add active file as snippet`
- [ ] Command: `Prompt Snippet Editor: Add file to Curated`
- [ ] Command: `Prompt Snippet Editor: Parse file as prompt`
- [ ] Command: `Prompt Snippet Editor: Parse file as block`
- [ ] Command: `Prompt Snippet Editor: Edit tags`
- [ ] Each prompt has multiple tags/labels. Snippets can be invoked from command pallette by typing tag(s) name.

Explanation 

1. Curated: verified that folder with prompt follows naming conventions. 
2. Parsed: parses file as 
   1. prompt: verifies that file is not empty. 
   2. block: verifies that file is structured. 
3. Added to snippets. Reference to file and title are added to `snippets.json`. Correct prefixes are added automatically as per naming conventions. 
4. 

## Get Started 🚀  

  To get started, hit the 'clear' button at the top of the editor!  
  
## Prebuilt Components/Templates 🔥  

  You can checkout prebuilt components and templates by clicking on the 'Add Section' button or menu icon
  on the top left corner of the navbar.

## Save Readme ✨  

  Once you're done, click on the save button to download and save your ReadMe!
  
# Project Title  

This is an example ReadMe with light selections.  

## Run Locally  

Clone the project  

~~~bash  
  git clone https://link-to-project
~~~

Go to the project directory  

~~~bash  
  cd my-project
~~~

Install dependencies  

~~~bash  
npm install
~~~

Start the server  

~~~bash  
npm run start
~~~

## Contributing  

Contributions are always welcome!  

See `contributing.md` for ways to get started.  

Please adhere to this project's `code of conduct`.  

## License  

[MIT](https://choosealicense.com/licenses/mit/)

## Badges  

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)  
[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://choosealicense.com/licenses/gpl-3.0/)  
[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](https://choosealicense.com/licenses/gpl-3.0/)  

## Demo  

Insert gif or link to demo  

## Features  

- Accessibility in VS Code  
- Download directly to project root  
- Live Previews

## License  

[MIT](https://choosealicense.com/licenses/mit/)  

## Run Locally  

Clone the project  

~~~bash  
  git clone https://link-to-project
~~~

Go to the project directory  

~~~bash  
  cd my-project
~~~

Install dependencies  

~~~bash  
npm install
~~~

Start the server  

~~~bash  
npm run start
~~~

## Test  

# IDENTITY and PURPOSE

You are a helpful code assistant that can teach a junior developer how to code. Your language of choice is JavaScript.

# STEPS

1. Start from brief explanation of what the code does (no more than 25 words)
2. When the code is more than 10 lines, break down the code into smaller logical parts and explain each part to a beginner programmer.
3. Insert empty line between paragraph explanation for each logical part.
4. Follow my instruction precisely.
5. Explain each code line. Print that line in a code block. Then on a new line print explanation
6. Be specific and ask for confirmation if the answer is clear before proceeding to the next part. If you need more information or encounter difficulties in explaining, please inform me.
7. Keep explanation for each logical part within 50 words and use simple explanations for complex concepts.
8. You can use code snippets in your explanation.
9. Be helpful and ensure the beginner's understanding.
10. Only explain provided code.
11. The final paragraph should be summary, no more than 70 words

# OUTPUT INSTRUCTIONS

1. Format and structure your response using the sample response below.
2. Format you answer as a markdown.

Sample response:

```markdown
The code you provided is written in Python and seems to be setting up imports and  the logging configuration for a Streamlit application. Let me break it down for you:

1. **Imports**: This part of the code imports various Python libraries and modules that will be used in the application. Here's what each import does:
   
`import logging`

Imports the Python standard library's logging module, which allows you to log messages, warnings, and errors.

`import sys`

Imports the sys module, which provides access to some variables used or maintained by the interpreter and functions that interact with the interpreter.

2. **Log Configuration**: This section configures the logging for the application. It sets the format for log messages and the log level.

`log_format = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"`
This variable defines the format for log messages. It includes placeholders like `%(asctime)`, `%(name)`, `%(levelname)`, and `%(message)` to format the log messages with the timestamp, logger name, log level, and the actual log message content.


In summary, this code sets up logging for a Streamlit application, allowing the application to log messages with a specified format and level. This is useful for debugging and monitoring the application's behavior. It's important to note that this code snippet is just the setup; it doesn't contain the main logic of the Streamlit application. The actual application logic would be found in other parts of the code.
```

# INPUT

Explain the code  to a beginner programmer.
Below are my instructions. Let me know if my instructions are clear and ask me to provide the code.
