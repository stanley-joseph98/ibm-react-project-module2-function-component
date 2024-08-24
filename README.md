# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh


Setting up the environment
From the menu on top of the lab, click on the Terminal tab at the top-right of the window shown at number 1 in the given screenshot, and then click New Terminal as shown at number 2.



Write the following command in the terminal to clone the boiler template for this React application and hit Enter.

1
git clone https://github.com/ibm-developer-skills-network/event_planner.git
Copied!
The above command will create a folder named as event_planner under Project folder and the structure will be as shown in the given screenshot.


Write the command to enter the event_planner folder in the terminal. Use the below command to navigate to the event_planner folder in the terminal.

1
cd event_planner
Copied!
To make sure that the code you have cloned is working correctly, you need to follow the given steps:

Write the following command in the terminal and hit Enter to install all the necessary packages to execute the application:

1
npm install
Copied!
Then execute the following command to run the application and this will provide you with port number 4173:

1
npm run preview
Copied!
To view your React application, click the Skills Network icon on the left panel (refer to number 1). This action will open the SKILLS NETWORK TOOLBOX. Next, click Launch Application (refer to number 2). Enter port number 4173 in Application Port (refer to number 3) and click .



The output will display as shown in the given screenshot.


You can preserve your latest work on this lab by adding, committing, and pushing it to your GitHub repository. This ensures that even if you're not working on the task continuously, your progress will be saved, allowing you to resume from where you left off.

Note: Step 8 is optional.


Create Basic Template
Navigate to the Components folder located within the src folder of your React project. The event_planner application folder includes the class component named as EventPlanner.jsx and a css file named as EventPlanner.css.

Navigate to the EventPlanner.jsx component located within the src folder of your React project. In the return of this component you have a parent <div> with class name event-planner-container which includes child <header> tag with <h1> tag.

You need to create five <section> tags after the <header> tag.

First section tag with class name description
Second section tag with class name events_categories
Third section tag with class name features
Fourth section tag with class name testimonials
Fifth section tag with class name contact

  <div className="event-planner-container">
            <header>
                <h1>Welcome to Event Planner</h1>
            </header>
            <section className="description">
            </section>
            <section className="events_categories">
            </section>
            <section className="features">
            </section>
            <section className="testimonials">
            </section>
            <section className="contact">
            </section>
        </div>


Define Description and Event Categories
Inside the section tag with class name description, add a <p> tag and a button tag. In the <p> tag, insert text related to the event planning theme. Assign the class name get-started-button to the button tag.

1
2
3
4
5
6
7
8
9
 <section className="description">
                <p>
                    Plan and organize your events effortlessly with Event Planner. From
                    birthdays to corporate meetings, we've got you covered.
                </p>
                <button className="get-started-button">Get Started</button>
            </section>
Copied!
Now you need to rerun the React application and see the output. The output should be as per the given screenshot.



Note: If the page is already open in the browser, you will need to refresh it

Next you need to create multiple events categories inside section tag with class name events_categories.For this create <ul> tag inside this section. Inside <ul> tag you should have a <h1> tag for event heading and multiple <li> tags for different categories of that particular event.

1
2
3
4
5
6
7
8
9
<ul>
 <h2>Social Events:</h2>
 <li>Birthday parties</li>
  <li>Anniversary celebrations</li>
  <li>Wedding receptions</li>
  <li>Baby showers</li>
  <li>Graduation parties</li>
  <li>Family reunions</li>
</ul>
Copied!
You can also include multiple <ul> tags for different event headings and sub categories just as above.

1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
            <section className="events_categories">
                <ul>
                    <h2>Social Events:</h2>
                    <li>Birthday parties</li>
                    <li>Anniversary celebrations</li>
                    <li>Wedding receptions</li>
                    <li>Baby showers</li>
                    <li>Graduation parties</li>
                    <li>Family reunions</li>
                </ul>
                <ul>
                    <h2> Entertainment Events:</h2>
                    <li>Concerts</li>
                    <li>Music festivals</li>
                    <li>Film screenings</li>
                    <li>Comedy shows</li>
                    <li>Art exhibitions</li>
                    <li>Cultural events</li>
                </ul>
                <ul>
                    <h2>Community Events:</h2>
                    <li>Fundraising events</li>
                    <li>Charity galas</li>
                    <li>Volunteer drives</li>
                    <li>Neighborhood block parties</li>
                    <li>Community festivals</li>
                    <li>Cultural celebrations</li>
                </ul>
            </section>
Copied!
Again re-run the application and check the output which will display as shown in the given screenshot.


Note: If the page is already open in the browser, you will need to refresh it

Create Features Section
Now you need to display the different features that this event planner organization is providing services for.

