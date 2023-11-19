# MyDetective

<div align="center">
   <img src="https://cdn.discordapp.com/attachments/1156344075134451816/1175586513954812054/DALLE_2023-11-16_15.33.53_-_Logo_design_for_MyDetective_app_integrating_EEG_device_and_interrogation_themes._The_logo_features_a_brainwave_pattern_symbolizing_EEG_intertwined.png?ex=656bc542&is=65595042&hm=d07321e02b1a8b9f4b5db06c801d4cdebbb35004b09985fc0296a2670de22ec6&" width="300">
</div>

## Overview
Welcome to MyDetective, an innovative project presented at natHacks 2023! Designed to revolutionize security interviews, such as suspect interrogations in police investigations, our program integrates advanced AI technologies to assist interviewers. This README provides a comprehensive overview of the program's flow, technology rationale, relevance, and our team's roles.

## Program Flow and Technology Rationale
Our program harnesses various AI technologies, each chosen for its specific capabilities:

1. **Question Generation with GPT-4**:
   - Background information of the interviewee is inputted into OpenAI's GPT-4.
   - **Why GPT-4?**: GPT-4's advanced language understanding generates contextually relevant and strategic questions, providing interviewers with tailored queries based on the interviewee's background.

<div align="center">
   <img src=./README_img/gpt_example.png width="100%" height="auto">
</div>

2. **Data Analysis During Interview**:
   - **Facial Expression Analysis with DeepFace API**: Analyzes interviewee's facial expressions to identify emotions.

<div align="center">
   <img src="https://raw.githubusercontent.com/serengil/deepface/master/icon/stock-2.jpg" width="100%" height="auto">
</div>

   - **Speech Recognition and Analysis**: Google's speech recognition API transcribes responses. The `MoritzLaurer/DeBerta-v3-base-mnli-fever-anli` model classifies the speech into emotions.
   - **EEG Data Analysis**: A random forest model analyzes EEG data to determine whether the interviewee is lying or not. Brainflow library connects the EEG machine to the computer.
     <img width="1233" alt="Screenshot 2023-11-18 at 11 52 07 PM" src="https://github.com/KREATORS-2-0/MyDetective/assets/97474786/6f4e7897-ea79-4394-8566-674385724dd1">

   - **Why These Technologies?**: They enable a comprehensive analysis of the interviewee's responses, capturing verbal, emotional, and physiological reactions to reveal nuances and discrepancies.

3. **Dynamic Questioning with GPT-4**:
   - Integrates transcription, emotional data from facial expressions, NLP analysis, and EEG data.
   - GPT-4 suggests the next question, dynamically adapting to the interviewee's state.

<div align="center">
   <img src=./README_img/gpt_example2.png width="100%" height="auto">
</div>

4. **Iterative Process**:
   - Repeats steps 2 and 3 for a thorough, adaptive interview.

## Significance of Multi-Dimensional Analysis
- **Facial Expression Analysis**: Immediate emotional indicators providing insights into involuntary emotional responses.
- **Speech Analysis (NLP Zero-Shot-Classification)**: Uncovers underlying emotions within the spoken content, offering a deeper understanding beyond literal words.
  
<div align="center">
   <img src=./README_img/zero-shot-classification.png width="100%" height="auto">
</div>

- **EEG Analysis**: Trained to classify if a person is lying, providing a direct assessment of truthfulness, a critical factor in security interviews.
<div align="center">
   <img width="100% height="auto" src="https://github.com/KREATORS-2-0/MyDetective/assets/97474786/d4584d52-a310-4a77-9ad2-d6581bce028a">
</div>
## Relevance of the Project
- **Accuracy**: Detecting lies or stress is vital in ascertaining truth in critical situations like criminal investigations.
- **Efficiency**: Quickly identifying key emotional responses guides interviewers to focus on pertinent areas.
- **Psychological Insights**: Provides deeper insights into motives or hidden feelings.

## Technologies Used
- **Python**: Primarily for data science tasks.
- **React.js**: For the web interface.
- **Socket.IO and Amazon EC2**: For real-time communication and robust server infrastructure.

## Front-end and Data Visualization
- Visualizes emotional states and brainwave data in real-time, enhancing interviewer understanding and decision-making.

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

MyDetective is a testament to the power of AI in enhancing critical processes like security interviews. Our integration of advanced technologies aims to improve accuracy, efficiency, and depth in investigative interviews.
