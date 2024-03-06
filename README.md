# Tobogan
print("Dobrodošli na vožnju toboganom!")
visina = int(input("Koja je vaša visina u cm? "))
racun = 0

if visina >= 120:
  print("Možete se voziti na toboganu!")
  godine = int(input("Koliko imate godina? "))
  if godine < 12:
    racun = 5
    print("Cena karte za decu je 5 dolara.")
  elif godine <= 18:
    racun = 7
    print("Cena karte za mlade je 7 dolara.")
  else:
    racun = 12
    print("Cena karte za odrasle je 12 dolara.")
  
  zeli_sliku = input("Da li želite da vam slikamo? Y ili N. ")
  if zeli_sliku == "Y":
    racun += 3
  
  print(f"Vaš ukupan račun iznosi ${racun}")

else:
  print("Nažalost, morate biti viši da biste se vozili.")

