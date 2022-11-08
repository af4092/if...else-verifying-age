# if...else-verifying-age

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

1. this is the example output for following samples: name.Frank; gender.m; birthdate.1985:

![image](https://user-images.githubusercontent.com/24220136/200557320-5e8d3beb-e2af-4903-be34-5fb928bfa4b5.png)

2. this is the example output for following samples: name.Frank; gender.m; birthdate.2007:

![image](https://user-images.githubusercontent.com/24220136/200557439-d2425d05-2df9-4bcd-adda-1ebacdb94f2f.png)

3. this is the example output for following samples: name.Anna; gender.f; birthdate.1991:

![image](https://user-images.githubusercontent.com/24220136/200557588-5785c693-3ae5-4a41-ab11-7dc690d65ead.png)

4. this is the example output for following samples: name.Anna; gender.f; birthdate.2005:

![image](https://user-images.githubusercontent.com/24220136/200557717-b8cbbefc-cfaa-46a9-95c0-a0093c2d0325.png)

