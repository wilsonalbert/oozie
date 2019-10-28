## The next is the list of common commands to use with Yarn / Oozie


### Yarn get the status with application id

`yarn application -status [application_id]`

### Get a list of running applications

`yarn application -list -appStates RUNNING`
 
### Get info for a task

`oozie job -info [task_id] -len 100000`

### get yarn log fom oozie job

1. Get job id. e.g: `job_1570721854320_107114`
2. change the name replacing job_ for application_: Result: `application_1570721854320_107114`
3. Get yarn log using: 

`yarn logs -applicationId application_1570721854320_107114`

### get jobs from from a user

`oozie jobs –filter user=[user_id]`


