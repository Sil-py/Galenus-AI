# Galenus-AI

AI assistant for doctors


## Summary

A chatbot helps family doctors to manage routinary requests.


## Background

Family doctors are expected to handle most frequent illnesses and to send patient to specialists or to a hospital for more complex cases. 
Unfortunately, they must spend a great deal of time in answering to very routinary requests. Some doctors hire a human assistant to filter such requests (which of course is a pretty expensive solution), others struggle with voicemail, sms and whatsapp messaging. 
A chatbot could filter the simplest requests without the doctor having to phisically answer the phone or digit the messages, saving a lot of time and helping doctors to focus on more complex cases. 
(I refer to the situation in Italy, but I think that could be the case in other countries, too).


## How is it used?

At a first stage, the chatbot could handle two sets of simple cases:
* Appointments: the patient asks to see the doctor (eventually mentioning some preferred times or days) and the chatbot offers the first availability.
The appointment is automatically filled into the doctor’s agenda and confirmed to the patient via sms. The chatbot could also manage cancellations.
* Prescritions: the patient ask for prescrition of some drugs he/she routinary takes (e. g. birth control pill) or needed for most common illnesses (e. g. aspirin). The chatbot could be trained to ask some questions (How old is the patient? Does he/she take other drugs?). The doctor would find a list of required prescriptions; the decision whether it is correct to prescribe the drug or not (based on the information the patient gives to the chatbot) still lies with the doctor. The prescrition could include some instructions on how often or how to take th drug (as it already is now with “manual” prescritions: “Take a pill three times a day before meals”). Some drugs should be excluded from this method if they require special recommendation or supervision. The doctor could also get an alert if the patient’s request is anomalous (e.g. a patient that asks too frequently). In all this cases the patient receives an sms where he is advised to have a conversation with the doctor.

People affected by this solution are family doctors and patients, so potentially it is a very large set of very different people:
* Doctors could be very much relieved by a solution that saves their time. 
* Younger patients that are often more used to digital interaction could be at ease with this solution from day one. 
* Older patient could need some time to get used to it. Still, wating for hours to get the line with the doctor, as it may happen, could be unnerving if you have a very simple request and they could start liking the chatbot.



## Data sources and AI methods

The chatbot could be trained using real registered phone calls made to a panel of doctors. First, we have to label cases that are simple and could be solved by the chatbot and those which are complex and where a conversation with a real doctor would be needed. Then, for those which can be managed by the chatbot, the associated outcome could be an appoinment with the doctor or a prescrition. 

AI technique needed are NLP techniques.


## Challenges

Doctors carry a very important responsibility for their patient’s health. The point of the solution is not replacing their judgement, but helping them filter requests in a way that also makes its easier to detetct cases that need further attention. 

Also, as the laws and rules affecting medicines differ across countries (e. g.: which drugs need a prescritpion), so the solution should be developed separately or refined for every country where we wish to apply it.


## What next?

An image recognition tool: the spelling of drugs’ names could be tricky, if the patient could upload an image to be recognized.


## Acknowledgments

I thank for inspiration my brother-in-law, a talented and scrupulous doctor and the pediatrician that handles my children. 
