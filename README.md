# Cucumber-ai Example

## Preparation

### Clone the repository
```bash
git clone https://github.com/zbcjakson/cucumber-ai-example.git
```
### Install dependencies
```bash
cd cucumber-ai-example
pnpm install
```
### Set up environment variables
Create a `.env` file in the root directory of the project and add your API keys and model names. Two models need to be set: a model (Recommend a VLM) used by Midscence to interact with the browser; a LLM model for other agents. Here is an example of what your `.env` file should look like:
```dotenv
#Midscence
OPENAI_API_KEY=YOUR_API_KEY_FOR_MIDSCENE
OPENAI_BASE_URL=https://openrouter.ai/api/v1
MIDSCENE_MODEL_NAME=qwen/qwen2.5-vl-72b-instruct  #Strongly recommend to use visual language model
MIDSCENE_USE_QWEN_VL=1

#LLM
LLM_API_KEY=YOUR_API_KEY_FOR_LLM
LLM_BASE_URL=https://openrouter.ai/api/v1
LLM_MODEL_NAME=openai/gpt-4o
```

## Run the example
```bash
pnpm cucumber-ai
```