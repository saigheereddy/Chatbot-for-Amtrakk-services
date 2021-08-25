# Chatbot-for-Amtrakk-services
ABSTRACT

Before the Covid-19 pandemic, National Railroad Services doing business as the Amtrak Services was one of the most used means of transportation and was widely used by the people in the United States. This service provides medium and long-distance intercity service in contiguous United States and nine Canadian cities, it serves more than 500 destinations in 46 states. (Amtrak Facts)  Going by these numbers we can estimate that the passenger counts using this service will also be very high and to provide them with the information that they need in an efficient and easier way is the most important and crucial aspect of maintaining this service. In this project we are going to build a Chatbot that can be accessed using our website or by calling us at our designated telephone number. This chatbot answers various frequently asked questions and enables the feature of booking a ticket and it also sends an acknowledgement and confirmation mail to the designated mail id that has been provided by the customer through the Web UI or phone. This chatbot has been built using Google’s Dialog Flow which is a natural language understanding platform that makes it easy to design and integrate a conversational user interface into our mobile app, web application, device, bot, interactive voice response system, and so on. Dialogflow can analyze multiple types of input from the customers, including text or audio inputs (like from a phone or voice recording). It can also respond to customers in a couple of ways, either through text or with synthetic speech.(Google Cloud, 2021)  Before we dive deep into our project and the details let us first understand how NLP plays a role of a fundamental building block of Chatbots and Text Processing. 

Introduction to NLP:

Tracing back to the early stage of humans where only hand gestures were used to communicate, we have come a long way where we now interact with computers, almost every day, by a new method called Natural Language Processing. Thanks to the significant rise of AI and ML technologies that help facilitate seamless interaction between a human being and a machine. (Jena, 2020) NLP is a type of Artificial Intelligence that provides machines the capability of reading, understanding, and interpreting the meaning from human languages. Natural Language Processing, is concerned with the interactions between computers and human (natural) languages, how to program computers to fruitfully process large amounts of natural language data.” In layman's terms, Natural Language Processing (NLP) is concerned with how technology can meaningfully interpret and act on human language inputs.(Phillips, 2018) NLP allows technology such as Amazon’s Alexa to understand what you’re saying and how to react to it. Without NLP, AI that requires language inputs is relatively useless.

How Does NLP Work in Chatbot?

NLP is at the core of chatbot architecture without which they add no value. When you type “Hi”, the bot recognizes it as a standard greeting and leverages the AI capability to give a response. It understands the user’s message, parses, and converts it into structured data that computers can interpret. A message is not treated as a set of symbols but the hierarchical structure of language – words, phrases, sentences, and coherent ideas is analyzed. With the pre-programmed or acquired knowledge, NLP decodes the segments of the sentence and extracts the intent and entity of the message. “Intent” is the goal of the message and “entity” is something that modifies the intent. For example, in a statement “What is the weather in New York”? the intent of the user is to know the weather. Intents are often a verb or a noun. Here, the entity is “New York” i.e., the “place” Entities are often place, time, or objects.

Without NLP, bots cannot understand the difference between a “Hi” and a “Goodbye”. It is the NLP that provides the input text’s meaning and context for the bot to respond. Chatbots mimic the different functions of the human brain like learning, reasoning, interacting, understanding, and perceiving. (Jena, 2020)
i.	Learning: Chatbots evolve over time, that is, they can accept user “corrections” and improve response
ii.	Reasoning: NLP provides the ability to “read” and parse natural sentences
iii.	Interacting: They memorize and recall every single back and forth conversation and can learn to respond from human agents.
iv.	Understanding: Chatbots are smart to know what the user’s is intending to ask or know, even if their language is not phrased rightly
v.	Perceiving: Bots that are good at intent recognition can also be trained to answer simple FAQs so that agents can denote time for complex queries.


