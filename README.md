# MyDetective

## Overview
Welcome to MyDetective, our innovative solution presented at natHacks 2023! Aimed at revolutionizing security interviews, such as suspect interrogations in police investigations, MyDetective leverages advanced AI technologies to assist interviewers. This README details the program flow, technology rationale, relevance, and team roles.

## Program Flow and Technology Rationale
Our program uses various AI technologies, each chosen for its specific strengths and capabilities:

1. **Question Generation with GPT-4**:
   - Background information of the interviewee is inputted into OpenAI's GPT-4.
   - **Why GPT-4?**: GPT-4, with its advanced natural language understanding, can generate contextually relevant and strategically insightful questions. It assists interviewers by providing tailored questions that might uncover crucial information based on the interviewee's background.

2. **Data Analysis During Interview**:
   - **Facial Expression Analysis with DeepFace API**: Analyzes interviewee's facial expressions to identify emotions.
   - **Speech Recognition and Analysis**: Google's speech recognition API transcribes the interviewee's responses. The `MoritzLaurer/DeBerta-v3-base-mnli-fever-anli` model classifies the speech into emotions.
   - **EEG Data Analysis**: A random forest model analyzes EEG data, classifying it into emotional states. Brainflow library connects the EEG machine to the computer.
   - **Why These Technologies?**: They provide a multi-faceted analysis of the interviewee's responses, capturing not just what is said, but how it's said and the accompanying emotional and physiological responses. This comprehensive analysis can reveal discrepancies or nuances in responses that might not be evident from speech alone.

3. **Dynamic Questioning with GPT-4**:
   - Integrates transcription, emotional data from facial expressions, NLP analysis, and EEG data.
   - GPT-4 then suggests the next question, dynamically adapting to the interviewee's responses and state.

4. **Iterative Process**:
   - This process repeats, ensuring a thorough and adaptive interview.

## Relevance of the Project
Understanding the truthfulness and emotions of an interviewee is crucial in security interviews for several reasons:
- **Accuracy**: Detecting deception or stress can be vital in ascertaining the truth, especially in critical situations like criminal investigations.
- **Efficiency**: Quickly identifying key emotional responses can guide interviewers to focus on pertinent areas, saving time and resources.
- **Psychological Insights**: Emotional and physiological data provide deeper insights into the interviewee's mindset, potentially revealing motives or hidden feelings.

## Technologies Used

- **Python**: Mainly for data science tasks.
- **React.js**: For building the web interface.
- **Socket.IO and Amazon EC2**: For robust, real-time client communication and server infrastructure.

## Front-end and Data Visualization

- Real-time visualization of emotional states and brainwave data, enhancing the interviewer's understanding and decision-making.

## Communication and Server Setup

- Ensures dynamic, secure, and efficient data handling and communication between applications.

## Team and Roles

- **Joshua Tablan**: Hardware Specialist
- **Dohyun Kim**: Full Stack Developer
- **Yongbin Kim**: Frontend Developer
- **Minjae Jeong**: Backend Developer
- **Jamie Lee**: Data Scientist
- **Taekwan Yoon**: Data Scientist

---

MyDetective is a testament to the power of AI in enhancing critical processes like security interviews. By integrating advanced technologies, we aim to improve the accuracy, efficiency, and depth of investigative interviews.
