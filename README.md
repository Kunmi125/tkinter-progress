from tkinter import *
from tkinter.ttk import *
import time
window = Tk()
window.configure(background = "green")
window.geometry("300x300")

'''# Determinate progress bar
pb = Progressbar(window, orient = HORIZONTAL, length = 100, mode = "determinate")
pb.pack(padx = 20, pady = 10)
def pbar():
    pb["value"] = 20
    window.update_idletasks()
    time.sleep(0.5)

    pb["value"] = 40
    window.update_idletasks()
    time.sleep(0.5)

    pb["value"] = 60
    window.update_idletasks()
    time.sleep(0.5)

    pb["value"] = 80
    window.update_idletasks()
    time.sleep(0.5)

    pb["value"] = 100
    window.update_idletasks()
    time.sleep(0.5)

b1 = Button(window, text = "Enter", command = pbar)
b1.pack(padx = 30, pady = 30)'''

# Indeterminate progress bar
pb2 = Progressbar(window, orient = VERTICAL, length = 200, mode = "indeterminate")
pb2.pack(padx = 20, pady = 10)

def pbar2():
    pb2.start(50)



b2 = Button(window, text = "Enter", command = pbar2)
b2.pack(padx = 20,pady = 40)
window.mainloop()