About Amtrak Services:
The national Railroad passenger corporation, Amtrak is a corporation that is delivering high quality, safe, on-time rail passenger service connecting the United States of America in safer, greener, and healthier ways (Amtrak Facts). It was created in 1970, to take over the majority of the privately held intercity passenger rail services that showed huge net operating losses. With over 21000 route miles and establishment in 46 states including the US capitol Washington D.C, Amtrak is currently running 300 trains each day to over 500 destinations. Due to the ongoing COVID-19 Pandemic, the US-based passenger railroad service company has suffered huge losses since the travel demand has plummeted dramatically. Amtrak adjusted and reduced schedules beginning in March 2020 for services across its network. Many of the low demand national and international routes have been suspended due to border closures but the corporation is trying hard to restore services by assessing the travel needs continuously by following the COVID19 guidelines (Amtrak Facts).
Idea of the Project:
We know that at times like these when we are in the middle of a pandemic, people tend to have a lot of questions and concerns about using public transport and it becomes more and more difficult for everyone to either ask or answer these questions. Our chatbot can be used to address this problem as we have created the chatbot using dialogflow’s knowledge base service which uses Natural Language Processing to provide a response to an end-user expression. In a nutshell, the entire idea behind our chatbot is to provide an interface using which multiple users can interact with our chatbot for various reasons ranging from booking a train ticket to getting answers for the most basic questions and we want this chatbot to be more presentable and accessible to users without having to face the trouble of scrambling for the website and having to go through the job of typing in long queries and to address this issue we have used  Dialogflow’s Phone Gateway to build conversational interactive voice response services(IVR),(Google Cloud, 2021) that integrates with the rest of the agent. This is used to provide the users with a telephone interface agent which can be accessed by using the telephone number hosted by Google. 

Another important detail about our project is to make the task of booking a train ticket easier for everyone and when booking the ticket, it is important for the user to get an acknowledgement or confirmation of the event that has occurred and to address this we have implemented a python script which sends an acknowledgment email to the email address provided by the user. 

Different Platforms Available for Building Chatbots:
Chatbots are very popular. Being more advanced than a live chat tool, bots address the customers’ queries instantly across channels without the need for a support agent. It is very hard to believe that the most powerful brands today are building them (Patil, 2020). Businesses get tons of customer queries daily. It could become difficult to manage all the queries easily. So, the customer service has become the defining factor for customers choosing the best service among the available platforms.(Chatbot Frameworks 2021). With constant new releases and updates, there are many AI chatbot development frameworks that are combating each other for the top spot. Some of the powerful platforms for chatbot frameworks include the Microsoft Bot Framework, RASA, IBM Watson, Amazon Lex, Wit AI, Dialogflow etc (Chatbot Frameworks 2021). 


Why Dialogflow?
In this project the AI development framework used is Dialogflow, which is a subsidiary of Google. With its advantage of machine learning capabilities, built in NLP features and integrations with many other popular communications platforms, Dialogflow has the power to create highly intelligent chatbots that can understand and keep improving over time (Chatbot Frameworks 2021). The main advantage of Dialogflow is that it is supported by Google’s cloud natural language, making it easier to train the bot to understand human emotions and sentiments. Furthermore, the framework supports both voice-based and text-based assistants, support for more than 20 languages, performing sentiment analysis on every query, best quality conversations using NL, and above all it is easier to understand even for the beginners. The Dialogflow comes in both free and paid versions. The project is developed over the standard free edition (Chatbot Frameworks 2021).

Architecture: 
The system architecture has the following components: 
Multichannel integration: Any conversational interface connects to several networks, which can be speech or text based.
Conversation management: This part is at the heart of the GUI, and it usually performs the following tasks:
•	Text-to-Speech (TTS) and Speech-to-Text (STT): Conversation interfaces can communicate with both voice and text.
•	Agents: Agents oversee manipulating the conversation's flow based on the purpose or inspiration derived from the user's conversation. An agent framework that can manage linear and nonlinear conversations is an important feature of a good conversation interface.

Dialogflow is a development suite for building conversational interfaces for websites, mobile apps, common messaging channels, and Internet of Things (IoT) devices that is end-to-end, build-once, and deploy-everywhere. It can be used to create natural and rich interactions between users and the company, such as chatbots and conversational interactive voice response (IVR). Preprocessing data to construct topics and extracting and saving related synonyms for given topics are also part of the chatbot development process. Topics are imported as individuals, and data is uploaded to Dialogflow Agent. Entities are Dialogflow's way of defining and extracting valuable information from natural language inputs. We can build intents in the agent that map user feedback to responses once the entities are set. It allows us to describe examples of user statements that can activate the intent, as well as what to extract from them and how to react, in each intent.

Fulfillment interface: A robust fulfillment interface is needed to link virtual agents to external systems, and no conversation interface system is complete without one. This interface is needed to link to external systems and retrieve complex information to continue or complete a conversation. By using Fulfillment code, which is deployed as a webhook, Dialogflow can connect to external systems on an intent-by-intent basis. During a chat, fulfillment allows us to use the data gathered by Dialogflow's natural language processing to produce dynamic responses or initiate backend behavior. Finally, we use Dialogflow's JavaScript API to build a custom user interface that interacts with the chatbot. Because of all these advanced features it has to offer we have chosen dialogflow as our platform to build our chatbot.


