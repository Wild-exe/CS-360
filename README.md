# CS-360
Q: Briefly summarize the requirements and goals of the app you developed. What user needs was this app designed to address?\
A: This project aims to provide users with a mobile application to monitor, create, edit, and get event reminders. The requirements were essentially to develop an Android application that performed CRUD operations on an SQLite database for handling the events. The needs met include:
  Intuitive UI/UX.
  A login process for security. 
  Reminders via the required SMS Notifications.
The application is helpful for anyone interested in productivity and scheduling.\

Q: What screens and features were necessary to support user needs and produce a user-centered UI for the app? How did your UI designs keep users in mind? Why were your designs successful?\
A: Aside from a basic login and register screen, the application provides a list with expandable cards for editing and deleting. The other screen implemented is for adding an event to the list. For features, all CRUD operations are facilitated through buttons. A date and time dialog was implemented to provide a user-centric approach, while other needed features can be found through a menu in the action bar. The main benefits of this design come from to fundamentals that I am a big proponent of, minimal user inputs per feature and an optimal layout for interaction. By keeping core functionality condensed to a bottom navbar, primary user loops are kept accessible. The ability to edit and delete events if the event is expanded allows for quick editing without obfuscation. A Material Design palette was also used for highlighting core functionality. Overall, I consider the application's design successful due to the aforementioned, given the constraints.\

Q: How did you approach the process of coding your app? What techniques or strategies did you use? How could those be applied in the future?\
A: The coding was done using Agile methodology. Priority was given to the requirements necessaru to bring the application to a functional point. After, other features with less priority were added. I generally break down needs and requirements into user stories. I then work on creating story points or sub-user stories as needed. During coding, I generally examine the desired output, possible inputs, and implement solutions from that point. I plan to implement this strategy until another becomes more efficient.\

Q: How did you test to ensure your code was functional? Why is this process important and what did it reveal?\
A: For testing, I took on the role of a user. I felt too constrained by time; otherwise, I would have performed unit and integration tests. Testing is necessary for development to prevent errors and exceptions as resolving either become more costly the longer they reside in the code. One issue revealed was that the AlertManager sends alerts instantly instead of when the reminder time aligns with the current time. Before launch, this will need to be addressed when I update the API to the latest release.\

Q: Considering the full app design and development process, from initial planning to finalization, where did you have to innovate to overcome a challenge?\
A: I decided fairly early that I would not be satisfied with the UI unless it incorporated an expandable recycler view and calendar view for the events. Since both are views of the same data using a fragment was a better solution than separate activities. The recyclerview adapter become complicated due to this as did the alertmanager. To overcome this challenge a simpleton class was implemented containing the MainActivity's context, which should not cause memory leak. The code also had to be modified as the documentation does not provide clarity on handling certain classes, objects, or methods outside of an activity.\

Q: In what specific component from your mobile app were you particularly successful in demonstrating your knowledge, skills, and experience?\
A: I think the recyclerview illustrates both excellent design and code. Creating an expandable event card was facilitated by a hierarchy of different layouts and views necessary for functionality and using the hidden attribute for determining the event card's state.
