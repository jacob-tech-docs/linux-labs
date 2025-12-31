README - linux-user-permission-lab

Goal of the Lab: Assign Users to Groups. Configure limited visudo. Test Access.

Steps:
    Create Groups: developers, auditors
    Create Users: alice, bob, charlie
    Assign groups to users
    Create Project Directory and assign the setgid bit
    Configure Limited Sudo: Allow users in the developers group to view services

Why Permissions and Groups matter

Skills Demonstrated:

Additional Notes:
Observed Behavior:
    Files created in a setgid dir inherit the gorup but not the group write permissions due to user umnask.
Resolution:
    Implemented default ACLS to ensure consistent group collaboration while preserving system security.
