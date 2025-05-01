## Lab 1: Using out-of-the-box skills and creating a skill flow

## Use Case

In this tutorial we import a skill to generate a welcome message for new hires using the watsonx.ai generate content skill. We then use another skill (Outlook) to send the previously generated message by email. Finally, we combine the two skills into a Skill Flow, to accomplish a more complex multi-step task. The high-level steps to accomplish this are as follows:

* 1. Connect to watsonx.ai application and add the generate content skill to AI chat

* 2. Test the skill by generating a welcome email to a new hire

* 3. Connect to Outlook application and add the skill to send an email to AI chat

* 4. Test the skill by sending email to yourself

* 5. Create a skill flow by combining the two skills you just added

* 6. Test the skill by generating a new hire welcome email and sending it to yourself

## Assumptions

## See lab README file for details

To complete this lab you need:

* 1. Access to an IBM watsonx Orchestrate tenant (on AWS or on IBM Cloud)

* 2. As of now (2/16/25) you will need admin rights to connect skills to the AI chat. In the future admin rights may not be required.

* 3. Outlook email ID and credentials (see lab README file)

## Step 1: Connect to watsonx.ai application and add the generate content for an email skill to AI chat

* 1. Log into watsonx Orchestrate with your IBM ID

* 2. Navigate to Skill sets in the hamburger menu:

Note: if you are using watsonx Orchestrate on AWS, you would need to go into Manage Team -> Skill sets

* 3. Search for an application with skills you want to use in AI chat, i.e. watsonx.ai in this case

* 1. Select Orchestrate Agent Skillset

* 2. Select Connections panel

* 3. Search for application name (watsonx.ai)

* 4. Click on … to the right of the application name and then click on Connect app:

O

## 5. Select Team credentials and then click on Connect app:

## Connect to watsonx.ai(experimental)

Member

credentials

Each

team

member

uses

own

credentials

to

connect

this

their

and

use

skills.

to

app

its

O

Team

credentials

The

admin

credentials

each

team

member

to

this

and

sets

the

uses

connect

app

use

its

to

skills.

Click

type.

credential

credentials

Connect

provide

You

selected

Team

for

the

app

the

to

to

connect

to

use

will

team

your

credentials

and

the

app.

Connect

app

2

* 6. Enter bearer token (in this case no credentials are needed, you can just enter 6+ random characters) and click on Connect app:

* 7. Once the application has been connected, go into the AI Agent configuration:

* X IBM watsonx Orchestrate

* 8. Under Apps and skills select the application you just connected (watsonx.ai):

* 10. Provide a description about what the skill does, to help the supervisory agent route requests, and click on Add skill:

Step 2: Test the skill by generating a welcome email to a new

hire

* 2. Type your request in the chat to test the added skill:

Good

Evening

8:26

PM

## Hello, welcome to watsonx Orchestrate.

Hello,

How

Good

morning,

What

day

is

Help

me

send

an

email

you?

are

today?

Understand

AI

capabilities

Understand

AI

capabilities

Understand

AI

capabilities

with

with

with

the

help

of

AI

Assistant.

the

help

of

AI

Assistant.

the

helo

of

AI

Assistant.

IBM|

to

Engineer

>

AI

a

to

email

short

generate

welcome

new

hire

As you can see, the query was routed to the right skill.

Note: a screenshot will be added here asap - as soon as the product issue related to connecting to watsonx.ai has been resolved

## Step 3: Connect to Outlook application and add the send email skill to AI chat

We will follow similar steps to connect to Outlook application and add the send email skill to AI chat. Note: you will need to use credentials provided to you to connect to Outlook (instead of using your own email account).

* 1. Navigate to Skill sets in the hamburger menu:

Note: if you are using watsonx Orchestrate on AWS, you would need to go into Manage Team -> Skill sets

* 2. Search for an application with skills you want to use in AI chat, i.e. Outlook in this case

* 1. Select Orchestrate Agent Skillset

* 2. Select Connections panel

* 3. Search for application name (Outlook)

Skillset

Orchestrate

Agent

1-1

of

1

items

5

Items

per

* 3. Click on … to the right of the application name and then click on Connect app:

## 4. Select Team credentials and then click on Connect app:

X

## Connect to Microsoft Outlook

Member

credentials

Each

team

member

uses

credentials

to

connect

to

this

their

app

skills.

own

and

use

its

Team

credentials

uses

to

team

The

admin

