============
Introduction
============

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
into 5 Work Packages, the creation of a single repository
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

.. fig_organization_structure:

.. figure:: CN-HPC_GitHub_organization_structure.png
   :name: organization_structure
   :width: 604
   :height: 306
   :alt: map to buried treasure

   ICSC CN HPC Spoke 4 GitHub organization structure.

Organization Structure
----------------------

The Structure of a GitHub organization revolves
around **Teams**.
Teams are groups of organization members that can be
effectively utilized to control member permissions.
It is possible to create nested teams to reflect
the actual structure of working groups.
More details about GitHub Teams can be found :ref:`here <Teams>`.

Considering the structure of the Spoke's working groups,
a hierarchy of teams corresponding to the project proposal has been deployed.
Figure :ref:`fig_organization_structure` illustrates such structure.
The fine structure can be discussed and adapted based on
the needs of individual work packages
Five primary teams (**Work Packages Teams**) have been created, corresponding to
the five work packages of Spoke 4.
These teams are designed to bring together all the individuals
involved in or collaborating on the activities within
each work packages.
For each WP team, two member are required to be team maintainers
(basic concept :ref:`here <par_team_maintainers>`).
Maintainers will be able to manage team memberships and settings.
This approach ensures the necessary autonomy for individual work packages,
providing the organization with the required operational flexibility.

Roles
-----

Within a GitHub Organization, it is possible to define **Roles**.
Roles are a set of permissions that can be assigned to individuals or teams.
A permission is the ability to perform an action on GitHub.
There are three types of roles:

1.	**Repository-level:** creation and access to repositories.
2.	**Team-level:** team management.
3.	**Organization-level:** management of the entire organization and its settings, teams, and repositories.

Organization owners can create repositories, configure their settings,
delete them, and perform other relevant operations.
The access to each repository can be defined by `repository-level roles <https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization>`.
The following table provides a summary of the different possibility:
