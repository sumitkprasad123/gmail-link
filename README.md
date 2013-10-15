This is a scratch project to attempt to extract a reliable HTML href link to Google Mail messages.

Motivation
----------

The Todoist application previously created a text entity capable of opening an individual Google Mail message, for the purposes of including that message in the text body of a task.  This Google Mail reference was further capable of linking to any Google Mail domain account (e.g.: jake@umn.edu) when another Google Mail domain (e.g.: jake.gage@gmail.com) was used as an authenticating service for Todoist.

This behavior was highly useful and desirable, as it allowed for linking a task to a Google Mail conversation thread for later processing or clairification of the task.  This could be accomplished by authenticating Todoist to the domain of a source email to be linked (e.g.: jake@umn.edu), using the Todoist Chrome plugin to generate the text entity, and copying this enitity to any Todoist account (e.g.: jake.gage@gmail.com).

The added step of authenticating to the Todoist account domain for the source email address was undesirable, but not an undue burden.

This behavior has changed in Todoist.  Todoist now creates a non-text DOM entity, which may not be copied through standard means.  This seems to effectively disable the process for attaching an email in a Google Mail domain which differs from the Google Mail domain used to authenticate the Todoist Chrome plugin.