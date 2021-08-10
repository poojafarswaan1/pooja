# pooja
#rolling dice simulator.
rom tkinter import *
import random

root = Tk()

root.title("dice simulator")

root.geometry("600x500")

label = Label(root, font = ("Helvitica" , 350 , 'bold'), text = "" ,fg = "pink"  )

def rolldice():
    dice = ['\u2680','\u2681','\u2682','\u2683','\u2684','\u2685']
    label.configure(text = f'{random.choice(dice)}')
    label.pack()
    

button = Button(root, font = ("helvitica", 20, 'bold'), text = "dice roll" , command = rolldice , bg = "light yellow", fg = "red")
button.pack()
                            
root.mainloop()
