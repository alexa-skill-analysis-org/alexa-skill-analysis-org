A Privacy & Security Analysis of the Alexa Skill Ecosystem
==========================================================
Christopher Lentzsch, Sheel Jayesh Shah, Benjamin Andow, Martin Degeling, Anupam Das, William Enck

Security & Privacy Issues with Alexa Skills
-------------------------------------------

  * `data/skills` metadata downloaded from the skill stores
  * `data/fisher_test_samples` metadata and activation patterns of the *Auto-Enabling Skills* section

Paper
-----

### Overview: Findings


We perform the first large- scale analysis of Alexa skills, obtained
from seven different skill stores totaling to 90,194 unique skills. Our
analysis reveals several limitations that exist in the current skill
vetting process. We show that not only can a malicious user publish a
skill under any arbitrary developer/company name, but she can also make
backend code changes after approval to coax users into revealing
unwanted information. We, next, formalize the different skill- squatting
techniques and evaluate the efficacy of such techniques. We find that
while certain approaches are more favorable than others, there is no
substantial abuse of skill squatting in the real world. Lastly, we study
the prevalence of privacy policies across different categories of skill,
and more importantly the policy content of skills that use the Alexa
permission model to access sensitive user data. We find that around 23.3
% of such skills do not fully disclose the data types associated with
the permissions requested. We conclude by providing some suggestions for
strengthening the overall ecosystem, and thereby enhance transparency
for end-users.

  * Auto-Enabling the wrong skill
  * Faking Developer Names
  * Dormant Intents
  * Bypassing Permissions
  * Squatting Patterns
  * Privacy Policies

**For more details visit: [alexa-skill-analysis.org][0] or Read the [Paper][1]**

### Reference

**Christopher Lentzsch, Sheel Jayesh Shah, Benjamin Andow, Martin
Degeling, Anupam Das, and William Enck.** _Hey Alexa, is this Skill Safe?:
Taking a Closer Look at the Alexa Skill Ecosystem._ In Proceedings of the
28th ISOC Annual Network and Distributed Systems Symposium (NDSS), 2021.

### BibTeX

    @inproceedings{ alexa-skill-ecosystem-2021,
    author  = {Christopher Lentzsch and Sheel Jayesh Shah and Benjamin Andow and 
              Martin Degeling and Anupam Das and William Enck},
    title   = {Hey {Alexa}, is this Skill Safe?: 
              Taking a Closer Look at the {Alexa} Skill Ecosystem},
    booktitle = {Proceedings of the 28th ISOC Annual Network and 
                Distributed Systems Symposium (NDSS)},
    year   = 2021
    }
              

[0]: https://alexa-skill-analysis.org/
[1]: https://alexa-skill-analysis.org/
