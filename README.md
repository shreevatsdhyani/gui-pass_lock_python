# guicskpython
# tkinter              it is the built in GUI of python
import os
import tkinter as tk
def do_something(ucalled):
    if user.get()=="msd":
        msg=tk.Label(win,text=os.popen("C:\\Users\\shree\\Downloads\\Chennai_Super_Kings_Logo.png"),font="Algerian 20",bg="blue").place(x=100,y=200)
    else:
        win.destroy()
        



win=tk.Tk()
win.geometry("720x720")
win.configure(bg="yellow")
tk.Label(win,text="Welcome!",font="Lucida 20",bg="skyblue").place(x=0,y=0)
user=tk.Entry(win,font="50",bg="skyblue",width=20,)
user.place(x=300,y=0)


but_ton=tk.Button(win,text="ENTER",command=do_something,font="100")
but_ton.place(x=100,y=100)

win.bind("<Return>",do_something)

win.mainloop()
