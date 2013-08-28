first-programme
===============

simple programme from book
epic_programmer_dict={
    "tim b-l":["tbl@gmail.com",111],
    "guido VR":["gvr@gmail.com",222],
    "linus t":["lt@gmail.com",333],
    "larry page":["lp@gmail.com",444],
    "sergei bren":["sb@gmail.com",555]
    }


#adding me to the list

epic_programmer_dict["mejd"]=["mn@gdog.boi"]

def searchPeople(personsName):
    try:
        personsInfo=epic_programmer_dict[personsName]
        print "name: " + personsName.title()
        print "email: " + personsInfo[0]

    except:
        print "no info found"

userWantsMore=True
while userWantsMore==True:
    personsName=raw_input("Please enter a name: ").lower()
    searchPeople(personsName)
    userWantsMore=False
    
    searchAgain=raw_input("search again? (y/n)")
    if searchAgain=="y":
        userWantsMore=True
    elif searchAgain=="n":
        userWantsMore=False
    else:
        print "negatory"
        userWantsMore=False
