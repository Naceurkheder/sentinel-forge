*Sentinel Forge as an internal platform used by a security/operations team*

#The backend handles:
	authentication
	authorization
	incidents
	services
	detections
	files
	audit logs
	real-time updates
	background processing
	telemetry

#And the infrastructure underneath handles:
	PostgreSQL
	Redis
	object storage
	WebSockets
	etc. 

#What we are actually building?
We are building a security/operations website where a team can manage and investigate problems.

The website will have things like:
	Incidents → problems/security events that happened
	Services → systems/apps being monitored
	Detections → suspicious things the system found
	Files → evidence and reports
	Operations → actions/tasks being performed
	Audit log → who did what and when
	What will you actually do?

You'll build it step by step:
	+ Make the website
		Dashboard
		Incident pages
		Service pages
		Detection pages
		File/report pages
	+ Make login work
		Users can log in.
		Users have different permissions.
		Example: an admin can do more than a normal analyst.
	+ Make sure users only see their own company's data
		Company A must not see Company B's incidents.
		You'll actually write tests to prove this.
	+ Build the database
		Store users
		incidents
		services
		detections
		files
		activity history
	+ Make the application faster
		Use Redis for things that need to be accessed quickly.
		Add database indexes.
		Add limits so someone can't spam your API with thousands of requests.
	+ Make some tasks happen in the background



=> it's a real security management dashboard where users can investigate incidents, manage data and files, and perform operations 
while making sure it's secure, fast, multi-user, real-time, and properly monitored.



