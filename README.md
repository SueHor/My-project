
# AI autoordering another ticket when in a hurry

Final project for the Building AI course

## Summary

When user is on their way to perhaps a train station, the AI looks after them and when there is a possibility that the user might miss their train, AI orders a ticket for a later train and if the user gets to their train in time, AI cancels the other ticket. The user can focus only on their way of transportation to the station without other worries.


## Background

It solves user´s worry about not being physically able to order another ticket (due to crowded bus etc.) + AI will know better than the user that there was perhaps an accident and that it will slow their way to the station.
For people who have many responsibilities - it is more frequent to be late and miss the method of transport.
Personal motivation - I was once almost too late for the train. Due to traffic I was able to sprint to the train only in time for the door to close right behind me. I made it in time only due to my knowledge of "where I get on the underground" and "where do I need to get off to follow the shortest way possible". I was not able (due to crowded space in a bus) to book another ticket and since the other train was leaving about 15 minutes after my (the first) train, it would be for the best if, in case I did not make it to my train in time, I 1. knew that I have another train available, 2. already had a ticket for it, 3. knew where to go.

AI responsibilities:
* Watch the traffic situation ahead
* Calculate the possibility of being late
* Book another ticket (simmilar price would be better)
* Cancel original ticket (when no possibility of arrival on time) OR cancel new ticket (when arrival on time)
* etc.


## How is it used?

When buying a ticket - user can decide if they want to use AI in case of being late. They can also decide if they want AI to watch for other trainstations in the city (if there are any) in the case of "no train available" or "no suitable train in time available".
User is on their way to the train via public transport. AI watches (via cellphone data of other users) if there is a possibility of being late to the train station. AI watches out for traffic, accidents etc.. When there is a high possibility of being late (calculated with average speed of the user - speed would be different in case of a young person and a senior citizen) due to traffic, AI orders a new ticket to a later train (for a simmilar price as the original ticket if possible) and when there is absolutely no chance of getting to the orginal train in time, AI cancels the ticket and informs the user about the change in advance (with new platform number if possible). In case the user gets to their train in time, AI cancels the new ticket.


## Data sources and AI methods

I would use data from:
* The user - if they want AI to decide with precision, they can add "speed of walking" to their profile etc.
* The traffic situation (like googlemaps) - via cellphone coverage in certain places, we are able to recognize traffic.
* Train station schedules - current lateness of the train, departing and arrival times.

## Challenges

* Financial situation - user might not have enough money in their account to reserve two tickets at one time.
* Cancel time for tickets - every method of transport have different policy of ticket cancelation.
* Adrenalin and running - user who does not usually sprint (e.g.) might have their ticket canceled because the AI did not predict that the user is able of arriving on time.
* Forgetfullness - when user forgets their device at home, AI might think they are late and cancel their ticket.
