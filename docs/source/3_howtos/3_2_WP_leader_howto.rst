****************************
Work Package Leader's How-to
****************************

This guide is intended for the Project 
Work Package (WP) Leaders
who wish to set up an infrastructure
within the ICSC CN HPC Spoke 4 
GitHub Organization to host
the code produced during the activities
they oversee.
Leaders of Innovation Grants should
also follow these guidelines when 
requesting access to the Organization.


Teams Hierarchy
===============

.. note::
   Check out :ref:`Teams` for a brief description of what a team is
   and what the role of a team maintainer is.

Within the ICSC CN HPC Spoke 4 GitHub organization, 
the teams hierarchy is organized to mirror 
the structure outlined in the project proposal.
For safety and organizational reasons, 
the authority to create teams
is reserved for the Organization owners.

A three-level hierarchy has been implemented,
as described below:

.. figure:: ../images/CN-HPC_GitHub_organization_structure_v2.png
   :name: organization_structure
   :width: 734
   :height: 417
   :align: center 
   :alt: ICSC CN HPC Spoke 4 GitHub Organization structure

#. **Level 1: Work Packages/Innovations Grants**
   Each Work Package team consists of
   developers working 
   within the same WP.
   The *Innovation Grants* team groups
   all Organization members
   involved in one of these grants. 
   Each WP team is assigned two maintainers,
   appointed by the WP leader.
   No maintainers are assigned 
   to the *Innovation Grants* team.
#. **Level 2: Task/Thematic Area/Institution**
   The second level of the hierarchy
   is designed to adapt to the needs
   of the research groups involved 
   in the project.
   To encourage the sharing of code assets 
   produced, it is recommended to create 
   teams that reflect the project tasks.
   However, teams can also be organized 
   by grouping members affiliated
   with the same institution,
   or those working on similar
   thematic or disciplinary areas.
   The decision on how to organize 
   second-level teams is delegated to the
   work packages and innovation grants leaders.
   When requesting access to the Organization,
   WP/innovation grant leaders must 
   communicate the desired second-level 
   structure to the organization owners.
   Additionally, they should specify two 
   Organization member for each second level 
   team who will become team maintainers
   (for teams related to the project
   work packages, these member may,
   but are not required to, be the same 
   as the WP team maintainers).
   As the ability to create child teams
   is disabled for Organizazion members,
   Organization owners
   will be responsible for implementing
   the desired second-level structure.
    
#. **Level 3: Work Groups.**
   These teams are meant to group developers working on a single repository.
   They can consist of a single person, up to an arbitrary number of people.
   At least one organization member is required to be maintainer
   of each of these teams.
   Ideally, the maintainer should be the main developer of the code
   within the repository
   (akin to the owner of a personally held GitHub repository).



Memberships & Teams Management
==============================

If one or more individuals or work groups 
within a project Work Package or Innovation Grant
wish to use the ICSC CN HPC Spoke 4 GitHub Organization,
the WP (Innovation Grant) leader must contact 
the Organization owners and provide the following:

#. The desired structure of the 2nd level
   teams.
#. The **GitHub usernames** of the two
   maintainers for the 1st level team
   and each of the 2nd level teams.
   The following table can be
   used as a guide:

   +-----------------------+------------------+------------------+
   |                       | **Maintainer 1** | **Maintainer 2** |
   +=======================+==================+==================+
   | WP team               |                  |                  |
   +-----------------------+------------------+------------------+
   |  **2nd Level Teams**  |                  |                  |
   +-----------------------+------------------+------------------+
   | 2nd level team XXXX 1 |                  |                  |
   +-----------------------+------------------+------------------+
   | 2nd level team XXXX 2 |                  |                  |
   +-----------------------+------------------+------------------+
   | ...                   |                  |                  |
   +-----------------------+------------------+------------------+

   The Innovation Grants leaders 
   should provide only the GitHub 
   usernames of the two maintainers 
   for the corresponding team.
#. The list of developers who wish 
   to become member of the Organization,
   including their first and last names, 
   affiliation, GitHub username and 
   contact email address.
   WP leaders must also specify
   the 2nd-level team(s) that each
   member will join.
   The table below provides
   an example of such a request:

   +-------+------+-------------+----------+---------+-----------+
   | First | Last | Affiliation | GitHub   | Contact | 2nd-level |
   | Name  | Name |             | Username | Email   | Team(s)   |
   +=======+======+=============+==========+=========+===========+
   |       |      |             |          |         |           |
   +-------+------+-------------+----------+---------+-----------+
   |       |      |             |          |         |           |
   +-------+------+-------------+----------+---------+-----------+
   |       |      |             |          |         |           | 
   +-------+------+-------------+----------+---------+-----------+


.. important::

   Each developer must already possess their own personal GitHub account!


The Organization owners will set up the requested 
team structure and send invitations to join 
the Organization to the interested developers. 
The developers will have 7 days to accept the invitation, 
after which it will expire. 
During the invitation phase, 
each prospective member will be assigned 
to their respective 1st and 2nd-level teams.

.. warning::
   
   Please note that being a member of a 2nd-level 
   team grants **read** permissions to 
   all related repositories.


Individual developers can submit requests 
to join the Organization at a later time 
by directly contacting the Organization's owners 
- with the WP/Innovation Grant leader copied (Cc) -
and providing the necessary information.

Once developers have joined the Organization, 
team maintainers can add or remove them 
from the teams they manage.

.. note::
   Membership in a child team does not 
   automatically confer membership in the parent team.
   Therefore, each member must be added individually 
   to each team at every level.


Repositories Management
=======================

.. important::
  To protect the Organization's data, **the ability to create repositories
  is restricted to Organization owners only.**


Each Organization member can request 
the creation of a new repository or 
the transfer of an existing repository 
to the Organization. 
For detailed instructions on requesting 
the creation of a new repository 
within the ICSC CN HPC GitHub Organization, 
see the section :ref:`Request the creation of a new repository`.

