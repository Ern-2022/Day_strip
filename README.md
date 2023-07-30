# Day_strip
#I will use as main datetime library, when developing the program I can add other libraries. This program will subtract days in the one year to show how many days, hours and seconds are left until your birthday 🥳

from datetime import datetime
from time import sleep
date_now = datetime.now()
print("CURRENT DATE:",date_now)
print("WEEKS:",date_now.strftime("%A"))
print()

print("Example >> 02/05/2016 16:00")
date_pn = str(input("Do you want to predict his birthday for what year: ")).strip()
if len(date_pn) == 16:
 date_pn = datetime.strptime(date_pn,"%d/%m/%Y %H:%M")
 sum_date = date_pn - date_now 
 print(f"Missing {sum_date.days} days to your birthday")
 print("Day of the week:",date_pn.strftime("%A in %B at %H:%M hours"))
 for x in range(10,-1,-1):
  print(x)
  sleep(1)
 sleep(1.3)
 print()
 print("congratulations!")
 sleep(1.3)
 print("For you!")
 sleep(1.3)
 print("congratulations!")
 sleep(1.3)
 print("For you.")
 sleep(1)
 print()
 print("Have many years to live... ")
# Added colors as gifts🎁
 sleep(1)
 print("\033[1;42m    \033[m \033[1;43m    \033[m \033[7;40m    \033[m \033[1;41m    \033[m")
 sleep(1)
 print()
 print("\033[1;36mGoodbye! until your next birthday\033[m")
else:
 print("Error! Follow the example above!")

