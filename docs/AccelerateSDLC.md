Accelerate (SDLC Management Tool)
=============================

###Objectives###

1) Software should have unique login credentials and dashboard for all the resources present in a team
2) Software should have provision to create and maintain separate multiple projects and teams.
3) Software should have provision to maintain multi-level hierarchy for managers.
4) Software should hava a project creation and maintainance features.
5) Software should have three level users like below,

		--SuperUser level login to control team creation and resource creation.
		--Manager level login to control the resources in a team, manage projects and assign task or milestones with target to the resources.
		--Resource level login to complete tasks or milestones, provide daily summary of progress and auto carry-over of tasks which are pending to next day.

####Functional Architecture :####

1) **SuperUser**

	-- SuperUsers should create and manage teams and resources.
	-- They are the people who maintain organisations infrastructure.
	-- SuperUsers can maintain tasks that are visible to only them.
	
2) **Manager**

	-- Managers should create projects,milestones,tasks and issues(or)feedback.
	-- These tasks should be assigned to the resources allocated to them.
	-- Managers can be able to see dashboard of each and every resource in a team.
	-- Managers will have three dashboards resources dashboard, projects dashoard and manager dashboard.
	-- Higher level managers will have teams dashboard, managers dashboard.
	-- Manager can also maintain tasks that are not visible to higher level managers
	
3) **Resource**

	-- Resources should complete their tasks and provide summary to the manager.
	-- If tasks comtains any dependency with other resource in a team, it can be moved that resource.
	-- If the resource face any challenge or require help to complete the task resource can raise request to the manager so that a task can be completed by collaboration.
	-- Resource can also maintain tasks that are not visible to managers.
	
####Lifecycle####

**States of different entities in SDLC** 

######Employee states :######

1) A - Employee is active.
2) I - Employee is relieved.
3) U - Employee is in long leave

######Team states :######

1) A - Team is active.
2) D - All the resources in the team are desolved.Team is suspended or inactive for a duration of time.
3) I - Removed the team or merged with other team.

######Project states :######

1) A - Project is active, resources are contributing regularly for project completion.
2) H - Project is on hold, due to un-availability of resource or due to dependency or    because of other high priority projects.
3) S - Project is rejected or suspended because of better solution or client abandonned the requirement.
4) C - Project is completed, all the milestones in the project is completed. 

######Milestone states :######

1) P - Milestone is pending, all dependencies are met and ready to start.
2) I - Milestone is in-progress, resources are already working in the tasks present in the milestone.
3) D - Milestone is dependent on the other milestone, unable to start immediately.
4) B - Milestone is blocked because clarity is required from the client or bussiness model is not finalised.
5) C - Milestone is completed owing that all the issues that arised while completing the tasks in the milestone is resolved.

######Task states :######

1) P - Task is pending, resource is busy with other tasks.
2) B - Task is blocked, resource requires more clarity about the task from stakeholders.
3) I - Task is in-progress, resource is working in completing the task.
4) D - Task is dependant on other task or the resource require help from another resource.
5) W - Task is waiting for sign-off, resource has completed the task it either being reviewed or yet to be reviewed for sign-off.
6) C - Task is completed, resource has completed the task.

######Issue states :######

1) O - Issue is raised, resource has raised the issue and problem is clearly understood by the resource.
2) F - Issue needs more clarity, resource has moved the issue to the person who raised the issue for more clarity.
3) R - Issue is resolved, solution given by the resource should be reviewed and signed off by manager or another resource.
4) T - Fix is given to the stakeholders yet not completely resolved once and for all.
5) P - Issue is re-opened, solution given by the resource is in-adequete or not correct, asking the resource to come up with another solution
6) C - Solution to the issue is reviewed and signed-off or ready for production.



