# WHAT IS NO_CODE🤒🤒
No code doesn’t mean you do not write code completely. Visual programming / No code is an umbrella term for developing software using visual elements.
*The technicalities involved can be handled with a basic understanding of how software works.*
Know more about👉👉 [No code opportunities](https://www.google.com/search?q=what+is+no+code+and+what+are+the+opportunities+involved&ei=sysDZIP9OvPr7_UPpbGmqAo&ved=0ahUKEwjDouuMlsL9AhXz9bsIHaWYCaUQ4dUDCA8&uact=5&oq=what+is+no+code+and+what+are+the+opportunities+involved&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAzIHCCEQoAEQCjIECCEQFToKCAAQRxDWBBCwAzoHCAAQsAMQQzoFCAAQgAQ6BggAEBYQHjoJCAAQFhAeEPEEOgUIIRCgAToICCEQFhAeEB06CgghEBYQHhAPEB06BQgAEIYDOgUIABCiBEoECEEYAFD9BliDemCOfGgFcAF4AIAB6QOIAY5WkgEMMC4xNC4xMS4xNC4ymAEAoAEByAEKwAEB&sclient=gws-wiz-serp) 

## USE CASES OF AI/NO_CODE TOOLS
1.Data predictions - Obviously.ai
2.Creative writing - ChatGPT
3.Art & design - playgroundai
4.Music - Avia
5.Motion Capture - kinetix.tech
6.Voice Cloning - UberDuck
7.bravostudio app - create figma designs and turn to native app

## CREATING YOUR FIRST AI APP 🥳
Tools needed to complete this tutorial:
- Google sheets [see here](https://docs.google.com/spreadsheets/)
* Glide [see here](https://www.glideapps.com/)
+ Make [see here](https://www.make.com/en)

## STEP I
<img width="298" alt="image" src="https://user-images.githubusercontent.com/109626709/222929681-6071ceac-9686-4556-a738-76a47f605397.png">

-Open your Google sheets and design the nature the app you want to create 
*NB: We're creating a shitposting! app that generates random funny tweets(output) about things(inputs given by user)*

## STEP II
<img width="415" alt="image" src="https://user-images.githubusercontent.com/109626709/222930049-4eeec2a7-cd02-4316-9401-33feeb50e9d5.png">

- Open [glide.com](https://www.glideapps.com/) and link to your google sheets
* Glide automatically renders the data you entered in google sheets.
 then you can edit the interface as you wish
 
*Recommended : Start by creating a custom navigation bar* *see below* 👇👇
<img width="947" alt="image" src="https://user-images.githubusercontent.com/109626709/222930701-a5c1e175-5cdd-46d8-b58e-b7421250d22f.png">

## STEP III (Connecting a webhook to your APP)
<img width="954" alt="image" src="https://user-images.githubusercontent.com/109626709/222931283-f4e03a1e-ad46-4af3-b297-c0f732f69033.png">

- Open [make.com](https://www.make.com/en)
* create a new scenario
+ Generate a custom webhook (this gives a url address to send your information to if triggered)
- Go back to button under **COMPONENT** in glide, change the ***ACTION*** from ***show notifications***(which is its default if triggered) to ***trigger webhook***
* Now add the new webhook you just generated (name & url generated)
+ Then click on **add value** set the key value pairs (as Input => Input) && (Output => Output)

## STEP IV (Connecting an AI to your APP)
<img width="848" alt="image" src="https://user-images.githubusercontent.com/109626709/222932189-3b03f4e1-bf9a-4ea5-9389-89407c67ed00.png">

- on make.com, click on add new module, search openAI, click on create completion
* Model : text-davinci-003
+ Prompt: Create a shitpost about ```params:Input:Value```
- Max Tokens: 3000
* Temperature: 0.8

## STEP V (Connecting the output from the AI back into your APP)
<img width="957" alt="image" src="https://user-images.githubusercontent.com/109626709/222932528-c995faec-0329-435c-aed8-29ce581467cf.png">

- Create another module, search google sheets, click on update row
* Spreadsheet ID : *your spreedsheet file*
+ Sheet name : sheet 1
- Headers : yes
* Input : ```Params:Input:value```
+ Output : ```choices[ ]:text```
click ok!!

## Finally🎊🥳 checking to see if your APP works perfectly!🚀
- Enter a random input (according to your prompt in step IV above, thus: create a shitpost about ```input```), click on the button
* The input entered go thus : webhook => openAI => Google sheets => Glide app
+ This process might take a while to complete. 

```NB: Ensure you save your scenario on make.com to avoid errors ``` 

**Thank you!😎👏**
Follow me on [twitter](https://twitter.com/adavize_jude) and give me a shoutout tweet if this was helpful. Don't forget to tag me 🤗



**Want to learn more about no code And its endless opportunities??**😲🤭🚀
**Check out *Mr Norton, a social entrepreneur and no code developer on* [youtube](https://www.youtube.com/@mr.hackathon)**
