---
layout: project
type: project
image: img/DaClub2.png
title: "Da Club"
date: 2024-12-13
published: true
labels:
  - Programming
  - Javascript
  - Typescript
summary: "Da Club"
---
<div>
<img class="img-fluid" src="{{ site.baseurl }}/img/DaClub.png" alt="Da Club Image"> 
</div>

<h2>Overview on Da Club</h2>
UH Manoa definitely has a large catalogue of its respective clubs and various registered independent organizations (RIOs) but has the issue of lack of exposure. The most that there is of these RIOs is a spreadsheet online that isn’t necessarily the most telling representative of what the organization is about. For those that are really into looking for these organizations, this process isn't much of a problem, but we hope to streamline the steps into a more pleasing and welcoming site.

DaClub is an application that me and 4 others have developed to allow for site visitors to view UH Manoa’s RIOs in an aesthetic and organized fashion. Upon entering the site, users can log in with their profiles, create them if they don’t have one, view the clubs, and even start a club should they run one! The clubs can be shown and explored through using the club list that we have available. This is the main page that users are here for, allowing for quick and easy access to club information. Among what's presented is the organization's respective name, description, website, meeting times and locations, and photos.



<h2>Working on DaClub</h2>

Before working on the project itself, came team formation. We were a group of 5 and our team name ICS Code Crew. We made our regular meeting times, team contract, and started to brainstorm on how to implement an application that does what we set out to do. This was before the formal Milestone portion of our project development. There was a brief discussion of how work was to be distributed and who would do certain aspects. We decided that there isn't any set in stone role and that everyone can bounce to whatever issue or problem needed help in.

We carried on towards the starting of our app development, entering milestone 1, marking general development. From this point, we mainly focused on the logic of what we would add. We created our respective landing pages, edit and add forms, email format, databases, and most challenging, schema. For the most part, we got a lot of our functions up and running but we had some difficulties with some part. The schema proved to be the hardest portion but once we got it up and running, the rest was able to fall into place. Milestone 1 was completed and we had the baseline for our application. 

Come milestone 2, we further refined what we already had and added the addClub function, albeit a bit late. This allowed us to start adding real world data from the RIO spreadsheet. We worked further on what users would want to see and that was visual, so we worked on improving the user interface (UI) design of our site and made sure that everything was intuitive yet simple. Milestone 2 marked the end of adding new features while locking in the UI design that we had.

The next and final milestone, milestone 3 marked testing and application. From this point, playwright testing was implemented, making sure that our application passes the test while also applying whatever real data that we can from the RIO spreadsheet. With upwards of dozens of clubs in the database, we show the potential for our application. 


<div>
<img class="img-fluid" src="{{ site.baseurl }}/img/LandingPage.png" alt="Landing Page Image"> 
</div>
*The 'Landing Page' of DaClub, welcoming users to explore various clubs*

<div>
<img class="img-fluid" src="{{ site.baseurl }}/img/ClubList.png" alt="Club List Image"> 
</div>
*The 'Club List' page, listing clubs currently registered and active*









You can find the source code for DaClub on [GitHub](https://github.com/ics-314-code-crew).

You can find more information about the project on [our website](https://daclub-omega.vercel.app/).




#include <iostream>

using namespace std;


class Animal{
    protected:
        string type, color;
    public:
        void eat(){
            cout << "I can eat! Munch munch!" << endl;
        }

        void sleep(){
            cout << "I can sleep! Snoooze..." << endl;
        }

        void setColor(string input){
            color = input;
        }
        string getColor(){
            return color;
        }

};

class dog : public Animal{
    public:
        void bark(){
           cout << "I can bark! Woof woof!!" << endl;
        }
        void setType(string input){
            type = input;
        }
        void displayInfo(){
            cout << "I am a " << type << endl;
            cout << "My color is " << color << endl;
        }
     
};

class cat : public Animal{
    public:
        void meow(){
            cout << "I can meow! Meow meow!!" << endl;
        }   
        void setType(string input){
            type = input;
        }
        void displayInfo(){
            cout << "I am a " << type << endl;
            cout << "My color is " << color << endl;
        }        
};

int main() {

    dog pup;
    pup.setColor("black");
    pup.setType("mammal");
    pup.eat();
    pup.sleep();
    pup.bark();
    pup.displayInfo();

    printf("\n");

    cat kitten;
    kitten.setColor("white");
    kitten.setType("mammal");
    kitten.eat();
    kitten.sleep();
    kitten.meow();
    kitten.displayInfo();

    return 0;
}



<hr>

<pre>

</pre>

<hr>

 <!-- Source: <a href="https://github.com/jogarces/ics-313-text-game"><i class="large github icon "></i>jogarces/ics-313-text-game</a> -->
