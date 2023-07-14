Problem Statement: Develop a program to detect and prevent self-harm behaviour
Sub-Problems: Depression, Anxiety and Trauma
Sub-Solution : Seek profession help, develop a safety plan and reach out to a support network.
User input :
•	Obtain user input to gather information about their emotions and mental state
•	Analyze the input to identify potential triggers for self-harm
•	Define Variables :
•	userInput(string): stores the input provided by the user.
•	Triggers(list): stores the identified triggers for self-harm.
•	Is harmful(Boolean): indicates if the user input contains harmful content
FUNCTIONS FOR USER INPUT
#The below functions show how the application shall use userinput< analyses it for potential triggers of self-harm and returns a Boolean value indication if the input contains harmful content:
def detect_self_harm(user_input):
triggers = [“self-harm”, “suicide,”hurt myself, “cutting, “end it all”]# example of the list of triggers
#convert user input to lowercase for case-insensitive matching
User_input = user_input.lower()
# Check if any triggers are present in the user input
For trigger in triggers:
If trigger in user_input:
Return true # Harmful content detected
Return False # no harmful content detected

user_input = input("How are you feeling today? ")

if detect_self_harm(user_input):
print("Warning: Your input contains potential triggers for self-harm.")
# Take appropriate actions, such as alerting a caregiver or providing resources for help
else:
print("No harmful content detected. Stay strong and reach out for support if needed.")
you can use this function as part of a larger program to detect and prevent self-harm behaviour. After obtaining the users input, you can call this function to check if it contains any triggers.
B)Control Structures:
i) Conditional:
•	Use and if- else statement to check if the user input contains harmful keywords or phrases.
•	If harmful content is detected, the set is harmful to True and adds identified triggers to the triggers list.
ii) Iterative:
-	Implement a log(such as a for loop) to iterate over the harmfulKeywords list and check if each keyword exists in the user input.

iii) Conditional:
-Use a switch-case statement to handle specific actions based on the severity of harmful content detected.
-Actions can include providing immediate support resources or contacting a designated emergency contact.
FUNCTION FOR CONDITIONAL and ITERATIVE
# Control Structures
# Conditional
if any(keyword in userInput for keyword in harmfulKeywords):
isHarmful = True
triggers = [keyword for keyword in harmfulKeywords if keyword in userInput]

# Print the results
print("Is harmful:", isHarmful)
print("Triggers:", triggers)

# Control Structures
# Iterative
for keyword in harmfulKeywords:
if keyword in userInput:
isHarmful = True
triggers.append(keyword)
break

2. Emotional support
- Provide emotional support and resources to the user based on their reported emotions and mental state.
Variables:
-emotions(list): stores the users reported emotions.
- mental state(string): indicates the user’s reported mental state.
-support message(string): stores the message containing emotional support and resources.
B)Control Structures:
i) Conditional:
-Use an if-else statement to check the user’s reported mental state and provide appropriate support.

ii)Conditional :
-Utilize an if-else statement to customize the support message based on the user’s reported emotions.

iii)iterative:
-Implement a loop(such as a for loop) to iterate over a list of available emotion support resources and display them to the user.
FUNCTIONS OF EMOTIONAL SUPPORT
# User input
emotions = ["Depressed", "Sad"]
mental_state = "Low"

# Emotional support and resources
support_message = ""

# Check mental state and provide appropriate support
if mental_state.lower() == "suicidal":
support_message = "I'm really sorry to hear that you're feeling this way. It's important to reach out to a mental health professional or a helpline immediately. They can provide you with the support you need."

elif mental_state.lower() == "depressed":
support_message = "I'm here for you. It's important to remember that you don't have to go through this alone. Consider talking to a mental health professional or a trusted person in your life. They can help you navigate through these difficult emotions."

else:
# Customize support message based on reported emotions
if "depressed" in emotions:
support_message += "I'm sorry that you're feeling depressed. It can be helpful to engage in activities that bring you joy or talk to someone you trust about how you're feeling."

if "sad" in emotions:
support_message += "I understand that you're feeling sad. Remember to take care of yourself and reach out to loved ones for support."

# List of available emotion support resources
emotion_support_resources = ["Support helpline: 1-800-XXX-XXXX", "Online support group: www.example.com"]

# Display emotion support resources
if len(emotion_support_resources) > 0:
support_message += "\nHere are some emotional support resources you can explore:"
for resource in emotion_support_resources:
support_message += "\n- " + resource

# Print the support message
print(support_message)




3 Long-Term Prevention:
- Establish a long-term plan to prevent self-harm by creating a support network and setting up

# Function to create a support network
def createSupportNetwork():
supportNetwork = []  # Empty list to store the support network contacts

# Code to add contacts to the support network
while True:
contact = input("Enter a contact for your support network (or enter 'done' to finish): ")
if contact == "done":
break
supportNetwork.append(contact)

# Code to display the support network contacts
print("Support Network Contacts:")
for contact in supportNetwork:
print(contact)

# Function to set up a long-term prevention plan
def setUpLongTermPlan():
# Code to customize and set up the long-term prevention plan goes here...
print("Setting up the long-term prevention plan...")
print("1. Develop healthy coping mechanisms.")
print("2. Establish a regular exercise routine.")
print("3. Engage in activities that bring joy and relaxation.")
print("4. Seek professional therapy or counseling.")
print("5. Stay connected with supportive friends and family.")
print("6. Practice self-care and self-compassion.")
print("7. Create a safety plan in case of emergencies.")
print("8. Monitor and manage stress levels effectively.")
print("9. Educate yourself about self-harm prevention strategies.")
print("10. Regularly evaluate and reassess your progress.")

# Calling the functions
createSupportNetwork()
setUpLongTermPlan()