Inside section tag with class name features create a <h1> tag for heading and one <ul> tag with multiple <li> tags to demonstrate various features offered for event planning.

1
2
3
4
5
6
7
8
9
10
            <section className="features">
                <h2>Features</h2>
                <ul>
                    <li>Easy event creation and management</li>
                    <li>Customizable event templates</li>
                    <li>Guest list management</li>
                    <li>Real-time collaboration</li>
                    <li>Reminders and notifications</li>
                </ul>
            </section>
Copied!
The above code will display the output as the given screenshot after events categories.



To view the latest updates, you must rerun the application, and if the page is already open in the browser, you will need to refresh it.

Create Testimonials Section
To create the testimonials section given by multiple users, you need to create <h1> tag and <div> tag inside section tag with class name testimonials.

Then inside the <h2> tag you need to give the main heading of this section and inside the <div> tag you can write the review given by the user along with the username.

1
2
3
4
5
6
7
 <section className="testimonials">
    <h2>Testimonials</h2>
    <div className="testimonial">
       <p>"Event Planner made organizing my wedding a breeze. Highly recommended!"</p>
       <p className="author">- Emily Johnson</p>
      </div>
 </section>
Copied!
You can also create mutiple testimonials like above.
1
2
3
4
5
6
7
8
9
10
11
            <section className="testimonials">
                <h2>Testimonials</h2>
                <div className="testimonial">
                    <p>"Event Planner made organizing my wedding a breeze. Highly recommended!"</p>
                    <p className="author">- Emily Johnson</p>
                </div>
                <div className="testimonial">
                    <p>"I use Event Planner for all my corporate events. It saves me so much time and effort!"</p>
                    <p className="author">- John Smith</p>
                </div>
            </section>
Copied!
The output will display as shown in the given screenshot after the Features section.

Create Contact Section
Now, create a contact section so that any visitor to the webpage can easily reach out to the organization's employees.

For this again you can have one <h2> tag and one <form> tag with multiple input boxes and a <button> tag inside section tag with class name contact.

1
2
3
4
5
6
7
8
9
<section className="contact">
                <h2>Contact Us</h2>
                <form>
                    <input type="text" placeholder="Name" />
                    <input type="email" placeholder="Email" />
                    <textarea placeholder="Message"></textarea>
                    <button className="submit-button">Send</button>
                </form>
            </section>
Copied!
Now re-run the application again in the terminal and ceck the output. The output will display as shown in the screenshot.



Click here for the entire code of EventPlanner.jsx component
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
68
69
70
71
72
73
74
75
76
77
78
79
80
81
82
83
  import React from 'react';
  import './EventPlanner.css'; // Import CSS file for styling
 const EventPlanner = () => {
     return (
  <div className="event-planner-container">
             <header>
         <h1>Welcome to Event Planner</h1>
     </header>
     <section className="description">
         <p>
             Plan and organize your events effortlessly with Event Planner. From
             birthdays to corporate meetings, we've got you covered.
         </p>
         <button className="get-started-button">Get Started</button>
     </section>
     <section className="events_categories">
         <ul>
             <h2>Social Events:</h2>
             <li>Birthday parties</li>
             <li>Anniversary celebrations</li>
             <li>Wedding receptions</li>
             <li>Baby showers</li>
             <li>Graduation parties</li>
             <li>Family reunions</li>
         </ul>
         <ul>
             <h2> Entertainment Events:</h2>
             <li>Concerts</li>
             <li>Music festivals</li>
             <li>Film screenings</li>
             <li>Comedy shows</li>
             <li>Art exhibitions</li>
             <li>Cultural events</li>
         </ul>
         <ul>
             <h2>Community Events:</h2>
             <li>Fundraising events</li>
             <li>Charity galas</li>
             <li>Volunteer drives</li>
             <li>Neighborhood block parties</li>
             <li>Community festivals</li>
             <li>Cultural celebrations</li>
         </ul>
     </section>
     <section className="features">
         <h2>Features</h2>
         <ul>
             <li>Easy event creation and management</li>
             <li>Customizable event templates</li>
             <li>Guest list management</li>
             <li>Real-time collaboration</li>
             <li>Reminders and notifications</li>
         </ul>
     </section>
     <section className="testimonials">
         <h2>Testimonials</h2>
         <div className="testimonial">
             <p>"Event Planner made organizing my wedding a breeze. Highly recommended!"</p>
             <p className="author">- Emily Johnson</p>
         </div>
         <div className="testimonial">
             <p>"I use Event Planner for all my corporate events. It saves me so much time and effort!"</p>
             <p className="author">- John Smith</p>
         </div>
     </section>
     <section className="contact">
         <h2>Contact Us</h2>
         <form>
             <input type="text" placeholder="Name" />
             <input type="email" placeholder="Email" />
             <textarea placeholder="Message"></textarea>
             <button className="submit-button">Send</button>
         </form>
     </section>
 </div>
 );
 };
 export default EventPlanner;


