===============
Member's How-to
===============

-----------
First steps
-----------

After receiving and accepting the invitation to join the Organization,
members can access the Organization's web pages.
The `main page of the Organization <https://github.com/CN-HPC-Spoke-4-Earth-Climate>`
can be reached by using the link in the left sidebar of each member's GitHub main page,
under the section 'Organizations'.
In the invitation phase, each prospective member is assigned to their
respective WP and to a series of lower-level teams.
Additionally, they will be given access to a series of repositories.
Specifically, each member is included as:

#.  Maintainers of 3rd level teams corresponding to
    the repositories they are responsible for.
#.  Members of 3rd level teams corresponding to
    repositories they can access and participate in the development
    (but they are NOT responsible for).
#.  Members of the 2nd level related to activities/tasks they are involved in.
#.  Member of their WP team.

Being a member of each of these teams ensures the user a set of permissions on individual repositories.
This is because access to individual repositories is not granted to individual user accounts
but to Organization teams, following the policy below:

*  3rd level teams: write permissions on the corresponding repository.
   This enables the actual working group to autonomously manage the contents of the respective repository.
*  2nd level teams: read permission for all the related repositories.
   This promotes and strengthens collaboration between the project’s groups focusing on similar topics.

Please note that 3rd level teams and repositories have a one-to-one correspondence
and share the same name.
The users responsible for a repository are maintainers of the corresponding 3rd level teams.
This role grants them the authority to add and remove other members of the Organization to/from the teams.
In this way, they can control the group of collaborators who can actively contribute
to the development of the code within the repository, provided that these collaborators are members of the Organization.

.. figure:: CN-HPC_GitHub_organization_structure.png
   :width: 604
   :height: 306
   :alt: map to buried treasure

   ICSC CN HPC Spoke 4 GitHub organization structure.

------------------------
Authentication to GitHub
------------------------

What was previously mentioned applies to the content visible on GitHub.
In daily use, developers typically work on code saved on their local machines
and then push the changes they make to their code on GitHub.
To perform this operation, assumed to be done via the command line,
it is necessary to use one of the authentication methods offered by GitHub.

Authentication is the process of supplying or confirming credentials unique for each user,
proving that a user is indeed who they claim to be.
On GitHub, this process can occur in various ways.
An extensive guide on authentication on GitHub can be found on the webpage
`About authentication to GitHub <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/about-authentication-to-github>`.


^^^^^^^^^^^^^^^^^^^^^^
Personal Access Tokens
^^^^^^^^^^^^^^^^^^^^^^
For simplicity, it is recommended to access the GitHub Organization's
repositories from the command line using HTTPS.
To this end users must use personal access tokens (PATs) in place of passwords.
Whenever Git prompts for a password, the PAT must be entered instead.
A comprehensive guide on this topic is available in the GitHub documentation
(`Managing your personal access tokens <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens>`). 
However, a concise guide is provided below,
to assist users who require write access to repositories within the Organization.

Two types of PATs exist:

* Fine-grained PATs
* PATs (classic)

In the ICSC CN HPC Spoke 4 Organization, PATs (classic) have been restricted.
Therefore, only the use of fine-grained PATs is allowed.
To create a fine-grained PAT, users must follow these steps:

#.  `Verify their email address<https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/verifying-your-email-address>`
    (if it has not been verified yet).
#.	On any page, click their profile photo (upper-right corner) > Settings.
#.	On the left sidebar click Developer settings > dropdown menu “Personal access tokens” >
    Fine-grained tokens > Generate new token (top-right button).
#.	Set the token name, expiration, resource owner,
    repository access and permissions according to the table below:
+---------------------+----------------------------------------------------+
| Token name          |	<repo-name>_<username>                             |
| Expiration	      | Any option                                         |
| Resource owner      |	ICSC-CN-HPC-Spoke-4-Earth-Climate                  | 
| Justification	      | Enter a justification for the request              |
| Repository access   |	Only select repositories                           |
| Select repositories |	Name of the (single) repository to access          |
| Permissions	      | Repository permissions > Contents > Read and write |
+---------------------+----------------------------------------------------+
