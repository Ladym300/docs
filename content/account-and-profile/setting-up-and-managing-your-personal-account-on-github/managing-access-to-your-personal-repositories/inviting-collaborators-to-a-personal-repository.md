---
title: Inviting collaborators to a personal repository
intro: 'You can {% ifversion fpt or ghec %}invite users to become{% else %}add users as{% endif %} collaborators to your personal repository.'
redirect_from:
  - /articles/how-do-i-add-a-collaborator
  - /articles/adding-collaborators-to-a-personal-repository
  - /articles/inviting-collaborators-to-a-personal-repository
  - /github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository
  - /github/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository
  - /account-and-profile/setting-up-and-managing-your-github-user-account/managing-access-to-your-personal-repositories/inviting-collaborators-to-a-personal-repository
product: '{% data reusables.gated-features.user-repo-collaborators %}'
versions:
  fpt: '*'
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Accounts
  - Repositories
shortTitle: Invite collaborators
---
## About collaboration in a personal repository

To collaborate with users in a repository that belongs to your personal account on {% data variables.location.product_location %}, you can invite the users as collaborators.

If you want to grant more granular access to the repository, you can create a repository within an organization. For more information, see "[AUTOTITLE](/get-started/learning-about-github/access-permissions-on-github)."

{% ifversion ghec %}

If you're a member of an {% data variables.enterprise.prodname_emu_enterprise %}, you can only invite other members of your enterprise to collaborate with you. {% data reusables.enterprise-accounts.emu-more-info-account %}

{% endif %}

{% data reusables.repositories.private_forks_inherit_permissions %}

## Inviting a collaborator to a personal repository

You can send an invitation to collaborate in your repository directly to someone on {% data variables.location.product_location %}{% ifversion fpt or ghec %}, or to the person's email address{% elsif ghes or ghae %}.{% endif %}

{% ifversion fpt or ghec %}

{% data variables.product.company_short %} limits the number of people who can be invited to a repository within a 24-hour period. If you exceed this limit, either wait 24 hours or create an organization to collaborate with more people. For more information, see "[AUTOTITLE](/organizations/collaborating-with-groups-in-organizations/creating-a-new-organization-from-scratch)."

{% endif %}

1. Ask for the username of the person you're inviting as a collaborator.{% ifversion fpt or ghec %} If they don't have a username yet, they can sign up for {% data variables.product.prodname_dotcom %}. For more information, see "[AUTOTITLE](/get-started/signing-up-for-github/signing-up-for-a-new-github-account)".{% endif %}
{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
{% ifversion fpt or ghec or ghes > 3.4 or ghae > 3.4%}
1. In the "Access" section of the sidebar, click **{% octicon "people" aria-hidden="true" %} Collaborators**.
1. Click **Add people**.
2. In the search field, start typing the name of person you want to invite, then click a name in the list of matches.
3. Click **Add NAME to REPOSITORY**.
    ![Button to add collaborator](/assets/images/help/repository/add-collaborator-user-repo.png)
{% else %}
5. In the left sidebar, click **Collaborators**.
![Repository settings sidebar with Collaborators highlighted](/assets/images/help/repository/user-account-repo-settings-collaborators.png)
6. Under "Collaborators", start typing the collaborator's username.
7. Select the collaborator's username from the drop-down menu.
   ![Collaborator list drop-down menu](/assets/images/help/repository/repo-settings-collab-autofill.png)
8. Click **Add collaborator**.
   !["Add collaborator" button](/assets/images/help/repository/repo-settings-collab-add.png)
{% endif %}
{% ifversion fpt or ghec %}
9. The user will receive an email inviting them to the repository. Once they accept your invitation, they will have collaborator access to your repository.
{% endif %}

## Further reading

- "[AUTOTITLE](/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-personal-account-settings/permission-levels-for-a-personal-account-repository#collaborator-access-for-a-repository-owned-by-a-personal-account)"
- "[AUTOTITLE](/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/removing-a-collaborator-from-a-personal-repository)"
- "[AUTOTITLE](/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-access-to-your-personal-repositories/removing-yourself-from-a-collaborators-repository)"
- "[AUTOTITLE](/organizations/organizing-members-into-teams)"
