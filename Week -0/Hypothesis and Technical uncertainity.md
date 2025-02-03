# Hyposthesis and Technical Uncertainity

## Hypothesis

We now have built a AI powered sentence constructor that helps students learn how to translate english sentences into Japanese sentences along with proper grammar rules of the Japanese Language.

The system acts as guide but doesn't give the full answer to the student we have added this guardrail in our initial prompt as well but noticed that upon constant incorrect responses it tries to give you the answer in a sneaky way. The responses were pretty acqurate since we used a top of the line paid model.

## Technical uncertainity

- **How can AI-Powered Assistant perform a very broad task?**
  AI-powered assistants aren't able to handle such tasks very well as they start to hallucinate so we made a concise prompt that included all the necessary functions our system should perform.

- **Would a very broad task be better performed by dividing it into subtasks with specialized agents?**
  Absoultely, dividing the task into multiple subtasks and then creating specialized agents for them would give us better results.

- **Does using an AI-Powered Assistant make for a good place to rapidly prototype agents?**
  Yes, we can modify and play around wiht an AI-powered assistant to prototype our agents and then use the final prompt in our agent.

- **How could we take the agent we built in an AI-Powered Assistant and reimplement it into a stack that allows for direct integration into our platform?**
  We can use the final prompt that we made in our AI-powered assistant in our agent and then see if the prompt needs changes based on the results of the agent.

- **How much do we have to rework our prompt documents from one AI-Powered Assistant to another?**
  It depends on different AI-powered assistants and the version of the model they are using. Some don't need any changes while some might need the prompt to be re-written entirely.

- **What prompting techniques can we naturally discover working in the confines of an AI-Powered Assistant?**
  We used few-shot prompting in our prototype. We gave a prompt that told the AI-Powered Assistant what system we needed and then gave it a few examples of what the system should and shouldn't do.

- **Are there any interesting innovations unique to specific AI-Powered Assistants for our business goal?**
  The model we used (Gemini 1.5pro-002) is also available in Google AI Studio where we can modify the temprature, add system instructions and even guardrails and integrations with our own system as well.

- **What were we able to achieve based on our AI-Powered Assistant choice and our hardware, or budget limitations?**
  We were able to build a successful prototype of the sentence constructor application that is a part of our gen-ai offerings in our learning platform and the model was available for free using Google AI Studio even though it's a paid model. We used a cloud offering for the prototype and no amount from the budget was used.

## Technical exploration

First we looked at the given examples and then constructed a prompt for our task that included a lot of instructions on what the AI-system should do. Then we tested the system thorughly and found it wokrs fine but it was showing the kanji for the japanese words which we again had to instruct it to stop doing.

It worked pretty well and the outcome was as expected but can be more better with a better prompt and model.
