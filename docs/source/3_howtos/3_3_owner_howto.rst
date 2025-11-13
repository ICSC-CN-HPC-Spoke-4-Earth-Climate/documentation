============================
Organization Administrators
============================

This guide summarizes the most common 
administrative workflows for the ICSC CN HPC 
Spoke 4 GitHub Organization.

Adding a User to the GitHub Organization
----------------------------------------

This section explains how an administrator 
can add a new user to the GitHub Organization 
once the necessary agreements and requests have been made.

1. **Prepare the request**

   - Ensure that agreements have been made with the relevant WP Leader.  
   - Complete the user request table (see :ref:`Memberships & Teams Management`).

2. **Invite the user**

   - Go to the **People** tab of the organization. 
   - Click on the **Invite member** button.

   .. figure:: images/3_3_invite_member.png
      :width: 600
      :height: 60
      :align: center 
      :alt: Add to teams.

   - Search for the user by their GitHub username.
   - Click **Invite.**

3. **Set membership type**

   - Select **Member** (do not select Owner!).

   .. figure:: images/3_3_select_role.png
      :width: 400
      :height: 200
      :align: center 
      :alt: Select role.


4. **Assign teams**

   - Add the invited user to the relevant WP/Innovation Grant team.  
   - If applicable, also add them to the second-level team, 
     according to the structure previously agreed with the WP Leader.

   .. figure:: images/3_3_add_to_teams.png
      :width: 400
      :height: 600
      :align: center 
      :alt: Add to teams.

5. **Send the invitation** 

   - Click **Send Invitation**.  
   - The invited user will receive an email and 
     has **7 days** to accept and join the organization.

Further details on this process can be 
found in the official GitHub documentation: 
:ref:`Memberships & Teams Management``
`Inviting users to join your organization <https://docs.github.com/en/organizations/managing-membership-in-your-organization/inviting-users-to-join-your-organization>`_.


Creating a New Repository
-------------------------

Before starting, the user requesting the repository 
must follow the guide on requesting a new repository:  
:ref:`Request the creation of a new repository`.

Once the request has been submitted, 
a new issue will appear in the **administration** 
repository of the GitHub Organization.  

Steps for Administrators
~~~~~~~~~~~~~~~~~~~~~~~~~

1. **Review the issue**

   - Go to the **administration** repository > **Issues**.  
   - Select the newly created issue.  
   - Ensure the issue complies with the prescribed format.  
   - If not, comment on the issue requesting the user to fix it.


2. **Create the repository**  

   - Go to the main page of the organization > **Repositories**.  
   - Click **New repository**.

   .. figure:: images/3_3_new_repo.png
      :width: 500
      :height: 540
      :align: center 
      :alt: New repository.

   - Fill in the **Repository name** as requested by the user.
   - Add the **Description** if provided (the "purpose" field from the issue).   
   - Set the **visibility** (private/public) according to the requirement.  
   - Click **Create repository**.


3. **Create the associated team**

   - Go to the main page of the organization > **Teams**.
   - Click **New team**.

   .. figure:: images/3_3_create_new_team.png
      :width: 450
      :height: 575
      :align: center 
      :alt: New team.

   - Give the team the **same name as the repository**.  
   - Select a **parent team**. 
     Typically, the parent team should be a second-level team. 
     For Innovation Grant repositories, 
     select the corresponding Innovation Grant team as the parent.
   - Once created, navigate to the **parent team** page: 
     Organization main page > Teams > <WP team name> > <2nd level team name>.  
   - Verify that the newly created team is listed under the correct parent team.


4. **Add members to the team**

   - Open the newly created team page > Members > **Add a member**.
   - Add the people listed in the issue.

   .. warning::
      All people should already be members of the organization.


5. **Set the repository manager (maintainer)**

   - Select the person indicated in the issue as the **repository manager**.  
   - A button will appear saying "**1 member selected**". Click it.  
   - From the dropdown menu, select **Change role**.  
   - Set this person’s role to **Maintainer**.


6. **Connect teams to the repository and set permissions**

   - Go to the repository page and select **Settings**.  
   - Under **Collaborators and teams**, in the **Manage access** section, click **Add teams**. 

   .. figure:: images/3_3_collaborators_teams.png
      :width: 600
      :height: 270
      :align: center 
      :alt: Add collaborators and teams.

   - Add two teams:

     1. The newly created team (give **Write permissions**).  
     2. The relevant 2nd level team (give **Read permissions**).  
   
     To modify the permissions for a team, 
     click the corresponding **Role** button and 
     choose the appropriate option from the dropdown menu.


This completes the workflow for creating a new repository 
and assigning the relevant permissions.

