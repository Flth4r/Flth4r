import tkinter as tk

def dodawanie():
    try:
        wynik.set(float(entry1.get()) + float(entry2.get()))
    except ValueError:
        wynik.set("Błąd")

def odejmowanie():
    try:
        wynik.set(float(entry1.get()) - float(entry2.get()))
    except ValueError:
        wynik.set("Błąd")

def mnożenie():
    try:
        wynik.set(float(entry1.get()) * float(entry2.get()))
    except ValueError:
        wynik.set("Błąd")

def dzielenie():
    try:
        wynik.set(float(entry1.get()) / float(entry2.get()))
    except ValueError:
        wynik.set("Błąd")

def potęgowanie():
    try:
        wynik.set(float(entry1.get()) ** float(entry1.get()))
    except ValueError:
        wynik.set("Błąd")

def obwód():
    obwod = tk.Tk()
    obwod.title("Obwody")

    tk.Button(obwod, text="Kwadrat", command=kwadrat).grid(row=1, column=0)
    tk.Label(obwod, text="Obw:4a").grid(row=1, column=1)
    tk.Button(obwod, text="Prostokąt", command=prostokąt).grid(row=2, column=0)
    tk.Label(obwod, text="Obw:2a+2b").grid(row=2, column=1)
    tk.Button(obwod, text="Rąb", command=rąb).grid(row=3, column=0)
    tk.Label(obwod, text="Obw:4a").grid(row=3, column=1)
    tk.Button(obwod, text="Równoległobok", command=równoległobok).grid(row=4, column=0)
    tk.Label(obwod, text="Obw:2a+2b").grid(row=4, column=1)
    tk.Button(obwod, text="Trójkąt", command=trójkąt).grid(row=5, column=0)
    tk.Label(obwod, text="Obw:a+b+c").grid(row=5, column=1)
    tk.Button(obwod, text="Trójkąt Równoboczny", command=trójkąt_równoboczny).grid(row=6, column=0)
    tk.Label(obwod, text="Obw:3a").grid(row=6, column=1)
    tk.Button(obwod, text="Trapez", command=trapez).grid(row=7, column=0)
    tk.Label(obwod, text="Obw:a+b+c+d").grid(row=7, column=1)
    tk.Button(obwod, text="Równoległobok Równoboczny", command=równoległobko_równobocznny).grid(row=8, column=0)
    tk.Label(obwod, text="Obw:4a").grid(row=8, column=1)
    tk.Button(obwod, text="Koło", command=koło).grid(row=9, column=0)
    tk.Label(obwod, text="Obw:2*π*r").grid(row=9, column=1)

def kwadrat():
    try:
        wynik.set(float(entry5.get()) * 4)
    except ValueError:
        wynik.set("Błąd")

def prostokąt():
    try:
        wynik.set(float(entry5.get()) * 2 + float(entry6.get()) * 2)
    except ValueError:
        wynik.set("Błąd")

def rąb():
    try:
        wynik.set(float(entry5.get()) * 4)
    except ValueError:
        wynik.set("Błąd")

def równoległobok():
    try:
        wynik.set(float(entry5.get()) * 2 + float(entry6.get()) * 2)
    except ValueError:
        wynik.set("Błąd")

def trójkąt():
    try:
        wynik.set(float(entry5.get()) + float(entry6.get()) + float(entry7.get()))
    except ValueError:
        wynik.set("Błąd")

def trójkąt_równoboczny():
    try:
        wynik.set(float(entry5.get()) * 3)
    except ValueError:
        wynik.set("Błąd")

def trapez():
    try:
        wynik.set(float(entry5.get()) + float(entry6.get()) + float(entry7.get()) + float(entry8.get()))
    except ValueError:
        wynik.set("Błąd")

def równoległobko_równobocznny():
    try:
        wynik.set(float(entry5.get()) * 4)
    except ValueError:
        wynik.set("Błąd")

def koło():
    try:
        wynik.set(float(entry9.get()) * 2 * 3,14)
    except ValueError:
        wynik.set("Błąd")

