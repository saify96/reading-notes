# Tasks and Back Stack
- A task is a collection of activities that users interact with when performing a certain job.
- The activities are arranged in a stack—the back stack.

## To summarize the default behavior for activities and tasks:
- When Activity A starts Activity B, Activity A is stopped, but the system retains its state (such as scroll position and text entered into forms). If the user presses the Back button while in Activity B, Activity A resumes with its state restored.
- When the user leaves a task by pressing the Home button, the current activity is stopped and its task goes into the background. The system retains the state of every activity in the task. If the user later resumes the task by selecting the launcher icon that began the task, the task comes to the foreground and resumes the activity at the top of the stack.
- If the user presses the Back button, the current activity is popped from the stack and destroyed. The previous activity in the stack is resumed. When an activity is destroyed, the system does not retain the activity's state.
- Activities can be instantiated multiple times, even from other tasks.


## Defining launch modes
- Launch modes allow you to define how a new instance of an activity is associated with the current task. You can define different launch modes in two ways:

- Using the manifest file
  - When you declare an activity in your manifest file, you can specify how the activity should associate with tasks when it starts.

- Using Intent flags
  - When you call startActivity(), you can include a flag in the Intent that declares how (or whether) the new activity should associate with the current task.

## Using the manifest file
- When declaring an activity in your manifest file, you can specify how the activity should associate with a task using the <activity> element's launchMode attribute.

