===========================
Kim Lab Computing Resources
===========================

.. contents::
    :local:

Here is an overall list of computing resources available to students in the Paton lab

But first, here are some tips for accessing these computers:

* ssh is a fundamental command used to virtually log into a system
* $USER in all these example commands should be replaced with your username on these computers
* You will need to create accounts on all of these computers to gain access
* I recommend setting up aliases in your ~/.bashrc or ~/.bash_profile or ~/.zshrc
   * Aliases are shortcuts for bash commands
   * Using aliases to log into different computers can save time and confusion

Expanse and Bridges2
--------------------

We typically apply for an ACCESS grant each year to get compute time on the 
**Expanse** and **Bridges2** clusters.

The following aliases will allow you to type ``expanse`` or ``bridges2`` into 
your terminal and immediately ssh to that computer. 

.. code:: shell

    alias expanse='ssh $USER@login.expanse.sdsc.edu'
    alias bridges2='ssh $USER@bridges2.psc.edu'

.. note:: 

    You will still have to type in a password, but this will allow you to avoid 
    typing the long hostname each time you want to access another computer.

Before you can access either of these computers, you will have to create accounts 
for both **Expanse** and **Bridges2**, as well as ACCESS in order to use the resources.

.. note:: 

   Make sure you know your username on each of these computers, as it may be 
   different than what you normally use depending on how the account is created.

You can follow these websites to make accounts on 
`Expanse <https://www.sdsc.edu/index.html>`__, 
`Bridges2 <https://www.psc.edu/>`__, and 
`ACCESS <https://access-ci.org/>`__.

Additionally, you will need to fill out 
`this form <https://www.psc.edu/resources/software/gaussian/>`__ to gain access 
to Gaussian, or email them for help.

You should also get in contact with an ACCESS admin in the group 
(Seonah as of March 2023) to be added to the allocations group for the lab.

Alpine
------

As CSU students, we have access to a shared cluster **Alpine** with CU Boulder 
(hosted in Boulder, CO).

In order to gain access to Alpine follow 
`this link <https://it.colostate.edu/research-computing-and-cyberinfrastructure/compute/get-started-with-summit/>`__.
Each time you log onto Alpine, you will need to run the command 
``module load slurm/alpine``. More information can be found 
`here <https://curc.readthedocs.io/en/latest/clusters/alpine/quick-start.html>`__.

The alias to log in to Alpine is:

.. code:: shell

    alias alpine='ssh $USER@colostate.edu@login.rc.colorado.edu'

You will be required to log in using your CSU NetID information 
(username and password), as wel as sign in with Duo. There are two ways to sign 
in with Duo to this computer: type ``password`` then enter in the 6-digit pin on
the Duo app, or type ``password,push`` which will send a Duo push notification 
to your phone.

.. note:: 

   Lets say that for illustrative purposes that your password is ``123456`` and 
   that you want a Duo push. Then you will type ``123456,push``. 

ACME 
----

**ACME** is a shared computer between the Paton and Kim labs. This computer has 
a queue system (sbatch) to allow for easy use for all students of the Theory Suite. 

There are also a number of premade submission scripts on ACME that are available
to help with running jobs.

Here is the alias for ACME:

.. code:: shell

    alias acme='ssh $USER@acme.chem.colostate.edu'

To gain access to ACME, contact an admin to make an account. The current admins 
are Yeonjoon, Collin, Sabari, and Guilian (March 2023).

Local Resources
---------------

The Kim lab also has a number of **local machines** available members to use. 
These machines do not have a queue system like many of the other computers do, 
but are useful for different tasks you may have. 

Here are aliases to the local CSU resources:

.. code:: shell

    alias falcon='ssh $USER@falcon.chem.colostate.edu'
    alias loki='ssh $USER@loki.chem.colostate.edu'

To get accounts on these computers, you will need to contact an admin. For the 
Kim lab, this is Yeonjoon, Sabari, Raul and Collin (March 2023).
    

