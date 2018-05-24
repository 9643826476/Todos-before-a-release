# Nextcloud is available in many languages. How is that done?
Instead of maintaining our own translation server, like Pootle, Nextcloud uses [Transifex](https://www.transifex.com/nextcloud/nextcloud/dashboard/) to facilitate translations for many languages.
Transifex offers free service for open source projects.

Are you interested in translating Nextcloud?

Create an account on Transifex, then apply to join the Nextcloud organization. You are welcome.

Once you have joined the organization, apply to join one of the over 70 target languages available. Should yours be missing, feel free to request it.

Best way is to start translating some strings. Get an overview of what and how things have already been translated.
There are some features and functions in Transifex, but the basics is pretty much all that works.

If translating is not your boat of wood, or similar, you can be a reviewer. Even more fun :-)

## How to discuss at Transifex?

You can discuss for each string. Whoever reads it can respond. There is no way to subscribe to any discussion as long as somebody doesn't mark the discussion as an issue.

For language teams there is a chance to discuss as well. It is not easy to find through the web UI and not many people respond (German team experience with more than 100 members)

You can send private message to other members. Inbox and outbox are separate and there is no option to see threaded messages. You cannot invite a third person to private discussions.

Using [the forum](https://help.nextcloud.com/) is a much better idea.

## Different roles at Transifex?

To understand roles and their respective permissions see https://docs.transifex.com/teams/understanding-user-roles/

You have Maintainers,language coordinators, reviewers and most importantly: translators. You are the engine of the car.

# Information for Translators
## Basic knowledge to start
You have joined a language team. Do not hesitate to contact people in it.

Newbie information: Whenever translating parts of a single resource please do not just translate a single string without looking at already translated strings. Most resources have a common wording and you should follow it. If you have a different position you should discuss first before changing strings.

Translate easy ones before trying complex ones.

Do not use translate.google.com to just enter and copy result to Transifex.

## Common rules

### Ellipsis
Whenever you need triple dots (punctuation mark) to show progress or similar status you should use unicode character '…' instead of html entity (&#x2026 ; &#8230 ; &hellip ;) e.g. 'Uploading…'

## When to comment a string at Transifex?

If you are struggling to translate a string feel free to add a comment including your question.

You like to discuss your thoughts? No problem, just invite your team members using @username.

## When to create an issue at Transifex?

Whenever you feel just a comment is not sufficient and you need information to help all other language translators feel free to mark your comment as an issue.

## What to do if I want to change a source string?

Sometimes you encounter a typo or some other spelling error inside a source string. Or you find an error or grammar issue. If so, feel free to file an issue by marking a comment as an issue, or, even better, go to GitHub and provide a PR (Pull request) to correct it.

Most translators are not familiar with coding tools like GitHub nor have any coding background. It is though easy enough to make a GitHub account and navigate to the related repository. From there you can file issues directly where coders see it, get help, and learn to fix things on your own. GitHub has a bigger community since it is more integrated in the workflow.

# Information for Project Maintainers
## How to handle new language requests?

Nextcloud wants to cover the world. To reach this target as many languages as possible need be covered.
Luckily every week we get new language requests. Great. But do not simply accept it. 
Please check if similar languages are already there. If so, check the team size and send a personal message to the language requester. Tell him/her about the language you found, provide link to team and ask her/him to join named team.

...


## How to work on issues


...

# Information for German Team Members (in German)

## Wie kann ich mich beteiligen?
Schön, dass Du Lust hast hier etwas beizutragen. Nextcloud ist ein tolles Projekt dazu. 
Melde Dich bei Transifex an. Trete den deutschsprachigen Teams bei, schaue Dich um. Hast Du Fragen, dann wende Dich im Forum an uns (Links folgen noch).

## Wieso zwei Sprachen?
Für die deutsche Sprache gibt es zwei Übersetzungen bei Transifex. Diesen Luxus und Aufwand gönnen sich aktuell nur die Deutschen. Die Mitgliederzahl ist stark und der Übersetzungsgrad hoch.

In Deiner Nextcloud kann jeder Benutzer seine Sprache in den persönlichen Einstellungen vornehmen (nicht global).

Die Language-Codes mit deren Zuordnung wurden vom Nextcloud-Projekt festgelegt.

Habt Ihr generelle Fragen zur Übersetzung der deutschen Sprachen? Dann schaut hier:
 https://help.nextcloud.com/t/german-translation-endless-thread-in-german/7181

### Die formelle Übersetzung (Sie-Form).

Link: https://www.transifex.com/nextcloud/nextcloud/language/de_DE/

Language code: de_DE

### Die informelle Übersetzung (Du-Form).

Link: https://www.transifex.com/nextcloud/nextcloud/language/de/

Language code: de

## Infos für Reviewer
Immer an die beiden Sprachen denken.

Die sachliche Formulierung anwenden, nicht die persönliche:

Beispiele ...


## Infos für Übersetzer

Am besten erstmal eine Übersicht auf Transifex verschaffen. Auch die Begriffe im Glossar nachschlagen.
Ideen und Vorschläge im [Forum](https://help.nextcloud.com/c/translations/deutsch) diskutieren.

Wenn ein String übersetzt wird, dann immer beide Sprachen pflegen. Das führt zu einem konsistenten Übersetzungsgrad und spart die Nacharbeit.

Details im nächsten Absatz.

## Angleichen der Übersetzungen
Das pflegen von zwei deutschen Übersetzung ist aufwendig. Damit die Übersetzungen nicht auseinander laufen, sollten immer beide Sprachen übersetzt werden. Praktisch bedeutet dies, das ein Übersetzer nicht nur in der von ihm bevorzugten Form (Du oder Sie) übersetzen sollte, sondern auch die andere Form pflegen soll.

Aktuell gibt es einige Unterschiede. Die Reviewer kennen das, wenn sie beide Sprachen zeitgleich reviewen.

## Besonderheiten der mobilen Apps
### iOS-App
In der Apple-Welt wird die Sie-Form empfohlen und es kann nur eine deutsche Übersetzung für die Sprachauswahl "deutsch" herangezogen werden. Das App-Team hat entschieden die Sie-Form zu verwenden. Daher ist eine Übersetzung für die Du-Form nicht notwendig. Daher wird bei allen Strings der Du-Form der String "" eingetragen. Vorteil: Auch Personen die selten an den Übersetzungen mitarbeiten verschwenden keine Energie für Nicht-Verwendete Übersetzungen.

Link zur relevanten Sprache: https://www.transifex.com/nextcloud/nextcloud/language/de_DE/

### Windows Phone-App
Auch hier wird, wie bei iOS, nur die Übersetzung in der Sie-Form benötigt. 

Link zur relevanten Sprache: https://www.transifex.com/nextcloud/nextcloud/language/de_DE/

### Android-App
In Android ist nur eine Form für die deutsche Sprache möglich. Deswegen hat das Android-Team beschlossen, nur die formelle Anrede zu verwenden.

Umsetzung erfolgt. rakekniven 2018-05-23

Link zur relevanten Sprache: https://www.transifex.com/nextcloud/nextcloud/language/de_DE/

## Anmerkungen zu Transifex
Diskussionen auf Transifex sind schwer zu führen. Man kann sich Nachrichten schreiben, allerdings nur zwei Personen. Man kann aktuell keine weiteren Personen zu Diskussionen einladen.

