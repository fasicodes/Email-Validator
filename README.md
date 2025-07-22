#i am writing a program through which we chick the email it is vilid or not
email = input("Enter the Email:  ")        #(f@f.in) --- -- > it is the simple of email
d,g,f=0,0,0
if len(email) >= 6:
    if email[0].isalpha() :
        if (email.count("@") == 1) and  ( "@" in email) :
            if (email[-3] ==".") ^ (email[-4] == ".") :
                for i in email :
                   if i == i.isspace() :
                        d = 1
                   elif  i.isalpha():
                      if  i == i.upper():
                         g = 1
                   elif i.isdigit():
                        continue
                   elif i == "_" or i== "." or i == "@":
                        continue
                   else :
                        f=1
                            
                if d == 1 or g== 1 or f == 1:
                    print("Yor email is wrong please chick the space , must all letter is small , and nothing special character is used")  
                else :
                    print(" email")      
            else :
                print("Wrong Email because the use of '.' is not correct location")
            
        else :
            print ("Wrong Email because the @ is used more than one")
    
    else :
        print("Wrong Email because the first letter is not aphabet ")

else :
    print("Wrong Email because in email all letter is not avaliable")
                        
            
        
                               
                          

