# Azure OpenAI Quickstart

Learn how to set up and leverage Azure OpenAI for building intelligent applications. 

## Step 1: Setting Up Azure OpenAI
1. Navigate to the Azure Portal.
2. Create a new Azure OpenAI resource.
3. Follow the [official documentation](https://learn.microsoft.com/en-us/azure/cognitive-services/openai/) for detailed setup instructions.

## Step 2: Use Cases
- Build intelligent chatbots.
- Process large-scale datasets with AI.
- Generate content programmatically.

## Example Script:
```python
import openai

openai.api_key = "your-api-key"

response = openai.Completion.create(
    engine="davinci",
    prompt="Write a short introduction about AI.",
    max_tokens=100
)

print(response.choices[0].text.strip())

