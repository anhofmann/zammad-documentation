Everything about the ticket
***************************

A ticket is a container for a conversation with the customer about one dedicated topic/issue.

Ticket states
=============

In default setup Zammad has the following ticket states:

* new

  * Ticket has been created by a customer, no agent has sent out a response to the customer yet
  * If an agent replies to the customer, the ticket will change its state to "open" automatically

* open

  * Ticket is open, an agent needs to work on it (e. g. close it or set a pending reminder state to let others know that somebody is working later on it)

* pending reminder

  * Tickets which will "sleep" (no further action/attention needed right now) till pending date is reached
  * Tickets will not escalate (in case of escalation, escalation is suspended)
  * The time where the ticket is in pending reminder is not counted for escalation

* pending close

  * Tickets which will "sleep" (no further action/attention needed right now) till pending date is reached
  * Tickets will not escalate (in case of escalation, escalation is suspended)
  * The time where the ticket is in pending close is not counted for escalation
  * After pending time is reached, the ticket will be closed by Zammad automatically

* closed

  * Ticket has been solved/finished, no further action/attention needed


Ticket colors
=============

Almost anywhere a ticket is being shown you will see a colored circle. The color tells you if the ticket needs attention:

* Orange

  * Ticket has been created, somebody needs to work on it
  * Pending reminder of ticket has been reached, somebody needs to work on it

* Red

  * Ticket is escalated, somebody needs to work immediately on this ticket to cancel escalaction state (e. g. needs to send out a customer response or set the ticket to pending reminder until somebody can solve the ticket)

* Green

  * Ticket is closed, no further action/attention needed

* Dark gray

  * Pending reminder or pending close has been set but not yet reached, no further action/attention needed right now
