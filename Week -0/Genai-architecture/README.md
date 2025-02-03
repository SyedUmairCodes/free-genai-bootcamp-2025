# Architecture of the App

## Functional Requirements

The company wants to host the AI models and related services on their own infrastructure due to the following factors:

- They possess high-performance hardware that can effectively support the required computational loads.
- Self-hosting provides significant cost advantages compared to managed services, especially at scale.
- Given their user base includes minors (students under 18), they must maintain strict data privacy controls, including COPPA compliance in the US and GDPR requirements for European users.

## Assumptions

We are assuming that training the foundation model takes around 10-15k alone. Since we already the hardware we just need to fine-tune the model for our usecase and we should be good to go.

Updates and further fine-tuning will be handled by the internal team as they will mostly be computational rather than financial.

The self-hosted approach that the company has choosen is likely to break-even within 12-18 months as compared to using a managed service.

## Data Strategy

The data approach focuses on:

- Utilizing carefully vetted open-source educational materials and datasets
- Implementing a three-stage content verification process:

  - Copyright clearance
  - Educational appropriateness assessment
  - Bias and accuracy review

- Creating synthetic training data when needed to fill gaps
- Maintaining clear documentation of all data sources and usage rights
- Regular audits of training data to ensure continued compliance

## Considerations

We are considering using the LLama 3.3 foundation model from Meta AI since our hardware can support the 70B parameter version we can fine-tune it and run it locally using Ollama or LMStudio. It should give us the same performance as LLama 3.1 450B parameter one but at a lower cost.

We are also condidering adding calendar functionality to the main system as well. This will allow students to keep track of their assignments and tasks easily.

We can use google-calendar or other options and enable two-way sync between our system and the calendar for self-study purposes as well.