Implementation using Dialog Flow:
Some of the basic features that we have used to build our chatbot are:
i.	Agent: User interactions are handled by handler, which is an all-encompassing natural language comprehension module.
ii.	Intents: An end-user request is known as intent
iii.	Entities: Entities are parameters that are derived from end-user intents and used to fill requests.
iv.	Context: Context is used to link intents and create natural conversations between the agent and the end-user.
v.	Fulfillment: The Dialogflow agent can only answer with static pre-defined messages if fulfillment is not provided. Fulfillment must be allowed to dynamically fulfill requests.

For example, you could create a weather agent that recognizes and responds to end-user questions about the weather. You would likely define an intent for questions about the weather forecast. If an end-user says, "What's the forecast?", Dialogflow would match that end-user expression to the forecast intent. (Google Cloud, 2021) You can also define your intent to extract useful information from the end-user expression, like a time or location for the desired weather forecast. This extracted data is important for your system to perform a weather query for the end-user.
A basic intent contains the following:
i.	Training Phases: These are example phrases for what end-users might say. When an end-user expression resembles one of these phrases, Dialogflow matches the intent. You don't have to define every possible example, because Dialog Flows built-in machine learning expands on your list with other, similar phrases.
ii.	Action: You can define an action for each intent. When an intent is matched, Dialog Flow provides the action to your system, and you can use the action to trigger certain actions defined in your system.
iii.	Parameters: When an intent is matched at runtime, Dialog Flow provides the extracted values from the end-user expression as parameters. Each parameter has a type, called the entity type which dictates exactly how the data is extracted. Unlike raw end-user input, parameters are structured data that can easily be used to perform some logic or generate responses.
iv.	Responses: You define text, speech, or visual responses to return to the end-user. These may provide the end-user with answers, ask the end-user for more information, or terminate the conversation.
v.	Integrations: Dialog Flow integrates with many popular conversation platforms like Google Assistant, Slack, and Facebook Messenger. If you want to build an agent for one of these platforms, you should use one of the many integration’s options. Direct end-user interactions are handled for you, so you can focus on building your agent. Each integration handles end-user interactions in a platform-specific way. There are multiple types of integrations. In this project we have used only web Demo and Dialog Flow Messenger integrations.
vi.	Dialog Flow Web Demo: Dialogflow Web Demo provides a simple text chat user interface for our agent.
vii.	Dialog Flow Messenger: The Dialogflow Messenger integration provides a customizable chat dialog for our agent that can be embedded in our website. The chat dialog is implemented as a dialog window that can be opened and closed by our end-user. When opened, the chat dialog appears above your content in the lower right side of the screen.
viii.	Webhook: A webhook is a user defined HTTP callback that is automatically invoked whenever certain criteria is fulfilled. A webhook can be created in any server-side programming language like Python, PHP or Node.js. In Dialog Flow, a webhook can be used to fetch data from our server whenever a certain intent having webhook enabled is invoked. The information from the intent is passed to the webhook service to receive the result.
ix.	Dialog Flow Phone Gateway: The Dialog Flow phone gateway feature provides a telephone interface to our agent. It is used to build conversational IVR (interactive voice response) solutions that integrate with the rest of your call center network. Currently, we can select a telephone number hosted by Google. In the future, we will also be able to port an existing telephone number.

Knowledge Base: 
A knowledge base represents a collection of knowledge documents that you provide to Dialog Flow. Knowledge documents contain information that may be useful during conversations with end-users. Some Dialog Flow features use knowledge bases when looking for a response to an end-user expression. We have used knowledge base to answer the user’s frequently asked questions (FAQ’s) that we have framed based on our application.


Detailed steps of working of Chatbot:

i.	A user sends a message to a computer or an App through text or voice.
ii.	The message is sent to Dialogflow by the app/device.
iii.	The message is classified and matched to the appropriate purpose (Intents are defined manually by developers in Dialogflow)
iv.	For each intent in the fulfillment process, we describe the actions that will be taken (Webhook).
v.	When Dialogflow discovers a specific purpose, the webhook can use external APIs to search for an answer in external databases.
vi.	The webhook receives information from the external databases.
vii.	The webhook responds to the purpose with a formatted answer.
viii.	Intent creates actionable data based on various platforms.
ix.	Input Apps/Devices receive the actionable data.
x.	The user receives an answer in the form of text, picture, or speech.

