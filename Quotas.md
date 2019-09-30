Quotas can be assigned to orgs or spaces. Quotas at the org level affect all new spaces and can be overridden by setting space quotas.   

    $ cf set-quota ORG ORG_QUOTA

    $ cf set-space-quota SPACE_NAME SPACE_QUOTA_NAME

Orgs support manager, billing and auditing roles. You associate the role and the user account with the org:

    $ cf set-org-role USERNAME ORG ROLE

Spaces support manager, developer, and auditing roles. You associate the role and a user account with the space:

    $ cf set-space-role USERNAME ORG SPACE ROLE
