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
<img src="img/DaClub.png"> 
</div>
UH Manoa definitely has a large catalogue of its respective clubs and various registered independent organizations (RIOs) but has the issue of lack of exposure. The most that there is of these RIOs is a spreadsheet online that isn’t necessarily the most telling representative of what the organization is about.

DaClub is an application that me and 4 others have developed to allow for site visitors to view UH Manoa’s RIOs. From there, users can log in with their profiles, create them if they don’t, view the clubs, and even start a club should you run one!






In this assignment from ICS 212, we were told to implement an Animal class that had various methods, variables, and instances of said object. 

It started with the declaration of various variables, all protected as to not be accessible outside of the class and its descendants. Then the public methods that can be accessed from anywhere.
Methods like eat, sleep, setcolor and get color can be used. Then respective dog and cat classes are made, extending the Animal class. They override the methods within the Animal class and 
modify them to whatever they are set to. 

This assignment helped us to to get familiar with classes, inheritance, and privacy modifiers like public, protected, and private.

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
