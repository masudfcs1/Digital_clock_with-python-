from  tkinter import *
from  time import strftime

def t():
    str=strftime("%H : %M : %S %p")
    lbl.config(text=str)
    lbl.after(1000,time)

w=Tk()
w.title("Digital Clock")
lbl=Label(w,font=("Arial",100),background="black",foreground="cyan")
lbl.pack()

t()
mainloop()