def pole():
    pola = tk.Tk()
    pola.title("Pola")
    tk.Button(pola, text="Kwadrat", command=kwadrat1).grid(row=1, column=0)
    tk.Label(pola, text="Pole:a*a").grid(row=1, column=1)
    tk.Button(pola, text="Prostokąt", command=prostokąt1).grid(row=2, column=0)
    tk.Label(pola, text="Pole:a*b").grid(row=2, column=1)
    tk.Button(pola, text="Rąb", command=rąb1).grid(row=3, column=0)
    tk.Label(pola, text="Pole:e*f").grid(row=3, column=1)
    tk.Button(pola, text="Równoległobok", command=równoległobok1).grid(row=4, column=0)
    tk.Label(pola, text="Pole:a*h").grid(row=4, column=1)
    tk.Button(pola, text="Trójkąt", command=trójkąt1).grid(row=5, column=0)
    tk.Label(pola, text="Pole:0,5ah").grid(row=5, column=1)
    tk.Button(pola, text="Trójkąt Równoboczny", command=trójkąt_równoboczny1).grid(row=6, column=0)
    tk.Label(pola, text="Pole:a^2√3/4").grid(row=6, column=1)
    tk.Button(pola, text="Trapez", command=trapez1).grid(row=7, column=0)
    tk.Label(pola, text="Pole:(a+b)*h /2").grid(row=7, column=1)
    tk.Button(pola, text="Koło", command=koło1).grid(row=8, column=0)
    tk.Label(pola, text="Pole:π*r^2").grid(row=8, column=1)

def kwadrat1():
    try:
        wynik.set(float(entry5.get()) * float(entry5.get()))
    except ValueError:
        wynik.set("Błąd")

def prostokąt1():
    try:
        wynik.set(float(entry5.get()) * float(entry6.get()))
    except ValueError:
        wynik.set("Błąd")

def rąb1():
    try:
        wynik.set(float(entry5.get()) * float(entry6.get()) / 2)
    except ValueError:
        wynik.set("Błąd")

def równoległobok1():
    try:
        wynik.set(float(entry5.get()) * float(entry7.get()))
    except ValueError:
        wynik.set("Błąd")

def trójkąt1():
    try:
        wynik.set(float(entry5.get()) * float(entry10.get()) / 2)
    except ValueError:
        wynik.set("Błąd")

def trójkąt_równoboczny1():
    try:
        wynik.set(float(entry5.get()) * float(entry5.get()) * 1.73 / 4)
    except ValueError:
        wynik.set("Błąd")


def trapez1():
    try:
        wynik.set((float(entry5.get()) + float(entry6.get())) * float(entry10.get()) / 2)
    except ValueError:
        wynik.set("Błąd")

def koło1():
    try:
        wynik.set(3.14 * float(entry9.get()) * float(entry9.get()))
    except ValueError:
        wynik.set("Błąd")

def równoległobok_równoboczny1():
    try:
        wynik.set(float(entry5.get()) * float(entry10.get()))
    except ValueError:
        wynik.set("Błąd")

def Objętość():
    objentosc = tk.Tk()
    objentosc.title("Objętość")
    tk.Button(objentosc, text="Sześcian", command=sześcian).grid(row=1, column=0)
    tk.Label(objentosc, text="Obj:a^3").grid(row=1, column=1)
    tk.Button(objentosc, text="Prostopadłościan", command=prostopadłościan).grid(row=2, column=0)
    tk.Label(objentosc, text="Obj:a*b*c").grid(row=2, column=1)
    tk.Button(objentosc, text="Graniastosłup", command=graniastosłup).grid(row=3, column=0)
    tk.Label(objentosc, text="Obj:Pp*H").grid(row=3, column=1)
    tk.Button(objentosc, text="Ostrosłup", command=ostrosłup).grid(row=4, column=0)
    tk.Label(objentosc, text="Obj:Pp*H").grid(row=4, column=1)
    tk.Button(objentosc, text="Walec", command=walec).grid(row=5, column=0)
    tk.Label(objentosc, text="Obj:πr^2*H").grid(row=5, column=1)

def sześcian():
    try:
        wynik.set(float(entry5.get()) * float(entry5.get()) * float(entry5.get()))
    except ValueError:
        wynik.set("Błąd")

def prostopadłościan():
    try:
        wynik.set(float(entry5.get()) * float(entry6.get()) * float(entry7.get()))
    except ValueError:
        wynik.set("Błąd")

def graniastosłup():
    try:
        wynik.set(float(entry11.get()) * float(entry10.get()))
    except ValueError:
        wynik.set("Błąd")

def ostrosłup():
    try:
        wynik.set(float(entry11.get()) * float(entry10.get()))
    except ValueError:
        wynik.set("Błąd")   

def walec():
    try:
        wynik.set(3.14 * (float(entry9.get()) * float(entry9.get())) * float(entry10.get()))
    except ValueError:
        wynik.set("Błąd")       

