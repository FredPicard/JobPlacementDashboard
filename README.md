# Live Project

## Introduction

For the last two weeks of my time at the tech academy, I worked with my peers in a team developing a full scale MVC Web Application in C#. Working on a legacy codebase was a great learning oppertunity for fixing bugs, cleaning up code, and adding requested features. I saw how a good developer works with what they have to make a quality product. I worked on a couple back end stories [back end stories](#back-end-stories) that I am very proud of. Because much of the site had already been built, there were also a good deal of front end stories [front end stories](#front-end-stories) and UX improvements that needed to be completed, all of varying degrees of difficulty. Everyone on the team had a chance to work on front end and back end stories. Over the two week sprint I also had the opportunity to work on some other project management and team programming skills that I'm confident I will use again and again on future projects.</p>

## Back End Stories
* [Filter Content in Search Box](#filter-content)
* [DateTime Attribute](#datetime-attribute)




### Filter Content
This story allowed users to search content in their employee chat messages

     ViewBag.MessageSortParm = String.IsNullOrEmpty(sortOrder) ? "Message" : "";
        if (!String.IsNullOrEmpty(searchString))
                    {
                        messages = messages.Where(m => m.Sender.Contains(searchString) || m.Message.Contains(searchString));
                    }
 
 ### DateTime Attribute
The other back end story was to modify the model, controller methods and all views so it created a DateTime attribute every time a news article was contributed so it could properly sort by date created..


#### In the controller

          if (ModelState.IsValid) { companyNews.DateCreated = DateTime.Now; db.CompanyNews.Add(companyNews); db.SaveChanges(); return RedirectToAction("Index");
#### In the model
          [Display(Name = "DateCreated")]
          [DisplayFormat(DataFormatString = "{0:MM/dd/yyyy}")]
           public  DateTime DateCreated { get; set; }


*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*


## Front End Stories
* [Animated Hover Effect](#animated-hover-effect)
* [Hover Effect](#hover-effect)

### Animated Hover Effect
This story implemented a wiggle effect and text color change when hovered over widget.


            }.col-4:hover {
                /* Start the shake animation and make the animation last for 0.5 seconds */
                animation: shake 0.5s;
                /* When the animation is finished, start again */
                animation-iteration-count: infinite;
            }@keyframes shake {
                0% {
                    transform: translate(1px, 1px) rotate(0deg);
                }
                10% {
                    transform: translate(-1px, -2px) rotate(-1deg);
                }
                20% {
                    transform: translate(-3px, 0px) rotate(1deg);
                }
                30% {
                    transform: translate(3px, 2px) rotate(0deg);
                }
                40% {
                    transform: translate(1px, -1px) rotate(1deg);
                }
                50% {
                    transform: translate(-1px, 2px) rotate(-1deg);
                }
                60% {
                    transform: translate(-3px, 1px) rotate(0deg);
                }
                70% {
                    transform: translate(3px, 1px) rotate(-1deg);
                }
                80% {
                    transform: translate(-1px, -1px) rotate(1deg);
                }
                90% {
                    transform: translate(1px, 2px) rotate(0deg);
                }
                100% {
                    transform: translate(1px, -2px) rotate(-1deg);
                }

 ### Hover Effect
This front end story is another hover effect for buttons.

                navbar-nav {
                font-family: 'Raleway', Arial, sans-serif;
                text-align: left;
                text-transform: uppercase;
                font-weight: normal;
                etter-spacing: 1px;
                min-width: 10px
                }
                
               .navbar-nav * {
               -webkit-box-sizing: border-box;
                box-sizing: border-box;
               -webkit-transition: all 0.35s ease;
                transition: all 0.35s ease;
                }
                
                .navbar-nav li { 
                display: inline-block;
                list-style: outside none none;
                margin: -2.7px;
                padding: 0px;
                }
                
                .navbar-nav li:hover li {
                 display: block;
                 z-index: 99999;
                } 
                
                .navbar-nav a {
                 padding: 0px;
                 color: rgba(255, 255, 255, 0.5);
                 position: relative;
                 text-decoration: none;
                 display: inline-block;
                }
                
                .navbar-nav a:before {
                 position: absolute;
                 content: '';
                 -webkit-transition: all 0.35s ease;
                 transition: all 0.35s ease;
                 opacity: 0;
                 left: 15%;
                 right: 15%;
                 top: 0;
                 bottom: 0;
                 border-left: 3px solid #2e338c;
                 border-right: 3px solid #2e338c;
                  } 
                  
                  bar-nav a:hover,
                 .navbar-nav .current a {
                  color: #ffff .navff;
                  }

                 .navbar-nav a:hover:before,
                 .navbar-nav .current a:before {
                  opacity: 1;
                  left: 0;
                  right: 0;
                  }
                  
*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*

## Other Skills Learned
* Working with a group of developers to identify front and back end bugs to the improve usability of an application

* Improving project flow by communicating about who needs to check out which files for their current story

* Learning new efficiencies from other developers by observing their workflow and asking questions

* Practice with team programming/pair programming when one developer runs into a bug they cannot solve

*Jump to: [Front End Stories](#front-end-stories), [Back End Stories](#back-end-stories), [Other Skills](#other-skills-learned), [Page Top](#live-project)*

                  

                   

                       
                 


               

                 

       
   
 
