// kratin_Final_Project
// Hey ! This is the kind of project related to Health.  By Suraj Rambhade
package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner ns = new Scanner(System.in);

        System.out.println("Enter Your Name Maam");
        String name = ns.nextLine();
        System.out.println("Enter In Which Area Are You From ");
        String Area = ns.nextLine();

        System.out.println("Please Enter Your Valid Age Maam");
        int age = ns.nextInt();
        if (age >= 65){
            System.out.println("Yes " + name + " You Are Elegible To Cheak Your Health Status In Your "+ Area );
        }
        else {
            System.out.println("Please Come Back,  Hope Your Are Fit And Fine !");
        }

        System.out.println();

        System.out.println("Here Is The Some Quetions About Your Health, You Need To Answer");
        System.out.println("Refer Your Report To Cheak Following Are Fine ! \n \t 1. B.P \n \t 2. Pulse \n \t 3. SPO2 ");

        System.out.println("Enter The Value Of B.P");
        int bp = ns.nextInt();
        if (bp<125){
            System.out.println("Your B.P IS Low, Now You Have to Low Down Your Work Pressure, Need To Take Care With No Tension");
        }
        else if (bp>=125){
            System.out.println("Your B.P IS Well, As Age is High Follow Proper Deit Plan According To Age");
        }
        else if (bp<=181){
            System.out.println("Your B.P IS High, Now You Have to Low Down Your Work Pressure, Need To Take Care With No Tension");
        }
        else{
            System.out.println("System Can't Able To Define Your Value Re-attempt All Process Agaain, If Not Move to Next Quetions.\n Make Sure You Enter Right Key Word ");
        }

        System.out.println();

        System.out.println("You Are Done With Your Basic Tests.");
        System.out.println("Here We Need To Know About Your Eating Habits ! \n \t 1. Healthy \n \t 2. Oily \n \t 3. Spicy \n \t 4. Junk Food ");
        System.out.println("Enter Which Food You Eat More From Above list");
        Scanner eat = new Scanner(System.in);
        String eating = eat.nextLine();

        switch (eating){
            case "Healthy":
                System.out.println("Wow! In This Morden Era You Eat Healty Food well Done, keep Adding More Vegetable in Meal");
                break;
            case "Oily":
                System.out.println("Plz!,\n Avoid The Oily Food It Causes Heart Disease, Heart Burn And Many More");
                break;
            case "Spicy":
                System.out.println("Plz!,\n Avoid The Spicy Food It Causes Acidity Problem, Gases And Many More");
                break;
            case "Junk Food":
                System.out.println("Plz,\n Avoid The Junk Food It Causes Diarrhoea, Constipation And Many More" );
                break;
            default:
                System.out.println("System Can't Able To Define Your Value Re-attempt All Process Agaain, If Not Move to Next Quetions.\n Make Sure You Enter Right Key Word");
        }

        System.out.println();

        System.out.println("The Next Quetion Is About Are You Drink, Answer is Expect in \"Yes\" OR \"No\"." );

        Scanner input = new Scanner(System.in);

        String yes = input.nextLine();


        if (yes.equals("Yes")){
            System.out.println("It Very Harm For Your Health, Plz! Avoid As Much As You Can, Your Chances of Recovery Is Less If You Drink.");
        }
        else {
            System.out.println("Congratulation! You Are In safe Zone In This Age.");
        }

        System.out.println();

        System.out.println("The Next Quetion Is About The Execise,\n Have You Do Execise Answer Expected In \"Yes\" OR \"No\"");
        Scanner Execise = new Scanner(System.in);
        String ans1 = Execise.nextLine() ;
        if (ans1.equals("Yes")){
            System.out.println("Well Done! Your Chances of Recovery Is More Then Other.");
        }
        else {
            System.out.println("Do Exesise Regular! It Help You To Recover Form Any Disease. ");
        }

        System.out.println(" ");

        System.out.println(" If You Don't Mine We Want to Give Some Advice In Which You Can live a healthier and better life?");
        System.out.println("If You Allow Us, The Amswer Is Except In \"Yes\" OR \"No\" " );
        Scanner Advice = new Scanner(System.in);
        String ans2 = Advice.nextLine() ;
        if (ans2.equals("Yes")){
            System.out.println("1. Eat nourishing food." +  "\n" +
                    "2. Sleep seven to eight hours a night." + "\n" +
                    "3. Keep company with good people." + "\n" +
                    "4. Avoid news overdose. \n" +
                    "5. Get regular exercise. \n" +
                    "6. Do something meaningful each day. \n" +
                    "7. Think good thoughts for others.");
        }
        else {
            System.out.println("Stay Safe Stay Happy Tack Care Of Yourself And Family");
        }

    }
}