credentials

each

member

connect

this

and

use

sets

the

app

its

to

skills.

You

selected

Team

for

the

Click

credentials

credential

Connect

provide

type.

app

the

to

credentials

your

team

will

and

to

connect

to

app.

use

the

5. Select Non-admin user and then click on Connect app:

Connect to Microsoft Outlook

x

Type

Non-admin

user

Cancel

Connect

app

* 6. Use the credentials provided to you to log into Outlook (do not use your own Outlook email account):

* 7. Select Ask Later if prompted for additional security information

* 8. Select No when asked to “Stay signed in?”

* 9. Once you are connected to the application, go back into the AI agent

configuration: 10.Under Apps and skills select the application you just connected (watsonx.ai):

AI

agent

configuration

Agent

configuration

users

to

customize

their

chat

experience

according

to

their

allows

preferences

Apps

let

your

team

and

skills

connect

data

to

Model

settings

other

and

complete

tasks

in

applications

System

prompt

Starter

prompts

C

Whv

add

apps

and

skills?

€

Assistants

Apps

and

skills

Apps

Embed

chat

</>

Skills

are

grouped

by

their

a

plication.

Select

an

app

to

se

Q

Search

Sort

bv:

Alphabetically

A-Z

Outlook

IBM

Document

Processing

Microsoft

nx.ai(experimental)

Skill

flows

vices

11.Add skill to chat:

2

20

Ite

21-28

of

28

items

page:

* 12. Provide a description about what the skill does, to help the supervisory agent route requests, and click on Add skill:

email

Send

an

X

from

Microsoft

Outlook

An accurate description of the purpose and capabilities of the skill is required for the AI model to successfully activate this skill in the chat.

## Routing description

## Step 4: Test the skill by sending a test email

* 2. Type your request in the chat to test the added skill:

As you can see, the query was routed to the right skill. Fill in the details, click on Apply: You

9:04

PM

email

send

watsonx

Cancel

Apply

Verify that you received the test email: watsonx

9:06

PM

email

sent.

The

was

## Step 5: Create a skill flow by combining the two skills you just added

So far you have added the individual skills and tested them. You can combine two or more skills to create a skill flow. Steps to create a skill flow:

* 1. First, before creating the skill flow, we need to add the skills to our Personal Skills from the catalog:

Go into Skill catalog:

Search for watsonx.ai application in the Skill catalog and click on the watsonx.ai tile:

## Add the Generate an email skill:

Go back into the Skill catalog, search for Microsoft Outlook app, and click on the tile:

Search for the Send an email skill and Add skill:

Now that the skills have been added to the Personal Skills in the catalog, we are ready to create the skill flow!

* 2. Navigate to Skill studio by clicking the hamburger menu in the upper left corner and selecting Skill studio in the BUILD section

* 3. Create a new Skill Flow by clicking the dropdown on Create, then selecting Skill Flow

* 4. Click on the pen icon to edit the name of the skill and change it to

{Your_Initials} GenAI Email Flow then select Save

* 5. Click on the plus sign between the Start and End flow, then search for watsonx.ai skills and select

6. Search for Generate an email and select Add Skill +

* 7. Next click the + button below the Generate an email skill to add a new skill. Search for outlook and select the Microsoft Outlook skill group.

8. Select Add Skill + for the Send an email skill

* 9. Click on Send an email skill and in the Input tab click the body.Content, select Generate an email → generated_text

* 10. Now select Generate an email skill, in the Output tab turn on the toggle Hide

this form from the user

HB

11.Now save your skill flow as a draft by clicking the Actions drop down and

selecting Save as Draft 12. Next, click on the Actions dropdown again and select Enhance

(HB

13. To publish your skill, select the Publish button

Skills

/

## 14. Go into the AI agent configuration:

15.Under Apps and skills search for skill flows and click on the Skill flows tile:

16.Search for your skill flow by name and click on Add to chat to add the skill flow

to the AI chat:

AI

agent

configuration

data

tically

A-Z

17.Provide a routing description and click on Add skill:

## Step 6: Test the skill flow

Finally, you can test the skill flow that you have configured by entering your query in the AI chat:

|AI

:>

Note: screenshot of output will be added soon.

This final step concludes the lab. In this lab, you connected watsonx.ai and Microsoft Outlook send email applications and added the generate email and send email skills to the AI chat. Finally you combined those two skills into a skill flow and added the skill flow to the AI chat.