# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

# Date:30-10-2025
# Register no.212222050061
# Aim: To develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.

#AI Tools Required: 

| S.No | Tool Name                  | Purpose                             |
| :--: | :------------------------- | :---------------------------------- |
|   1  | ChatGPT / OpenAI API       | To process natural language prompts |
|   2  | Python (optional)          | To simulate command-line interface  |
|   3  | Text editor / Google Colab | For writing and testing prompts     |
|   4  | Spreadsheet / Table        | To maintain task records            |



# Explanation: 
Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."
Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.



A prompt-based application uses a Large Language Model (LLM) like ChatGPT to generate intelligent and context-aware responses based on user inputs.
Here, the system acts as a Personal Productivity Assistant that can:

Accept and organize daily tasks.

Schedule reminders.

Suggest health and wellness tips.

Answer user’s general questions.

This exercise demonstrates prompt engineering — how carefully crafted prompts lead to efficient and personalized outputs.

# Prompt:

“Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time.”

# Procedure:

1.Define Core Requirements – Identify functionalities like task management, scheduling, and wellness support.

2.Design Prompts – Frame natural language prompts for each function.

3.Implement Using Python (optional) – Simulate prompt interaction via command line.

4.Test Interactions – Observe how responses vary with different prompt structures.

5.Refine and Document – Record prompts, responses, and performance in tabular form.

# Sample Code Implementation (Python Simulation):

# Personal Productivity Assistant Simulation using ChatGPT API (Example)

import openai

openai.api_key = "your_api_key_here"

def assistant_response(prompt):

    response = openai.ChatCompletion.create(
    
        model="gpt-3.5-turbo",
        
        messages=[{"role": "user", "content": prompt}]
    )
    
    return response["choices"][0]["message"]["content"]
    

# Simulated user interactions

print("Welcome to your AI Personal Assistant!")

while True:

    user_input = input("You: ")
    
    if user_input.lower() in ["exit", "quit"]:
    
        print("Assistant: Goodbye! Have a productive day!")
        
        break
        
    reply = assistant_response(user_input)
    
    print("Assistant:", reply)
    

# Explanation:

The code takes user input and sends it to ChatGPT.
It returns natural-language responses, simulating a productivity chatbot.
The user can exit anytime by typing “exit” or “quit”.

# Tabular Representation of Prompt Design and Output:

| S.No | Feature       | Example Prompt                                                | Example Response (by ChatGPT)                                                  |
| :--: | :------------ | :------------------------------------------------------------ | :----------------------------------------------------------------------------- |
|   1  | Task Manager  | “Add a reminder to pay the electricity bill at 6 PM.”         | “Got it! I’ll remind you at 6 PM to pay your electricity bill.”                |
|   2  | Scheduler     | “Schedule a meeting with the project team tomorrow at 11 AM.” | “Meeting scheduled for tomorrow at 11 AM with your project team.”              |
|   3  | Wellness Tips | “Give me a wellness tip for today.”                           | “Take a 5-minute walk every 2 hours to reduce screen fatigue.”                 |
|   4  | General Query | “What are some time management strategies?”                   | “Try the Pomodoro technique and prioritize tasks using the Eisenhower Matrix.” |
|   5  | Adaptation    | “I prefer wellness tips in the evening.”                      | “Sure! I’ll share your daily wellness tip at 7 PM from now on.”                |

# Expected Output:

A responsive AI assistant capable of:

->Understanding natural language commands.
->Managing and prioritizing tasks.
->Scheduling and reminding events.
->Offering adaptive wellness suggestions.
->Responding conversationally to general queries.

# Example Interaction:

User: “Remind me to complete my lab report by 5 PM.”
Assistant: “Sure! I’ll remind you at 5 PM to complete your lab report.”

User: “Give me a wellness tip for concentration.”
Assistant: “Try the 20-20-20 rule — every 20 minutes, look at something 20 feet away for 20 seconds.”


# Result: 
The lab exercise resulted in the creation of a prototype concept for a personal assistant powered by large language models. Students were able to:
 Understand how to tailor LLM prompts to real-life applications.
 Foster creativity by designing features suited to their personal or academic lives.
 Learn prompt engineering techniques for optimal interaction with AI tools.
 Experience the versatility and utility of generative AI in solving everyday problems.

# Conclusion:

This experiment enhanced the understanding of prompt-based design and AI-driven productivity systems.
By combining creativity with structured prompt design, students successfully developed a conceptual prototype of an intelligent personal assistant.