A more detailed illustration can be seen in the below screenshots:
Chatbot Welcome page (We have used a different name for our website “AmTrack” in order to distinguish it from the original one)
 
                                          

 

The above screenshots show us that we have successfully booked a ticket from Columbus to Boston and a confirmation mail is being sent to the given email ID.




Test cases
 
 
The above scenario shows that there are no trains available from Chicago to Baltimore	  
                                   
 There are no trains available on the requested date.
  











FAQ’S : Our chatbot can give information to various queries, some of the queries which we can ask the chatbot are shown below 

 

Getting information about face masks and various mandatory rules to follow
	 

Getting information about the speed of the train 
 
Information about cancelling any reservations made. 
	 

Information about ticket cost 



Challenges faced:
One of the major challenges we faced in this chatbot was to get the data of the available sources and destinations, there was no API to provide us this data and as a result of this we had to create a custom dataset that contains this information. The next challenge was to create an API that could provide this data to the chatbot. Based on our requirement it was also important for us to send an acknowledgement email confirming the ticket booking event and implementing this task using the custom API was also a stretching task.  
Creating a visually intuitive UI and deploying it through node js was another monumental task that we had to deal with. We also had to train our agent for various test cases and as we wanted to build a chatbot that connects all the dots without leaving any ambiguity we had to make sure that booking the ticket was only possible after validating the date and time the user enters to the actual schedule of the trains that we were running(Custom dataset). All these validations required a lot of effort and rigorous testing of all these use cases was done before finally deploying our chatbot. 


Conclusion:
Finally, we have created a chatbot that can be accessed through our website or the phone number(+1 678-827-5769) that we have reserved from dialogflows phone gateway feature. Once the user has accessed the chatbot our agent can interact with the user and respond to the queries that the user sends through text or speech. The UI has been designed using html and a custom API has been created for providing the data related to schedules of the trains that are currently operating on our service. The website is hosted in the localhost server that is deployed through Node JS.
We have created various validation steps that process the user inputs and provide the user with an accurate and closely related response and when any of these validations fail exception responses informing the user about the reason are displayed. Once the user input matches the schedule of our train service the chatbot agent asks for additional information such as name, phone number, and email. An acknowledgment mail is sent to the user’s mail id that has been entered. This email contains the details of the ticket that has been booked, a unique booking id is also generated for every ticket that has been booked. 


Bibliography
Amtrak. (2020, 09 08). Amtrak Facts. https://www.amtrak.com/about-amtrak/amtrak-facts.html
Google Cloud. (2007). Dialogflow ES documentation (1st ed., Vol. 1). Google. https://cloud.google.com/dialogflow/es/docs/
Google Cloud. (2007, 10 1). Intents. Dialogflow ES. https://cloud.google.com/dialogflow/es/docs/intents-overview
Google Cloud. (2021, 05 07). Building a chatbot agent by using Dialogflow. https://cloud.google.com/architecture/building-chatbot-agent-dialogflow
Google Cloud. (2021, 05 07). Building and deploying a chatbot by using Dialogflow. https://cloud.google.com/architecture/building-and-deploying-chatbot-dialogflow
Google Cloud. (2021, May 07). Dialogflow. https://cloud.google.com/dialogflow/docs#:~:text=Dialogflow%20is%20a%20natural%20language,response%20system%2C%20and%20so%20on.
Jena, S. (2020, October 5). Natural Language Processing in Chatbots. Data Science Central. https://www.datasciencecentral.com/profiles/blogs/natural-language-processing-how-this-innovative-technology-is
Maruthi TechLabs. (2020, November 10). Step-by-step Guide On Building a Chatbot Using DialogFlow. https://marutitech.com/build-a-chatbot-using-dialogflow/
Patil, P. (2020, July 14). Top 30 Popular Platforms For Chatbot Development. https://chatbotsjournal.com/top-30-powerful-and-best-platforms-to-build-chatbots-bf413419d584
Phillips, C. (2018, May 24). Natural Language Processing (NLP) & Why Chatbots Need it. Chatbots Magazine. https://chatbotsmagazine.com/natural-language-processing-nlp-why-chatbots-need-it-a9d98f30ab13
Space Technologies. (2020, October 23). Top 10 AI Chatbot Development Frameworks [Pros + Cons + Integration + Pricing]. https://www.spaceo.ca/top-ai-chatbot-frameworks/
Google Cloud. (2021, May 07). Dialogflow phone gateway. https://cloud.google.com/dialogflow/es/docs/integrations/phone-gateway

