# Desktop-Notifier



This Python script utilizes the Tkinter library to craft an interactive graphical user interface (GUI) for a notification application. The code elegantly integrates various libraries, including tkinter, tkinter.ttk, plyer, datetime, and pywhatkit.

The core functionality lies within the create_notification function. This function takes in parameters such as the task description and time, precisely specified in hours, minutes, and seconds. By converting this time to seconds, the function effectively suspends execution using time.sleep and subsequently triggers a desktop notification using the plyer.notification module. Notably, the pywhatkit library is harnessed to dispatch a WhatsApp message containing the task particulars.

The submit_tasks function serves as the connector. Extracting data from input fields in the GUI—namely task description, hours, minutes, and seconds—it seamlessly invokes the create_notification function for each distinct task.

Initiating the Tkinter GUI window, dubbed "Notification Application," grants it dimensions of 500x400 pixels. Notably, the window is thoughtfully centered at the screen's uppermost region.

A textual cue is thoughtfully inserted within the GUI window, prompting users to input their tasks alongside the corresponding timing.

To facilitate multiple tasks, an iterative loop meticulously generates five pairs of input fields. Each pair consists of a task label, a task description entry field, as well as labels and combo boxes for selecting hours, minutes, and seconds.

The task_entries list proficiently collects all the input fields for each task, streamlining management.

To finalize the user experience, a submission button is thoughtfully positioned within the GUI window. Upon being activated, this button triggers the submit_tasks function, ensuring a coherent flow of task submission and notification scheduling.

To kickstart the GUI event loop and display the window, the mainloop method is judiciously invoked on the Tkinter root object.

Note: It's imperative to replace "+91YourNumber" in the pwt.sendwhatmsg function call with your personal phone number to facilitate the receipt of WhatsApp notifications.

