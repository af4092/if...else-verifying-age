# if...else-verifying-age
if... else in the example of Age verification.
This is the simple age verification example, which firstly asks for the name and get the gender, based on this it executes particular line of codes and finally checks for age by asking the birthdate (age = 2022year-birthdate): 

    import java.util.Scanner;
    public class ifelse {
    public static void main(String args[]){
    Scanner input = new Scanner(System.in);
    String name, gender;
    Double age, birthdate;
    
    System.out.println("What is your name? ");
    name = input.nextLine();
    
    System.out.println("Please choose your gender: male / female");
        gender = input.nextLine();
        if (gender.equals("m")){
            System.out.println("Hello Mr." + name + ", please provide your date of birth: ");
                birthdate = input.nextDouble();
                age = 2022 - birthdate;
                    if (age >= 18){
                        System.out.println("Ok Mr." + name + " you can buy ALCOHOL, have nice day :)");
                    }else{
                        System.out.println("Sorry Mr." + name + ", you are not allowed to buy ALCOHOL, pls come back when you grow up :(");
                    }
        } else{
            System.out.println("Hello Ms." + name + ", please provide your date of birth: ");
                 birthdate = input.nextDouble();
                 age = 2022 - birthdate;
                        if (age >= 18){
                            System.out.println("Ok Ms." + name + " you can buy ALCOHOL, have nice day :)");
                        }else{
                            System.out.println("Sorry Ms." + name + ", you are not allowed to buy ALCOHOL, pls come back when you grow up :(");
                }
        }
    }
    }

