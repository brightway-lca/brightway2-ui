bw2-browser commands
====================

Project related
----------------

lpj
^^^

List the available projects.


Database related
-----------------

ldb
^^^

List the available databases.

db
^^

Select a different database by name. ::

        db biosphere

Activity related
-----------------

a
^
Select an activity by providing the id. ::

        a 101

aa
^^
Display all the activities in a database.

b
^
List biosphere flows of selected activity.

i
^
Show basic information of an activity.
When available, the following information is shown:

+ name
+ Database
+ ID
+ Product
+ Production amount
+ Location
+ Classifications
+ Number of Technosphere inputs
+ Number of Biosphere flows
+ Number of reference flows used by the activity

ii
^^
Show extended information about the activity.
All the metadata of the activity is shown. This includes the basic information.

s
^

Search in the currently selected database an activity.
It accepts the modifier ``-loc {A_LOCATION}`` to search only activities matching the location. ::

        s -loc {MX} oil

r
^

Randomly select one activity from the currently selected database.

d
^
Show downstream activities of the selected activity.

u
^
Show upstream activities of the selected activity.

uu
^^
Show upstream activities *extra information like formulas* of the selected activity.

Methods related
----------------

lm
^^

List available methods.

mi
^^

Show the currently selected method metadata. Only works for a full Method, category and subcategory.

cfs
^^^

Print the characterisation factors of the selected method for the currently selected activity.

Parameters related
------------------

lpam
^^^^

List all (Project, Database, Activity) parameters.

lpamg
^^^^^

List parameter groups.

ap
^^
List the parameters of the currently selected activity.
dp
^^
List the parameters of the currently selected database.
pp
^^
List the parameters of the currently selected project.

fp
^^
Find a specific parameter by name.

sp
^^
Search for a parameter by name, accepting wildcards in arg.

Calculation related
--------------------

G
^

Do an LCA of the selected activities and methods.
At least one method and one activity must be selected.

ta
^^

Display top activities contributing to the lca score if an lca is active (after using the ``G`` command).

te
^^

Display top emissions contributing to the lca score if an lca is active (after using the ``G`` command).

Misc
----

q
^
Exit the browser

quit
^^^^
Exit the browser

h
^

Show the history of database and activities.

help
^^^^

Show a summary of the available commands.

l
^
List current options. Useful after a search for example.

n
^
Go to the next page of options. Useful when navigating over search results.

p
^
Go to the previous page of options. Useful when navigating over search results.

web
^^^

Start the web application.

.. note:: Currently broken

wh
^^

Write the history of commands used in the cli tool.

.. note::
        currently broken.
