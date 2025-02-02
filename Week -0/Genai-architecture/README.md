# Architecture of the App

## Functional Requirements

The company wants to host the AI models and related services on their own infrastructure. They have hardware available that is more than capable and they also want to save costs by not using a managed service. Lastly, they are also worried about the privacy of their user data since most of the users are students, they might be under 18 so data privacy is a must for them.

## Assumptions

We are assuming that training the foundation model takes around 10-15k alone. Since we already the hardware we just need to fine-tune the model for our usecase and we should be good to go.

## Considerations

We are considering using the LLama 3.3 foundation model from Meta AI since our hardware can support the 70B parameter version we can fine-tune it and run it locally using Ollama or LMStudio. It should give us the same performance as LLama 3.1 450B parameter one but at a lower cost.
