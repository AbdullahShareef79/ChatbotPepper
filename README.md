# ChatbotSample

ChatbotSample is an Android application for **Pepper the Robot** that demonstrates how to implement a chatbot using the **Android QiSDK**. This project combines a local **qichatbot** and an online **Dialogflow** agent to enable Pepper to engage in structured and casual conversations effectively.

## Project Overview
This project showcases a hybrid chatbot for Pepper Robot, leveraging local qichatbot capabilities for robot-specific interactions and an online Dialogflow agent for general queries. The chatbot demonstrates structured dialogues aligned with a functional scenario and casual discussions for broader engagement.

## Features
- **Local QiChatbot**: Handles Pepper-specific conversations, including robot information and simple actions.
- **Dialogflow Integration**: Manages general inquiries not covered by qichatbot.
- **Hybrid Chat Engine**: Ensures seamless transition between structured and open-ended dialogues.
- **Interactive Behavior**: Pepper uses speech, gestures, and visual outputs for a dynamic experience.
- **Customizable Intents**: Adapt both chatbots to fit specific application needs.

## Minimum Configuration
- **Pepper Robot SDK 2.9**
- **API Level 3**

## Getting Started
### Dialogflow Agent Setup
This sample uses a **Dialogflow v1 agent**. To run the application, you need to set up your own agent via the Dialogflow console (https://console.dialogflow.com).

#### Creating a Dialogflow Agent
1. Log in to the Dialogflow console.
2. Create a new agent and ensure the *V1 API* is selected in the *General* tab under settings.

#### Client Access Token
Add your Dialogflow agent’s **client access token** to the Android project:
1. Locate the **global gradle.properties** file in your *~/.gradle* folder.
2. Add the following line:
   ```
   CHATBOT_SAMPLE_DIALOGFLOW_TOKEN=your_client_access_token
   ```
   This keeps the token secure and out of version control.

### Populating the Dialogflow Agent
You can populate your Dialogflow agent manually or import a predefined agent.

#### Importing the Sample Agent
1. Open your Dialogflow agent settings.
2. Select *Export and Import* > *Restore from zip*.
3. Follow the instructions to upload the provided [DialogflowChatbotAgent.zip] file.

This sample agent includes fallback intents for responding to general questions.

## Project Structure
- **/src**: Contains Java source code for integrating and managing the hybrid chatbot.
- **/res**: Resources such as layouts, strings, and drawable assets.
- **/docs**: Documentation and usage guides.
- **/tests**: Automated tests for chatbot reliability.

## Additional Resources
### UML Diagrams
- [Class Diagram](classDiagram.plantuml): Provides an overview of the application’s structure.
- [Sequence Diagram](sequenceDiagram.plantuml): Illustrates the flow of interactions.

You can view these diagrams using the *PlantUML integration* plugin in Android Studio or via http://www.plantuml.com/plantuml.

## Future Enhancements
- **Enhanced Natural Language Understanding**: Upgrade to Dialogflow v2 for advanced capabilities.
- **Personalized Conversations**: Add user profiling for more tailored responses.
- **Advanced Analytics**: Implement logging and analytics for monitoring chatbot interactions.

## Contribution
Contributions are welcome! If you’d like to contribute:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Submit a pull request with a detailed description of changes and testing results.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For questions, suggestions, or collaboration inquiries, please contact:
- **Developer**: Abdullah Shareef
- **Email**: abdullahshareef7945512@gmail.com

---
**University of Trier | Pepper Robot Project | ChatbotSample**

