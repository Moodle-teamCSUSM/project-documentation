# Project Plan

## How we make it all work

  Date Created   |  Last Modified
:--------------: | :--------------:
January 16, 2016 | January 16, 2017

--------------------------------------------------------------------------------

### Document Objective

To describe what software systems we use, how we determine our deadlines, referencing the use of the [Communications Document](communications.md), and managing how we handle disparities between teams.

### Kickstart

Now that we have the team all set, we must first work on the design phase. **How do we want our system to work on each platform?** To design the application for iOS, Android and Web, we need to use a simple, and accessible application for each member of the team.

After we decide the design, the System Administrators need to setup the system so that each team has a sandbox environment, database access, repo integration, and any other service needed to allow our system to progress smoothly (This includes installing Moodle onto our system and initializing the process).

The Moodle System will allow us to determine what additional data tables we need for our database and what we need to create. The database team will start deciding which data is critical to production and what is optional. They will also keep documentation on each database, schema and attribute that we use.

Once the database is properly normalized, and analytics tables have been created in a separate database, all teams can move to their smaller groups. Each group will have a design they need to follow in addition to setting up their own testing environment. Each user can choose their ideal IDE, as long as it works with the team.

Note that all deadlines are subject to change. In addition to the repo, each team should maintain a single change-log that documents their work. This document does not need to be sorted by user, but allows other teams to compare progress. Please use standardized decimal version control for all versions.

### Implementation

#### Design

As mentioned prior, we need a consistent design software that allows us to achieve a vast majority of tasks that we will include in the live version. This includes any animations, any page changes and any data alteration.

For this project, we are going to use Microsoft PowerPoint. Due to its ability to be universal, this will allow for proper version control across teams with easy management. This program allows for animations between slides as well as 'jumping' to different pages in the document using bookmarks and reference points.

Each team will maintain their own PowerPoint document and store on its relative repository. The design must be consistent. Before we even create the document, the Design Team must all agree on a color scheme (use the Poll channel if needed). To reduce work, each team must only create a max of 2 pages at a time. This max may change if productivity is better than expected.

A preference may be to use [Google's Material Design](https://design.google.com) or [Apple's Design Specifications](https://developer.apple.com/design/) as a starting point.

#### System Administrators

While/After the design is being created, the Backend Administrators must get the system setup for each team member. This includes setting up any version control, remote hosting, package management, database initialization, etc. that may be needed.

In addition to the setup, the backend team must create any documentation required to assist other team members get started. They are not required to remote-into any persons personal machine. The documentation must be enough that doing so is not needed.

There may be documents already created for some items. System Administrators should make any recommended documents accessible on the project-documentation repository in a separate folder.

#### Database

We have a few options for database:

- MySQL
- MongoDB
- Any Other (Those are already installed)

Depending on the System Administrators, and what may seem as a best fit for the needed requirements, we may even use multiple.

The database ERD must be completed in [Omnigraffle 6]('') (Sorry, no code available for 7 yet) so the relationships and entities could easily be moved and altered.

Each team will have an account (user) for the database. There will be individual accounts as needed.

To update the database table-set, there must be an issue reported in GitHub. The issue must state what you wish to change and why. This may include any additional tables, rows, columns, relationships, etc that may prohibit pre-existing statements from working. You must also post in the #database channel of slack adhering to the change.

There will be at least 2 databases - one for strict application information while the other is for analytics and log information. All pages must have appropriate log information for administrative troubleshooting.

#### Project Creation

After the application is completely setup, meaning we have completed:

- Project Documentation
- Administrative Management (Super Admins)
- Wireframes
- Database Implementation

We can move onto the application we set out to create (Moodle Theme)

##### All Encompassing

###### User Rights

Within the actual project, there must be user rights. Our respective stakeholders include:

- Super Admins
- Instructor/Staff Administrators
- Students
- Guests

Each branch of the project must consider each of the user's views when both designing and implementing the theme. Be sure to create relative test cases as well.

###### Project Documentation

Due to the differences that my appear in each project, each critical team (collaborative efforts of Android, iOS and Web Teams) each must create their own SRS (Systems Requirements Specifications) that include information such as:

- Use cases
- Stakeholders
- Known Bugs
- Instruction Manual (including breakdowns per user)

In addition, each team must also prepare a master change-log that keeps other teams within the project updated on your current status. This is a single documentation appended in the beginning such that the newest changes appear first. This should be general knowledge similar to what you see in a public application/Operating System change-log. This should be updated for every project change, published to the master "project-documentation" channel on Slack and branch on GitHub.

Lastly, each team should use [Asana](https://app.asana.com/0/dashboard/248713323873832) (setup information will appear in the [Communications document](communications.md)) to manage their task lists. Each team should break down each task within their critical team and both assign and schedule each task. This list will be used to determine what is remaining in the project (for all teams, including yours).

#### Project Implementation

It does not matter which IDE you use - as long as it works with your small groups. Be sure to push to your repo regularly so other team members stay updated on your status. You should push to your branch every time you either take a break from coding, or walk away from your desk after working on it. Update to master at least once a week (more if needed - it is recommended).

##### Web Development Team

Since your project relies on web-based hosting, you will have access to a remote folder on our system. You should be receiving user-level access writing access as soon as the system is setup.

#### Final Notes

Remember, we are not on a set schedule, but we have to have some guidelines if anything should get done. For best results, we should treat this as a semester project. Below is a breakdown of dates that should get us started.

#### Timeline

All dates are subject to change. Keep checking these dates for additional notes or possible changes. Any date changes will also be noted in the #general channel on Slack.

Action                          | Date to Submit        | Team
------------------------------- | --------------------- | ---------------------
Project Documentation (PM Only) | January 23, 2017      | Project Lead
System Setup and Initialization | January 30, 2017      | System Administrators
Design Wireframes               | February 27, 2017     | All Critical Teams
SRS and Task List               | February 27, 2017     | All Critical Teams
**Removing inactive members**   | **February 27, 2017** | Project Lead
Database Initialization         | March 14, 2017        | System Administrators
Database Implementation         | March 27, 2017        | All Critical Teams
All Code w/ Documentation       | May 2, 2017           | All Critical Teams
Updated SRS w/ User Manual      | May 8, 2017           | All Critical Teams
Virtual Presentation w/ Group   | May 12, 2017          | All Critical Teams
