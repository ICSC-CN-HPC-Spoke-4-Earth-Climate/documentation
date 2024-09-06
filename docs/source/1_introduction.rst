============
Introduction
============

--------------------------
Aim and General Principles
--------------------------

`Git <https://git-scm.com/>`_ is a free and open-source
distributed version control system, that tracks changes in files,
and is particularly useful when different people are working
on the same file at the same time.
`GitHub <https://github.com/>`_ is a web-based platform
which provides hosting for Git repositories,
extending the functionalities of Git with a web-based graphical interface
and many other features like issue tracking and pull requests.
It enables code sharing and collaborative work,
fostering the revision process, allowing the integration of
different development lines without impacting the
functionalities of the production code,
and providing instruments to solve conflicts.

The aim of having a common space to gather the code
produced within Spoke 4 - Earth & Climate of the
ICSC - Italian Research Center on High Performance Computing,
Big Data and Quantum Computing is to provide a centralized space
for tracking code development, facilitate the sharing and coordination of efforts,
and preserve the assets built during the project's development.

It is assumed that the project developers have at least a basic understanding
of version control principles and fundamental Git and GitHub operations.

Being a large and heterogeneous project, involving tasks organized
into 5 Work Packages and several Innovation Grants,
the creation of a single repository
with a tree structure to collect the produced code is deemed too rigid.
This approach would inhibit the necessary management flexibility,
interfering with the day-by-day work of the various developers, also adding
a significant workload to administrators in charge of managing such infrastructure.
Taking into account the nature of the project,
the creation of a
`GitHub Organization <https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/about-organizations>`_
is considered more appropriate.
A GitHub organization is a shared account, serving as a container
for multiple repositories, which can be given a unique name and brand.
Organizations enable to define a hierarchy of roles
for the personal accounts joining it,
allowing a subset of people to granularly manage
the access to the organization resources.
This solution allows individual working groups
to organize their repositories according to specific needs,
while leaving control of the overall structure and organization
roles to a restricted group of administrators.

----------------------
Organization Structure
----------------------

The structure of a GitHub organization revolves
around **Teams**.
Teams are groups of organization members that can be
effectively utilized to control member permissions.
It is possible to create nested teams to reflect
the actual structure of working groups.
More details about GitHub Teams can be found :ref:`here <Teams>`.

Considering the structure of the Spoke's working groups,
a hierarchy of teams has been deployed.
The following figure illustrates such structure.

.. fig_organization_structure:

.. figure:: images/CN-HPC_GitHub_organization_structure_v2.png
   :name: organization_structure
   :width: 734
   :height: 417
   :alt: ICSC CN HPC Spoke 4 GitHub Organization structure

Five primary teams (**1st-Level Teams**) have been created, corresponding to
the five work packages of Spoke 4.
These teams are designed to bring together all the individuals
involved in or collaborating on the activities within
each work packages.
Additionally, a team has been created to group the developers
working on the Innovation Grants activities.
For each 1st-level team, two Organization members are required to be *team maintainers*
(more on this :ref:`here <par_team_maintainers>`).
Maintainers are able to manage team memberships and settings.
This approach ensures the necessary autonomy
for the individual work packages and innovation grants,
providing the Organization with the required operational flexibility.

The structure of the undelying level (**2nd-Level Teams**) is as follows:

* For the Work Packages 1st-Level Teams, the structure can be 
  discussed and adapted based on specific needs. 
  Common strategies include creating 2nd-Level Teams corresponding to:
  
  - The Project Proposal tasks
  - The institution involved
  - The thematic or disciplinary areas involved

* For the Innovation Grants 1st-Level Team, a separate 2nd-Level Team is created
  for each Innovation Grant requiring access to the Organization.

The lowest level of the hierarchy (**3rd-Level Teams**) includes
teams that group the Organization members working on
each code repository.
These teams have a 1-to-1 correspondance with these repositories and
are created alongside them upon request from an Organization member 
(see the Section :ref:`Request the creation of a new repository` for instructions
on how to request a new repository).

.. note::
  The ability to create child teams is disabled for the ICSC Spoke 4
  GitHub organization members.


-----
Roles
-----

Within a GitHub organization, it is possible to define **Roles**.
Roles are a set of permissions that can be assigned to individuals or teams.
A permission is the ability to perform an action on GitHub.
There are three types of roles:

#. **Organization-level:** management of the entire organization and its settings, teams, and repositories.
#. **Team-level:** team management.
#. **Repository-level:** creation and access to repositories.

Organization-level roles are meant to control members' access
to the organization and its resources.
Two organization roles are relevant to the ICSC Spoke 4 GitHub Organization:

* **Organization Member**: default, non-administrative role.
* **Organization Owner**: complete administrative access.

The owners of the ICSC CN HPC Spoke 4 GitHub Organization are appointed
by the coordination of the Spoke.
About 3-4 members are selected for this role,
to ensure the necessary stability and continuity in the management
and long-term maintenance of the Organization and the connected repositories.
Organization owners can create repositories, configure their settings,
delete them, and perform other relevant operations.

Team-level roles allow members to manage a team.
Any organization member can be assigned the role of team maintainer,
granting them administrative permissions over the team.
For more information check out :ref:`here <par_team_maintainers>`.

The access to each repository can be defined by
`repository-level roles <https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization>`_.
The following table provides a summary of the different possibility:

+----------+---------------------------------------------------------------------------------------------------+
| Role     | Description                                                                                       |
+==========+===================================================================================================+
| Read     | View the repo (for non-code contributors)                                                         |
+----------+---------------------------------------------------------------------------------------------------+
| Triage   | NO write access. Manage issues, discussions, and pull requests                                    |
+----------+---------------------------------------------------------------------------------------------------+
| Write    | Push to the repo (for active contributors)                                                        |                        
+----------+---------------------------------------------------------------------------------------------------+
| Maintain | Manage the repository without access to sensitive or destructive actions (for project managers)   |
+----------+---------------------------------------------------------------------------------------------------+
| Admin    | Full access to the repo, including sensitive and destructive actions (security settings/deletion) |
+----------+---------------------------------------------------------------------------------------------------+

Within the ICSC CN HPC Spoke 4 GitHub Organization, repository level roles
are assigned to teams as follows:

* 3rd-Level teams: **Write** access to the corresponding repository.
* 2nd-Level teams: **Read** access to the corresponding group of repositories.


-------------------
Repository Policies
-------------------

Each ICSC CN HPC Spoke 4 GitHub Organization member 
can request the creation of a new repository
(see the Section :ref:`Request the creation of a new repository`)
or the trasfer of an existing repository to the Organization.

.. important::
  To protect the Organization's data, **the ability to create repositories
  is restricted to Organization owners only.**

The following general policies apply to the repositories within the 
ICSC CN HPC GitHub Organization :

* Throughout the project, the repositories can be kept private
  (and are private by default).
* At the end of the project the repository will be made public.
  The scientific coordination of the Spoke or the WP leaders
  can decide to make part of the code
  within a repository public during the project lifetime.
* Each repository should contain and 
  track the development of a defined, independent 
  set of programs designed to perform a specific task.
  Considering the diverse needs of the developers involved 
  in the Spoke, a common layout is not strictly required.
  Nevertheless, GitHub
  `best practices <https://docs.github.com/en/repositories/creating-and-managing-repositories/best-practices-for-repositories>`_
  are recommended, particularly the creation of a README file
  specifying the purpose of the code contained in each repository.
