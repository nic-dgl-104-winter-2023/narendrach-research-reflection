# Narendra's Research and Reflection Journal

This is my research and reflection journal for DGL 104 winter 2023

# course goals

- Learning javascript in class and java languages simultaniously to helps in the future.
- Spending 5 to 6 hours on weekends to getting know better in the language.
- In time work completion and submission.
- From community code project i have don lot of rsearch for the finding logics and learnet new thing which is related to the java and oops concepts and also usage of oops in every usefull manner in the code.
- Want to use this in an organization i am going to work and get better in using those new technology.
- Perfect in what i am learning in this course.
- Learned java script along with lectures and done my own research where i am feeling difficult and applied those problems again in the code and solved by own.
- Through Community code works i am practicing java and writing some codes for issues and finding solutions to issues.
- From learning java helped me in learning new language called javascript where it is a essential language for user interactions in Html and css based websites and mobile sites.
- Where both the languages are littile bit similar and especially identical syntax helps in learning in fast manner and it is used in while writting in code for html pages.
- As i mentioned earlier by learning the programing language i wanted todevelop an site which is informative for the people and that same is i am developing through main project in the capstone by using this learning experience.
- These codes are validating better than at start of the semester and encourages me to work more and learn the important things.
- These learning things are possible because as my intention with these languages are positive and also very helpful in future endouver as well as in the course that running now.

## interests

- _Get_ a nice job and make satisfied with my job.
- Up to date with the new technologies.
- I want to learn HTML, CSS and scripting languages for my future goal, where these are source to make a website and run's in a effective manner.
- Want to develop one site for my village and local area about things in the places.
-

## Come up

- Develop web app or mobile app for my region on places. It helps in outer people know about particular place.
- Work through the knowledge you have keep track on it.
- Make sure to revise what you know and what has to do.
- I am working on my programming skills and language where it helps me in the project and some other courses, by spending some time on the outcomes of this course.
- By using javascript i have added some _onclick()_ method calling alerts to my page in project and done some dynamic changes to the pages in the site.
- Created some notification alerts for user informative alerts by spending some time across browsing things that i need.
- While learning the java and javascript(in class) gives confidence that we can make our own logic without search or asking someone for help.
- This helped me in making my project more interactive and user attention inaddition. these knowlwdge i have used in while clicking the buttons and also pop ups in the page that alerts user any warning or error in the operation.

# Reflection of Style guide

- The majority of class and interface names start with a capital letter and are nouns or noun phrases.
- Most method names start with a lowercase letter. A procedure name is typically a verb phrase that is a command to do something since a call on a process is a statement to do something.

- `void setTitle() public`
  Lowercase letters are typically used to begin variable names.
- The reader should be given suggestions in the variable names as to what they are utilized for. A well-documented program is simpler to understand and benefits from names that hint at the variable's meaning.
- On the other side, calling your variable names after your friends or your favourite flowers and complicates the application. Avoid doing that. Additionally, avoid giving variables ambiguous names like counter, var, or data; instead, consider what the variable will actually be used for and give it a more specific name.

# Week3

## Programming Practice Article

- Testing is the topic our group selected to do in the assignment that we have to write for it.

