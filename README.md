# TBG-Action-Menu_

#CS-30- TBG Action Menu_Aarushi Sethi
#date: 13 may 2022


#choose characters
print('''
Choose operation

1)Description of the game
2)description of characters
3)Start game
''')

choice=int(input('enter choice 1/2/3: '))

#description of game
if choice == 1:
    print('''
Introduction:

This game is based on a city attacked by terrorists.
These terrorists bombarded at railway stations restaurants and many more public places.
They also attack a 5 star hotel called the Raj hotel.
Choose your character to experience what that person went through when he/she was in the hotel

''')
 
 #de
elif choice ==2:
    print('''

Description of Characters

1)Fireman:
Raj mahal hotel is on fire.
You have been sent to rescue people.
Rescuing people from different locations will help you
score points depending on from where you rescue

2)Police:
You come to know that Raj hotel and many other public
places in the city have been attacked by terrorists.
You are to be sent for duty to protect the people at the Raj hotel

3)Staff:
You are either the Headchef who is informed by his collegue Arjun,
about the attack in the hotel or you are Arjun who was on duty and
sees terrorists attack the hotel. your hotel's principle is 'Guest is God'.
You have to save your guests and yourself.
''')
    
elif choice==3:
    print('''Choose your character:\n1)Police\n2)Staff\n3)Fireman ''')
    char=int(input('\nenter choice 1/2/3: '))
    
    #police
    if char==1:
        police={1:'local police',2:'special squad commander',3:'special squad soldier'}
        for i in police:
            print(f'{i}){police[i]}')
        me=int(input('\nenter choice 1/2/3: '))
        print('''
You come to know that Raj hotel and many other public places in the city
have been attacked by terrorists. You are sent for duty to protect the
people at the Raj Mahal hotel''')
        #local police
        if me ==1:
            print('''\nYou are local police officer.
You come to know that there is an injured lady waiting
for medical help near the service stairs with a staff member.
You have to rescue her''')
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            yes=input('You have reached the location of the injured lady! press enter to rescue ')
            print('\nCongratulations! You have rescued her!')
        
        #special squad commander
        if me ==2:
            print('''\nYou are Special Squad commander.
You come to know that there are hostages stuck in the lounge .
You have to guide your team to rescue them. Give them directions''')
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            yes=input('Your team has reached the location of hostages! press enter to say go ')
            print('\nCongratulations! Your team has rescued them!')
            
        #special squad soldier
        if me ==2:
            print('''\nYou are Special Squad Soldier.
You come to know that there are hostages stuck in the lounge.
You have to rescue them.''')
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
            yes=input('You have reached the location of hostages! press enter to rescue ')
            print('\nCongratulations! You have rescued them!')
        
    
    #staff
    elif char==2:
        staff={1:'Arjun',2:'Headchef'}
        for i in staff:
            print(f'{i}) {staff[i]}')
        me=int(input('\nenter choice 1/2: '))
            
            #Arjun
        if me ==1:
                print('''You are Staff member Arjun.
You see that the hotel is under attack.
You inform your headchef and he asks you to take the guests to the lounge as it is safe.
You have to take the guests through the service stairs. ''')
                news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
                news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
                yes=input('You have reached the launge safely! press enter to secure the lounge ')
                print('\nCongratulations! You are safe with the guests!')
                
            #headchef
        elif me ==2:
                print('''You are Headchef of the raj mahal hotel.
Your collegue Arjun tell you that the hotel is under attack.
you ask him to take the guests to the lounge as it is safe,
and yourself head ther with rest of your collegues
You have to go through the service stairs. ''')
                news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
                news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
                yes=input('You have reached the launge safely! press enter to secure the lounge ')
                print('\nCongratulations! You are safe with the guests and your collegues!')
        else:
            print('choice invalid')
                
            
    #fireman
    elif char==3:
        #selecting equipments
        equipments={1:'Nozzles',2:'High performance fans',3:'Submersible pumps',
                    4:'Thermal imaging camera',5:'Firefighting devices, extinguishing agents'}
        
        for a in equipments:
            print(f'{a}) {equipments[a]}')
        
        equip=int(input('\nenter choice 1/2/3/4/5: '))
        location={1:'Kitchen',2:'lounge',3:'hallway',4:'guest room',5:'service stairs',6:'terrace'}
        
        #selecting location
        for b in location:
            print(f'{b}) {location[b]}')
        
        loc=int(input('\nchoose location 1/2/3/4/5/6: '))
        print(f'There is fire in {location[loc]}!\nUse {equipments[equip]} to extinguish fire!')
        
        #extinguish fire
        news=int(input('1)North\n2)South\n3)East\n4)West\n\nenter direction:' ))
        extinguish=input('\npress enter to extinguish')
        print('\nGood Job! Mission Successful')
            
            
               
    else:
        print('Choice invalid')
    
    
