***************
Member's How-to
***************

First steps
===========

After receiving and accepting the invitation 
to join the Organization, members can access 
the Organization's web pages.
The `main page of the Organization <https://github.com/ICSC-CN-HPC-Spoke-4-Earth-Climate>`_
can be reached by using the link in the left sidebar 
of each member's GitHub main page, 
under the section **Organizations.**
In the invitation phase, each prospective member 
is assigned to their respective 1st-Level and 
to the relevant 2nd-Level team(s).

After being added to the Organization, members 
can request the creation of new repositories 
(:ref:`Request the creation of a new repository`).
For each repository, an organization member 
is required to be the **manager**, i.e. the person
responsible for the repository and the associated working group.
Each repository is associated with a 3rd-level team 
(see Figure :ref:`fig_organization_structure`
for a schematic of the Organization structure. 
A detailed description can be found
in Section :ref:`Organization Structure`), 
which is meant to group the Organization members 
working on the code contatined within.

.. note::
   3rd-level teams and repositories have a 
   1-to-1 correspondence and share the same name.

The repository manager is the **maintainer** 
of the corresponding 3rd-level team.
This role grants them the authority to add and remove 
members of the Organization to/from the team.
In this way, they can control the group of collaborators 
who can actively contribute to the development of 
the code within the repository, provided that 
these collaborators are members of the Organization.

To summarise the typical case, after joining 
the Organization and once some repositories 
have been set up, each member is:

#. A member of their 1st-Level team.
#. A member of the 2nd-level team(s) associated with the institution they belong to,
   or the activities/tasks they are involved in.
#. A maintainer of 3rd-level teams corresponding to
   the repositories they are responsible for
   (i.e. repository manager).
#. A member of 3rd-level teams corresponding to
   repositories they can access and participate 
   in the development of 
   (but for which they are NOT responsible).

These roles ensure the user a set of permissions on repositories.
This is because access to individual repositories 
is not granted to individual user accounts
but to Organization teams, following the policy below:

* 3rd-level teams: **write** permissions on 
  the corresponding repository.
  This enables the actual working group to 
  autonomously manage the contents 
  of the respective repository.
* 2nd-level teams: **read** permission for all 
  the related repositories.
  This is intended to promote and strengthen collaboration 
  between the project's groups focusing on similar topics.


.. _fig_organization_structure:

.. figure:: ../images/CN-HPC_GitHub_organization_structure_v2.png
   :name: organization_structure
   :width: 734
   :height: 417
   :align: center 
   :alt: ICSC CN HPC Spoke 4 GitHub Organization structure

   ICSC CN HPC Spoke 4 GitHub Organization structure


Request the creation of a new repository
========================================

After joining the Organization, each member 
can request the creation of a new repository.
The request involves opening a dedicated 
`issue <https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues>`_, 
following the procedure outlined below.

#. In the repository `administration <https://github.com/ICSC-CN-HPC-Spoke-4-Earth-Climate/administration>`_ 
   open the **Issues** tab.
#. Click **New Issue**, then click the 
   **Get started** button in the 
   **Repository Creation** template.

   .. figure:: images/repo_creation_template.png
      :width: 600
      :height: 50
      :align: center
      :alt: Repo creation template.

   .. attention::
      When requesting the creation of a new 
      repository related to an innovation grant,
      please use the corresponding issue template.

#. Fill in the fileds in the title and 
   description of the issue.

   .. figure:: images/repo_creation.png
      :width: 600
      :height: 370
      :align: center 
      :alt: Repo creation issue snapshot.

   Please fill in all the fields in <> brackets 
   without deleting any lines.
   If no collaborator exists at the time the 
   repository is created,
   please leave the corresponding line empty 
   (i.e. delete everything between the squared 
   brackets, including the brackets).
   Leave the *assignees* set to the Organization 
   owners and the *label* set to *new_repo*.
   Below is an example of a correctly 
   compiled request.

   .. figure:: images/repo_creation_ok.png
      :width: 604
      :height: 370
      :align: center
      :alt: Repo creation issue snapshot.

#. After completing the request, click **Submit new issue**.

The Organization owners will take care of 
creating the new repository 
and the related 3rd-level team.
After this, please check that the access 
permissions to the repository are correctly set 
(the 3rd-level team should have write access 
to the repository, and the 2nd-level team 
should have read access).
The repository manager can add 
Organization members to the 3rd-level team, 
thereby granting them
write access to the repository.


Authentication to GitHub
========================

In daily use, developers typically work on 
code saved on their local machines and then 
push the changes they make to their code on GitHub.
To perform this operation, assumed to be done 
via the command line, it is necessary to use 
one of the authentication methods offered by GitHub.

Authentication is the process of supplying or 
confirming credentials unique for each user,
proving that a user is indeed who they claim to be.
On GitHub, this process can occur in various ways.
An extensive guide on authentication can be found on the webpage
`About authentication to GitHub <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github>`_.


Personal Access Tokens
----------------------

For simplicity, it is recommended to access 
the Organization's repositories from the 
command line using HTTPS.
To this end users must use 
**personal access tokens (PATs)** 
in place of passwords.

.. important::
   Whenever Git prompts for a password, 
   the PAT must be entered instead.

A comprehensive guide on this topic is 
available in the GitHub documentation
(`Managing your personal access tokens <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens>`_). 
However, a concise guide is provided below,
to assist users who require write access 
to repositories within the Organization.

Two types of PATs exist:

* Fine-grained PATs
* PATs (classic)

In the ICSC CN HPC Spoke 4 Organization, 
PATs (classic) have been restricted.
Therefore, only the use of fine-grained PATs is allowed.
To create a fine-grained PAT, 
users must follow these steps:

#. `Verify their email address <https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/verifying-your-email-address>`_
   (if it has not been verified yet).
#.	On any page, click their profile photo (upper-right corner) > **Settings.**
#.	On the left sidebar click **Developer settings** > dropdown menu **Personal access tokens** > **Fine-grained tokens.**
#. Click the button **Generate new token** (top-right button).
#.	Set the token name, expiration, resource owner, repository access and permissions according to the table in Section :ref:`Token Request Details`.
#.	In the **Overview** section, review the request and submit.

After receiving approval from the Organization, 
the token can be utilized instead of a password 
for accessing the repository from the command line.

.. caution::
   Maintaining the security of PATs is crucial!
   They should be treated with the same care as passwords.


Token Request Details
^^^^^^^^^^^^^^^^^^^^^

+---------------------+----------------------------------------------------+
| Token name          | <repo-name>_<username>                             |
+---------------------+----------------------------------------------------+
| Expiration          | Any option                                         |
+---------------------+----------------------------------------------------+
| Resource owner      |	ICSC-CN-HPC-Spoke-4-Earth-Climate                  |
+---------------------+----------------------------------------------------+
| Justification       | Enter a justification for the request              |
+---------------------+----------------------------------------------------+
| Repository access   |	Only select repositories                           |
+---------------------+----------------------------------------------------+
| Select repositories |	Name of the (**single**) repository to access      |
+---------------------+----------------------------------------------------+
| Permissions         | Repository permissions > Contents > Read and Write |
+---------------------+----------------------------------------------------+


Notes:

* Please adhere to the specified 
  format for the token name.
* The Organization must be specified 
  as the resource owner.
* Metadata read-only permission will 
  be automatically added to the request.
* As each token needs approval, 
  please provide a justification for it 
  (e.g. “Code development repository XXXX”).
* For management reasons, it is required 
  to generate a separate token for each repository.
