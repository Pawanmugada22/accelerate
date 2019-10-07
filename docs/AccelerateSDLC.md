Accelerate (SDLC Management Tool)
========================

Objectives :

1) Software should have unique login credentials and dashboard for all the resources present in a team
2) Software should have provision to create and maintain separate multiple projects and teams.
3) Software should have three level hierarchy were like as follows,

		--SuperUser level login to control team creation and resource creation.
		--Manager level login to control the resources in a team, manage projects and assign task or milestones with target to the resources.
		--Resource level login to complete tasks or milestones, provide daily summary of progress and auto carry-over of tasks which are pending to next day.

Functional Architecture :

1) SuperUser

	-- SuperUser should create and manage teams and resources.
	
2) Manager

	-- Manager should create projects,milestones and tasks.
	-- Manager should be able to see dashboard of each and every resource in a team.
	
3) Resources

	-- Resources should complete their tasks and provide daily summary to the manager.
	-- If tasks comtains any dependency with other resource in a team, it can be moved that resource.
	-- If the resource face any challenge or require help to complete the task resource can raise request to the manager.

