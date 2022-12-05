import random


print("""

              ,---------------------------,
              |  /---------------------\  |
              | |                       | |
              | |     Password          | |
              | |      Generator &      | |
              | |       Manager         | |
              | |                       | |
              |  \_____________________/  |
              |___________________________|
            ,---\_____     []     _______/------,
          /         /______________\           /|
        /___________________________________ /  | ___
        |                                   |   |    )
        |  _ _ _                 [-------]  |   |   (
        |  o o o                 [-------]  |  /    _)_
        |__________________________________ |/     /  /
    /-------------------------------------/|      ( )/
  /-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/ /
/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/-/ /
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
""")

password = "mini"

fb_password = "facebookpass"
twit_password = "twitterpass"
insta_password = "instapass"
number = "09675123456"

password_usr = input("Enter the password :")

if password_usr == password:
                usr2 = input("Generate password[1] or Know Password[2] :")

                if usr2 == "1":
                    num = "0987654321"
                    lower = "abcdefghijklmnopqrstuvwxyz"
                    upper = "ABCDEFGHIJKLMNOPQQRSTUVWXYZ"
                    symbols = "~!@#$%^&*()"
                    length = input("How long would you like your password to be?")
                    string = num + lower + upper + symbols
                    new_password = "".join(random.sample(string, int(length)))
                    print("This is your new password :" + new_password)
           
                    

                elif usr2 == "2":
                    usr3 = input("Name of the app:")
                    if usr3 == 'facebook':
                        print("Facebook password :" + fb_password)
                        print("Phone number :" + number)
                        
                    elif usr3 == 'twitter':
                        print("Instagram password :" + insta_password)
                        print("Phone number :" + number)
                        
                    elif usr3 == 'instagram' :
                        print("Instagram password :" +insta_password)
                        print("Phone number :" + number)
                    
                    elif usr3 == "exit":
                        exit()   
                    else :
                        print("There is no password to show...") 
                    
                else :
                        print("Invalid Entry..")
