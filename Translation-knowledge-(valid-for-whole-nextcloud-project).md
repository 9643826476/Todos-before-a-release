# Nextcloud is available in many languages. How is that done?
Instead of maintaining an own translation server like pootle Nextcloud is using Transifex to achieve translation in many languages.
Transifex offers free service for open source projects.

Are you interested in translating Nextcloud?

Just create an account and apply to join Nextcloud organization. You are welcome!

Once you joined our organization you can apply to join your target language. There are already more than 70 languages available. Feel free to request a new one if your native language is missing.

Best way is to start translating some strings. Get an overwiew about already existing translations. Check features and basic function of Transifex.

If you get caught by l18n stuff and you take care about your language you can think about beeing a reviewer. Even more fun :-)

# General information about Transifex
## Language teams
Each language is organized in a team.

You have organizers, reviewers and most important translators. You are the engine of the car. 

## How to discuss at Transifex?

You can discuss for each string. Who ever reads it can respond. There is no way to subscribe to any discussion as long as somebody marks discussion as issue.

For language teams there is a chance to discuss as well. It is not easy to find at web UI and not many people responding (german team experience with more than 100 members)

You could send private message to other members. Inbox and outbox are separate and there is no option to see threaded messages. You cannot invite third person to private discussions.

## Different roles at Transifex?

To unterstand roles and their respective permissions see https://docs.transifex.com/teams/understanding-user-roles/

# Information for Translators
## Basic knowledge to start
You have joined a language team. Do not hesitate to contact persons of it.

Newbie information: Whenever translating parts of a single resource please do not just translate a single string without looking at already translated strings. Most resources have a common wording and you should follow it. If you have a different position you should discuss first before changing strings.

Translate easy ones before trying complex ones.

Do not use translate.google.com to just enter and copy result to Transifex.

## When to comment a string at Transifex?

If you are struggling to translate a string feel free to add a comment including your question.

## When to create an issue at transifex?

Whenever you feel just a comment is not sufficient and you need information to help all other language translators feel free to mark your comment as an issue.

## What to do if I want to change a source string?

Sometimes you encounter a typo are other spelling error inside a source string. Or you find an error or grammar issue. If so, feel free to file an issue or even better go to GitHub and provide PR (Pull request) to correct it.
Most translators are not familiar with coding tools like GitHub nor do have coding background. In such cases just add an comment and mark it as issue. Do you have an GitHub account? Go to related repository and file issue. Community members will work on it.

# Information for Project Maintainers
## How to handle new language requests?

Nextcloud want to cover the world. To reach this target we need to provide as many languages as we can get.
Luckily every week we get new language requests. Great. But do not simply accept it. 
Please check if similar languages are already there. If so, check the team size and send a personal message to language requester. Tell him/her about the language you found, provide link to team and ask her/him to join named team.

What happens if we accept all language requests?

We have a lot of languages. The no. will be impressive, but the state of completeness is low and quality might be as well.

...


## How to work on issues
...

# Information for German Team Members (in german)
## Wieso zwei Sprachen?
Für die deutsche Sprache gibt es zwei Übersetzungen bei Transifex. Diesen Luxus und Aufwand gönnen sich aktuell nur die Deutschen. Die Mitgliederzahl ist stark und der Übersetzungsgrad hoch.

In Deiner Nextcloud kann jeder Benutzer seine Sprache in den persönlichen Einstellungen vornehmen (nicht global).

Die Language-Codes mit deren Zuordnung wurden vom Nextcloud-Projekt festgelegt.

### Die formelle Übersetzung (Sie-Form).

Link: https://www.transifex.com/nextcloud/nextcloud/language/de_DE/

Language code: de_DE

### Die informelle Übersetzung (Du-Form).

Link: https://www.transifex.com/nextcloud/nextcloud/language/de/

Language code: de

## Infos für Reviewer

...

## Infos für Übersetzer

Wenn ein String übersetzt wird, dann immer beide Sprachen pflegen. Das führt zu einem konsistenten Übersetzungsgrad und spart die Nacharbeit.

...

## Angleichen der Übersetzungen

...
## Besonderheiten
### iOS-App
In der Apple-Welt wird die Sie-Form empfohlen und es kann nur eine deutsche Übersetzung für die Sprachauswahl "deutsch" herangezogen werden. Das App-Team hat entschieden die Sie-Form zu verwenden. Daher ist eine Übersetzung für die Du-Form nicht notwendig. Daher wird bei allen Strings der Du-Form der String "" eingetragen. Vorteil: Auch Personen die selten an den Übersetzungen mitarbeiten verschwenden keine Energie für Nicht-Verwendete Übersetzungen.

### Besonderheiten für die Windows Phone-App
Auch hier wird in Zukunft nur eine Übersetzung benötigt. Klärung erfolgt noch.
...

### Besonderheiten für die Android-App
... fehlt noch