Practice Exercise
In this practice exercise you will create one footer component which will be included in the EventPlanner.jsx component. With the help of this you will understand the concept of composition if components as well.

For this you need to right click on Components folder after selecting it and select New File. Give this new file name Footer.jsx. This will create a new component inside Components folder.

Inside Footer.jsx component, first create basic layout for the function component.

Hint: Use function component boiler plate to create this layout.

Click here for the solution
1
2
3
4
5
6
7
8
    import React from 'react';
    const Footer = () => {
            return (
        <>
        </>
    )}
export default Footer
Copied!
create one <footer> tag and you can include any information you want to display about the organization.

Hint: Use footer tag and include multiple tags such as <p>, <div> or <section> tag.

Click here for the solution
Include Footer.jsx component as last tag of div with class name event-planner-container within EventPlanner.jsx component.

Hint: Use import keyword to include Footer component as child at the top in parent EventPlanner component.

Click here for the solution
1
2
3
     import Footer from './Footer';
// include Footer component as attribute as below
<Footer/>
Copied!
6. Check the output by re-running the application again. The output of footer will be displayed acoording to given screenshot.


Note: To see the latest changes you need to execute npm run preview again in the terminal.

Click here for the entire code of EventPlanner.jsx component
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
17
18
19
20
21
22
23
24
25
26
27
28
29
30
31
32
33
34
35
36
37
38
39
40
41
42
43
44
45
46
47
48
49
50
51
52
53
54
55
56
57
58
59
60
61
62
63
64
65
66
67
68
69
70
71
72
73
74
75
76
77
78
79
80
81
 import React from 'react';
 import './EventPlanner.css'; // Import CSS file for styling
 import Footer from './Footer';
 const EventPlanner = () => {
 return (
     <div className="event-planner-container">
         <header>
             <h1>Welcome to Event Planner</h1>
         </header>
         <section className="description">
             <p>
                 Plan and organize your events effortlessly with Event Planner. From
                 birthdays to corporate meetings, we've got you covered.
             </p>
             <button className="get-started-button">Get Started</button>
          </section>
          <section className="events_categories">
             <ul>
                 <h2>Social Events:</h2>
                 <li>Birthday parties</li>
                 <li>Anniversary celebrations</li>
                 <li>Wedding receptions</li>
                 <li>Baby showers</li>
                 <li>Graduation parties</li>
                 <li>Family reunions</li>
             </ul>
             <ul>
                 <h2> Entertainment Events:</h2>
                 <li>Concerts</li>
                 <li>Music festivals</li>
                 <li>Film screenings</li>
                 <li>Comedy shows</li>
                 <li>Art exhibitions</li>
                 <li>Cultural events</li>
             </ul>
             <ul>
                 <h2>Community Events:</h2>
                 <li>Fundraising events</li>
                 <li>Charity galas</li>
                 <li>Volunteer drives</li>
                 <li>Neighborhood block parties</li>
                 <li>Community festivals</li>
                 <li>Cultural celebrations</li>
             </ul>
         </section>
         <section className="features">
             <h2>Features</h2>
             <ul>
                 <li>Easy event creation and management</li>
                 <li>Customizable event templates</li>
                 <li>Guest list management</li>
                 <li>Real-time collaboration</li>
                 <li>Reminders and notifications</li>
             </ul>
         </section>
         <section className="testimonials">
             <h2>Testimonials</h2>
             <div className="testimonial">
                 <p>"Event Planner made organizing my wedding a breeze. Highly recommended!"</p>
                 <p className="author">- Emily Johnson</p>
             </div>
             <div className="testimonial">
                 <p>"I use Event Planner for all my corporate events. It saves me so much time and effort!"</p>
                 <p className="author">- John Smith</p>
             </div>
         </section>
         <section className="contact">
             <h2>Contact Us</h2>
             <form>
                 <input type="text" placeholder="Name" />
                 <input type="email" placeholder="Email" />
                 <textarea placeholder="Message"></textarea>
                 <button className="submit-button">Send</button>
             </form>
         </section>
         <Footer/>
     </div>
    );
 };
  export default EventPlanner;
Copied!
Click here for the entire code of Footer.jsx component

      import React from 'react';
     const Footer = () => {
         return (
             <>
      <footer>
      <p>&copy; Event Planner Organization. All rights reserved.</p>
      </footer>
             </>
         )}
     export default Footer