- How to do unit testing by Sergey. K [Unit Testing and Coding: Best Practice for Unit testing | Toptal](https://www.toptal.com/qa/how-to-write-testable-code-and-why-it-matters#:~:text=A%20typical%20unit%20test%20contains,it%20observes%20the%20resulting%20behavior).
- In sergey explination, he thought about what it is and how we are using it and what are the benifits that we can achive by this unit testing.

- Unit Testing tutorial [Unit Testing Tutorial - What is, Types and Test Examples](https://www.guru99.com/unit-testing-guide.html).
- In this article there are couple of videos along with text that explains from what to when and where.these techniquies are using and uses.

- What is unit testing and how do you do it? [What is Unit Testing How do you Do it?](https://stackoverflow.com/questions/652292/what-is-unit-testing-and-how-do-you-do-it).
- In Stack overflow, there are small code snippets and testing examples and more over different people explination in their view which we can get more knowlwdge while we are searching for them.

- [Software testing methods like unit testing are essential for assuring the dependability and quality of a program. Early bug detection and correction can save time and money in the long run because it is a cost-effective method.](https://circleci.com/enterprise/)
- The ability to independently test particular pieces of code rather than having to test the complete application is one of the main advantages of unit testing.[How to do unit testing by Sergey. K](https://www.toptal.com/qa/how-to-write-testable-code-and-why-it-matters)
- This improves in spotting issues early on in the development process, before they escalate in complexity and cost to resolve. Unit tests also offer a safety net for upcoming code revisions, making it simpler to make sure that changes to one section of the code do not unintentionally break another.[Unit Testing Best Practices with .NET Core and .NET Standard.](https://learn.microsoft.com/en-us/dotnet/core/testing/unit-testing-best-practices)
- Additionally, unit testing encourages a more flexible and reusable code architecture. Developers are compelled to consider the different parts of their code in isolation and how they interact with one another when they design unit tests. As a result, the codebase is better planned and easier to maintain.[Why is unit Testing is important for developers.](https://www.techtarget.com/searchsoftwarequality/answer/Is-unit-testing-an-important-aspect-of-software-development)

# Community code

- [Find smallest number in matrix ](https://github.com/codinasion/program/issues/5129).
- [Write a java program to print number to word](https://github.com/codinasion/program/issues/2621).

```java

import java.util.Scanner;

public class PrintNumberToWord {


    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();/* User entered number.*/
        String result = convertNumberToWords(number);
        System.out.println("Result: " + result);
    }
/* The below code written on the oops based concept.
        the code is generalized with the if conditions as they are entered by the user and the conditions will be checked as a process.*/
    private static String convertNumberToWords(int number) {
        if (number == 0) {
            return "zero";
        }
        String words = "";    /* From above code words is initiated with empty quatations and also used to print whole number that we gave as input */
        if (number < 0) {
            words += "minus ";
            number = Math.abs(number);/* Math function for changing any negative number values to positive number if number is less than 0. */
        }
        /* I have written maximum number of on Billion as i am considering highest number.*/
        if (number >= 1000000000) {
            /* Here "words" will be assigned with the value that is in calling function that accepts number from user input followed by the division with a billion and returns with "billion" word.
            The same process continues with the remaining numbers upto humdreds. */
            words += convertNumberToWords(number / 1000000000) + " billion ";
            number %= 1000000000;
        }
        if (number >= 1000000) {
            words += convertNumberToWords(number / 1000000) + " million ";
            number %= 1000000;
        }
        if (number >= 1000) {
            words += convertNumberToWords(number / 1000) + " thousand ";
            number %= 1000;
        }
        if (number >= 100) {
            words += convertNumberToWords(number / 100) + " hundred ";
            number %= 100;
        }
        if (number >= 10 && number <= 19) {
            /* From this step onwards it calls another method that generates numbers below 100 as it is sub divided from here.*/
            words += getTeenNumberWord(number);
            return words;
        }
        if (number >= 20) {
            words += getTensNumberWord(number / 10) + " ";
            number %= 10;
        }
        if (number >= 1 && number <= 9) {
            words += getUnitNumberWord(number);
        }
        return words.trim();
    }
/* This Method is for numbers one to nine in single digit. instead of if condition i haev used switch condition as it is similar to each other in functioning. */
    private static String getUnitNumberWord(int number) {
        switch (number) {
            case 1:
                return "one";
            case 2:
                return "two";
            case 3:
                return "three";
            case 4:
                return "four";
            case 5:
                return "five";
            case 6:
                return "six";
            case 7:
                return "seven";
            case 8:
                return "eight";
            case 9:
                return "nine";
            default:
                return "";
        }
    }
/* This method returns values from ten to ninteen which are different for writing as compared to othe duble digit numbers.*/
    private static String getTeenNumberWord(int number) {
        switch (number) {
            case 10:
                return "ten";
            case 11:
                return "eleven";
            case 12:
                return "twelve";
            case 13:
                return "thirteen";
            case 14:
                return "fourteen";
            case 15:
                return "fifteen";
            case 16:
                return "sixteen";
            case 17:
                return "seventeen";
            case 18:
                return "eighteen";
            case 19:
                return "nineteen";
            default:
                return "";
        }
    }
/*This method returns tens values upto ninty. */
    private static String getTensNumberWord(int number) {
        switch (number) {
            case 2:
                return "twenty";
            case 3:
                return "thirty";
            case 4:
                return "forty";
            case 5:
                return "fifty";
            case 6:
                return "sixty";
            case 7:
                return "seventy";
            case 8:
                return "eighty";
            case 9:
                return "ninety";
            default:
                return "";
        }
    }
}

```

- To write code for this issue it took lot of time. it took one who;e day to crack the exact code and sort it in the program and worked on the some of the examples to get used to it.
- First i have used while loop to sole the problem and it didn't worked, then searched posibilities fo code and then found some example but not exact and then written with switch case statement to get the required output.

- [Write a java program to convert centimeter to meter](https://github.com/codinasion/program/issues/2374).~~
- [Write a java program to print string of ascii values](https://github.com/codinasion/program/issues/1639).
- [Write a program to convert a hours to weeks](https://github.com/codinasion/program/issues/1604).~~

```java
import java.util.Scanner;

public class HoursToWeeks {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);

      // Get the number of hours from the user
      System.out.print("Enter the number of hours: ");
      int hours = input.nextInt();

      // Calculate the number of weeks by performing math operation for user given hours with number of days in a week by hours in a day(standard values). 
      int weeks = hours / (7 * 24);

      // Output the result with the text with calculated results.
      System.out.println(hours + " hours is equivalent to " + weeks + " weeks.");
   }
}
```

- convert 12 hour format to 24 hour format:

```java
import java.util.Scanner;
import java.text.SimpleDateFormat;
import java.text.DateFormat;

public class convertTimeFrom12to24hours {

   public static void main(String[] args) {
       String time12 = "02:30 PM";
       DateFormat inFormat = new SimpleDateFormat("hh:mm aa"); // This Java file is a predefined with the conversions that we can use directly by importing the necessary libraries into our code. 
       DateFormat outFormat = new SimpleDateFormat("HH:mm");

       try {
           Date date = inFormat.parse(time12);
           String time24 = outFormat.format(date);
           System.out.println("24-hour format: " + time24);
       } catch (ParseException e) {
           e.printStackTrace();
       }
   }
}
```

- The above example was i found in the git hub, i started working on the issue in a simple manner but meanwhile soneone solve it and i decided to choose an another way of solving the problem in try and catch method of solving with the use of predefined java classes in the library.
- For above example i have applied try and catch methods because when i am learning java in CPS-100 i have practiced all types in this type of section also i have seen many examples so i didn,t find any example with these methods so, i started working on it and found solution.

- [Write a Java program to calculate compound interest](https://github.com/codinasion/program/issues/1362).

```java
import java.util.Scanner;

public class CalculateCompoundIntrest {

    public static void main(String[] args) {

        int principle;
        double rate, amount, time, subamt; // Declaration part for the variables

        Scanner scnr = new Scanner(System.in);

        System.out.println("enter your amount"); // Input frm the user.
        principle = scnr.nextInt();

        System.out.println("enter your Rate");
        rate = scnr.nextDouble();

        System.out.println("enter your Time");
        time = scnr.nextDouble();

        subamt = (Math.pow((1 + rate/100), time)); // I am calculating intrest amount that includes rate and  total time with math operator(predefined).
        amount = principle * subamt;   // Here i am finding actual amount with principle and data that clculated before (subamt).

        System.out.println("Total amount is " + amount);

    }
}
```

- The above example is for finding Compound Intrest. For this example i have written basic code that i learned at early stege of lerning java programming and it went through good.
- this is my first example in community code and i have done some research on to find formula it self. i have written in my own and basic form in java without any methods or object calling.

- [Write a java program to convert string to consonentcase](https://github.com/codinasion/program/issues/5150).

```java

import java.util.Scanner;



public class ConvertStringtoConsonentcase {

    public static void main(String[] args) {
        String str;
        char newstr;

        System.out.println("enter string");

        Scanner scnr= new Scanner(System.in);

        str = scnr.nextLine();

        for(int i = 0; i <= str.length(); i++){

            char ch = str.charAt(i);
            if(ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ){

                newstr = ch;
            }
            else{
                newstr = Character.toUpperCase(ch);
            }

        }
        System.out.print(newstr);
        scnr.close();
    }

}

```

- The above is good first issue that i found in my community. For this example i have used for loop and if conditions to get the desired output that user wants to test on it and its working as required.
- At starting i have found different ways to do the same problem, later just to make code legible and understands to every one i choose this way.

### Reflection on Community code

- Thank you for making us to work on the community code, from these i am learning a bit more rather than the normal learning by solving the issues and cracking the codes for good first issues and having some time with learning the new things form this Community code.

## Short reflection of Research and Reflection repository.

- Coming to this repository what i observed is i can monitor the things i have written in this journal and also can question us that what we have done and what i have to focus in the fututre to achive future goals by spending enough time on particular tasks.

## week 6 In class

- Prototype - MVP (Minimal viable Product)
- MIT app Inventor
- create space invadors app using MIT
- - things that we get from app is
- - i can see the rocket moving
- - i can see the bullet hitting
- - i can suacer horizonatal along screen
- - i can see the score changes and can reset it.

- singleton
-

## MIT App Inventor

- Created Homework MapIt app in MIT ap inventor by following tutoriols.
- created every component and botton text box and written code according to it.
- Tested the site with my android mobile its working as app apecification.
- Found an issue in the development stage that button is mentioned in the components page instead of text area so replaced it in the same area.
- I installed app in my phone and checked by the proccess how it is going through its working as it is.
- I have added address to database and retrieved when i clicked on the submit button.
- It showed address what i have entered and checked with other address and results are positive.
- When i clicked on location on the map it opened the map and din't showed any adress because location access was not provided then after turning on the location it showed my current address where i am right at that time and works same as designed.

# MIT Project Idea

- Ludo game
- It is a multiplayer game as upto 4 members can play at same time or individual can play ono on one.

-

# Week 8 In class lecture

## Model View Controller

- Frame work , libraries,programming language that implement MVC
- Ruby on Rails - PWA
- React, Angular, Embed vue
- .Net

#### Model

- Model comsists of Data(DB, Json file, Data Stored in App), Interface to Data, Business logic,

#### View

- view consists of Graphical User Interface(GUI), No Direct access to data, Representation of the model at given point in time.

#### Controller

- it Consists of Entry Points, Handles Events, controls the model.

## Week 10 replacement work

- Mit project is simple multiplayer game that has some boxes on the screen which displays players coin or players number in the box.
- The game description
- - The game has check boxes or text boxes around the screen and a dice with 6 numbers.
- - The game starts when the number appears on the screen first time and continues through boxes for the individual player
- - The game ends when one of the player reaches final spot and restarts the game again.
- - In this game if one person has to win the game he has complete one full round of boxes without overlaping with the co-players.
- - If the coins or players overlaps at same spot / box, the existing coin or person have to begin from start.s
- The players coin or number will move depending on the random number or dice that i am gone use in the app.
