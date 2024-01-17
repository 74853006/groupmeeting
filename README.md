# Meeting Scheduler
## Introduction:
Meeting Scheduler is a meeting scheduling system based on Spring Boot, designed to help tutors and students organize and participate in academic group meetings more conveniently.

## Compiler Environment: 
>jdk 21.0.1
>
>mysql 5.7.24

## Frame:
>springboot2.0 
>
>mybatis

## jar package management tool:
> Maven

## translater :
>IDEA

## Complete schedule:
	> Build the framework

## System functions :
### Tutor module
> Login: The tutor logs in to the system through an account.
> 
> Personal information management: View and modify personal information.
> 
> View student information: View students’ basic information and statistics on participation in group meetings.
> 
> Publish group meeting requirements: Publish the group meeting requirements, including the desired topics for the group meeting, etc.
> 
> View group meeting recommendations: system-generated recommendations for students and possible meeting times.
> 
> The modification group will recommend: Make manual modifications based on the recommended list.
> 
> Confirm group meeting arrangements: Confirm the final group meeting arrangements, and the system will send notifications to relevant students.
> 
> Process student applications: Allow or deny group conference applications from uninvited students.

### student module
> Login: Students log into the system through their accounts.
> 
> Personal information management: View and modify personal information.
> 
> View instructor information: View the instructor's basic information and related group meeting information.
> 
> Students apply: Non-invited students can apply to participate in the group meeting.
> 
> View group meeting invitations: View received group meeting invitations.
> 
> Respond to a group meeting invitation: Accept or reject the group meeting invitation.
> 
> View group meeting history: View the history of group meetings you have participated in.

### Automatic scheduling module
> Intelligent recommendation of participating students: Analyze the group meeting needs released by the instructor and recommend qualified students.
> 
> Recommended group meeting time: Intelligent scheduling of group meeting time based on the time range specified by the instructor.
> 
> Generate recommendation list: The system generates recommended students and possible meeting times based on the matching results.

### Administrator module
> System notification: The system sends notifications such as meeting invitations and confirmation information via email or SMS.
> 
> Calendar Integration: Integrate group meeting schedules into instructor and student calendars.
> 
> System configuration management: configure basic information of the system, such as semester start and end times, system notification methods, etc.
> 
> User management: View and manage the account information of all tutors and students.
> 
> System log: View the system operation log to monitor system operation.
> 
> Data statistics and analysis: View the activities of tutors and students through the statistical functions provided by the system.

## Project structure
```
meeting-scheduler
|-- src
|   |-- main
|       |-- java
|           |-- com
|               |-- example
|                   |-- meetingscheduler
|                       |-- MeetingSchedulerApplication.java
|                       |-- config
|                           |-- WebSecurityConfig.java
|                       |-- controller
|                           |-- TutorController.java
|                           |-- StudentController.java
|                           |-- AdminController.java
|                       |-- model
|                           |-- Tutor.java
|                           |-- Student.java
|                           |-- Meeting.java
|                           |-- Schedule.java
|                       |-- repository
|                           |-- TutorRepository.java
|                           |-- StudentRepository.java
|                           |-- MeetingRepository.java
|                           |-- ScheduleRepository.java
|                       |-- service
|                           |-- TutorService.java
|                           |-- StudentService.java
|                           |-- AdminService.java
|                           |-- MeetingService.java
|                           |-- ScheduleService.java
|                       |-- scheduler
|                           |-- AutoSchedulingService.java
|                       |-- exception
|                           |-- MeetingNotFoundException.java
|                           |-- UserNotFoundException.java
|-- resources
|   |-- application.properties
|   |-- templates
|-- test
|   |-- java
|       |-- com
|           |-- example
|               |-- meetingscheduler
|                   |-- controller
|                       |-- TutorControllerTest.java
|                   |-- service
|                       |-- TutorServiceTest.java
|                   |-- scheduler
|                       |-- AutoSchedulingServiceTest.java
|-- pom.xml
```
##How to run
> Run MeetingSchedulerApplication.java to start the application.
>
> Visit http://localhost:8080 to access the application.










