Accelerate (SDLC Management Tool)
========================

**Objectives**

1) Software should have unique login credentials and dashboard for all the resources present in a team
2) Software should have provision to create and maintain separate multiple projects and teams.
3) Software should have provision to maintain multi-level hierarchy for managers.
4) Software should hava a project creation and maintainance features.
5) Software should have three level users like below,

		--SuperUser level login to control team creation and resource creation.
		--Manager level login to control the resources in a team, manage projects and assign task or milestones with target to the resources.
		--Resource level login to complete tasks or milestones, provide daily summary of progress and auto carry-over of tasks which are pending to next day.

Functional Architecture :

1) SuperUser

	-- SuperUsers should create and manage teams and resources.
	-- They are the people who maintain organisations infrastructure.
	-- SuperUsers can maintain tasks that are visible to only them.
	
2) Manager

	-- Managers should create projects,milestones,tasks and issues(or)feedback.
	-- These tasks should be assigned to the resources allocated to them.
	-- Managers can be able to see dashboard of each and every resource in a team.
	-- Managers will have three dashboards resources dashboard, projects dashoard and manager dashboard.
	-- Higher level managers will have teams dashboard, managers dashboard.
	-- Manager can also maintain tasks that are not visible to higher level managers
	
3) Resource

	-- Resources should complete their tasks and provide summary to the manager.
	-- If tasks comtains any dependency with other resource in a team, it can be moved that resource.
	-- If the resource face any challenge or require help to complete the task resource can raise request to the manager so that a task can be completed by collaboration.
	-- Resource can also maintain tasks that are not visible to managers.
	

