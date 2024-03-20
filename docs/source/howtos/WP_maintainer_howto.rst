===========================
WP Team Maintainer's How-to
===========================

Teams Hierarchy
---------------

.. note::
   Check out :ref:`Teams` for a brief description of what a team is
   and what the role of a team maintainer is.

Within the ICSC Spoke 4 GitHub organization, the teams hierarchy
is organized to mirror the structure outlined in the project proposal.
For safety and organizational reasons, the authority to create teams
is reserved for the Organization owners.

A three-level hierarchy has been implemented:

#. **Level 1: Work Packages.**
   Each of these teams brings together developers
   working within the same WP.
   Each WP team is assigned two maintainers,
   appointed by the WP leader.
#. **Level 2: Task/Thematic Area/Institution.**
   The second level of the hierarchy
   is designed to adapt to the needs
   of the research groups involved in the project.
   To encourage the sharing of code assets produced within the project,
   it is recommended to create teams reflecting the project's tasks.
   However, teams can also be organized by grouping individuals
   working within the same institution.
   The decision on how to organize second-level teams is delegated to WP leaders
   and must be communicated to organization owners.
   When requesting access to the Organization,
   WP leaders must write to the organization owners,
   requesting the implementation of the desired second-level structure.
   Additionally, they should specify two members
   for each of the second level teams,
   who will become team maintainers
   (possibly but not necessarily the same members
   appointed as WP team maintainers). 
#. **Level 3: Work Groups.**
   These teams are meant to group developers working on a single repository.
   They can consist of a single person, up to an arbitrary number of people.
   At least one organization member is required to be maintainer
   of each of these teams.
   Ideally, the maintainer should be the main developer of the code
   within the repository
   (akin to the owner of a personally held GitHub repository).

Memberships, Teams & Repositories Management
--------------------------------------------

If one or more individual/work group within the WP
wish to utilize the ICSC Spoke 4 GitHub organization,
the WP leader must contact the Organization owners, providing:

#. The GitHub usernames of the two maintainers for the WP team,
   the structure and GitHub usernames of maintainers for the 2nd level teams.
   The following table can be used as a guide:
      
   +-----------------------+--------------+--------------+
   | Token name            | Maintainer 1 | Maintainer 2 |
   |                       |              |              |
   +=======================+==============+==============+
   | WP team               |              |              |
   +-----------------------+--------------+--------------+
   |                       |              |              |
   +-----------------------+--------------+--------------+
   | 2nd level team XXXX 1 |              |              |
   +-----------------------+--------------+--------------+
   | 2nd level team XXXX 2 |              |              |
   +-----------------------+--------------+--------------+
   | ...                   |              |              |
   +-----------------------+--------------+--------------+

#. The list of developers who are willing to become member of the organization,
   specifying name, family name, affiliation,
   GitHub username and a contact email address.
#. The list of repositories to be created, providing the name,
   the associated project task,
   and the GitHub username of the person responsible for the repository.

For convenience, points 2 and 3 can be done using a spreadsheet
provided by the organization's owners, which contains the following fields:

+-----------+-----------+-------------+-----------------+---------------+------+-----------------+--------------------+
| First Name| Last Name | Affiliation | GitHub Username | Contact Email | Task | Repository Name | Repository Manager |
+===========+===========+=============+=================+===============+======+=================+====================+
|           |           |             |                 |               |      |                 | ✔/✘               |
+-----------+-----------+-------------+-----------------+---------------+------+-----------------+--------------------+
|           |           |             |                 |               |      |                 | ✔/✘               |
+-----------+-----------+-------------+-----------------+---------------+------+-----------------+--------------------+
|           |           |             |                 |               |      |                 | ✔/✘               |
+-----------+-----------+-------------+-----------------+---------------+------+-----------------+--------------------+