def Pole_Powierzchni():
    powierzchnia = tk.Tk()
    powierzchnia.title("Pola Powierzchni")
    tk.Button(powierzchnia, text="Sześcian", command=szescian1).grid(row=1, column=0)
    tk.Label(powierzchnia, text="Pole Pow:6a^2").grid(row=1, column=1)
    tk.Button(powierzchnia, text="Prostopadłościan", command=prostopadłościan1).grid(row=2, column=0)
    tk.Label(powierzchnia, text="Pole Pow:2ab+2ac+2bc").grid(row=2, column=1)
    tk.Button(powierzchnia, text="Graniastosłup", command=graniastosłup1).grid(row=3, column=0)
    tk.Label(powierzchnia, text="Pole Pow:2Pp + Pb").grid(row=3, column=1)
    tk.Button(powierzchnia, text="Ostrosłup", command=ostrosłup1).grid(row=4, column=0)
    tk.Label(powierzchnia, text="Pole Pow:Pp + Pb").grid(row=4, column=1)
    tk.Button(powierzchnia, text="Kula", command=kula1).grid(row=5, column=0)
    tk.Label(powierzchnia, text="Pole Pow:4πr^2").grid(row=5, column=1)

def szescian1():
    try:
        wynik.set(6 * (float(entry5.get()) * float(entry5.get())))
    except ValueError:
        wynik.set("Błąd")

def prostopadłościan1():
    try:
        wynik.set( 2 * (float(entry5.get()) * float(entry6.get())) + 2 * (float(entry5.get()) * float(entry7.get())) + 2 * (float(entry6.get()) * float(entry7.get())))
    except ValueError:
        wynik.set("Błąd")

def graniastosłup1():
    try:
        wynik.set( 2 * float(entry11.get()) + float(entry12.get()))
    except ValueError:
        wynik.set("Błąd")

def ostrosłup1():
    try:
        wynik.set(float(entry11.get()) + float(entry12.get()))
    except ValueError:
        wynik.set("Błąd")

def kula1():
    try:
        wynik.set(4* 3.14 * (float(entry9.get()) * float(entry9.get())))
    except ValueError:
        wynik.set("Błąd")

root = tk.Tk()
root.title("Kalkulator")

entry1 = tk.Entry(root)
entry2 = tk.Entry(root)
wynik = tk.StringVar()


entry5 = tk.Entry(root)
entry6 = tk.Entry(root)
entry7 = tk.Entry(root)
entry8 = tk.Entry(root)
entry9 = tk.Entry(root)
entry10 = tk.Entry(root)
entry11 = tk.Entry(root)
entry12 = tk.Entry(root)

tk.Label(root, text="Liczba a:").grid(row=6, column=0)
entry5.grid(row=6, column=1)

tk.Label(root, text="Liczba b:").grid(row=7, column=0)
entry6.grid(row=7, column=1)

tk.Label(root, text="Liczba c:").grid(row=8, column=0)
entry7.grid(row=8, column=1)

tk.Label(root, text="Liczba d:").grid(row=9, column=0)
entry8.grid(row=9, column=1)

tk.Label(root, text="Liczba r:").grid(row=10, column=0)
entry9.grid(row=10, column=1)

tk.Label(root, text="Liczba h i H:").grid(row=11, column=0)
entry10.grid(row=11, column=1)

tk.Label(root, text="Liczba Pp:").grid(row=12, column=0)
entry11.grid(row=12, column=1)

tk.Label(root, text="Liczba Pb:").grid(row=13, column=0)
entry12.grid(row=13, column=1)


tk.Label(root, text="Liczba 1:").grid(row=0, column=0)
entry1.grid(row=0, column=1)

tk.Label(root, text="Liczba 2:").grid(row=1, column=0)
entry2.grid(row=1, column=1)


tk.Button(root, text="Dodaj", command=dodawanie).grid(row=4, column=0)
tk.Button(root, text="Odejmij", command=odejmowanie).grid(row=4, column=1)
tk.Button(root, text="Pomnóż", command=mnożenie).grid(row=4, column=2)
tk.Button(root, text="Podziel", command=dzielenie).grid(row=4, column=3)
tk.Button(root, text="Potęgowanie", command=potęgowanie).grid(row=4, column=4)
tk.Button(root, text="Obwody", command=obwód).grid(row=4, column=5)
tk.Button(root, text="Pola", command=pole).grid(row=4, column=6)
tk.Button(root, text="Objętości", command=Objętość).grid(row=4, column=7)
tk.Button(root, text="Pola Powierzchni", command=Pole_Powierzchni).grid(row=4, column=8)

tk.Label(root, text="Wynik:").grid(row=5, column=0)
tk.Label(root, textvariable=wynik).grid(row=5, column=1)

root.mainloop()
