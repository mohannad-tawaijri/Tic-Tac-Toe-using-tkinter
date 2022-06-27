import tkinter.messagebox
from tkinter import *
tk = Tk()
tk.title("Tic Tac Toe")
#
# pa = StringVar()
# playerb = StringVar()
# p1 = StringVar()
# p2 = StringVar()
#
# player1_name = Entry(tk, textvariable=p1, bd=5)
# player1_name.grid(row=1, column=1, columnspan=8)
# player2_name = Entry(tk, textvariable=p2, bd=5)
# player2_name.grid(row=2, column=1, columnspan=8)


flag = 0

def disableButton():
    button1.configure(state=DISABLED)
    button2.configure(state=DISABLED)
    button3.configure(state=DISABLED)
    button4.configure(state=DISABLED)
    button5.configure(state=DISABLED)
    button6.configure(state=DISABLED)
    button7.configure(state=DISABLED)
    button8.configure(state=DISABLED)
    button9.configure(state=DISABLED)



def btnClick(buttons):
    global bclick, flag, player2_name, player1_name, playerb, pa
    if buttons["text"] == " ":
        buttons["text"] = "X"
        # playerb = p2.get() + " Wins!"
        # pa = p1.get() + " Wins!"
        checkForWin()
        flag += 1

    else:
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "Button already Clicked!")










    # vertical
    if ((button1["text"] == "0") and (button2["text"] == "0") and (button3["text"] == " ")):
        button3["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == "0") and (button5["text"] == "0") and (button6["text"] == " ")):
        button6["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == "0") and (button8["text"] == "0") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1
        # 1
    elif ((button1["text"] == "0") and (button2["text"] == " ") and (button3["text"] == "0")):
        button2["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == "0") and (button5["text"] == " ") and (button6["text"] == "0")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == "0") and (button8["text"] == " ") and (button9["text"] == "0")):
        button8["text"] = "0"

        checkForWin()
        flag += 1
        # 2
    elif ((button1["text"] == " ") and (button2["text"] == "0") and (button3["text"] == "0")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == " ") and (button5["text"] == "0") and (button6["text"] == "0")):
        button4["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == " ") and (button8["text"] == "0") and (button9["text"] == "0")):
        button7["text"] = "0"

        checkForWin()
        flag += 1
        # 3

        # Horizontal
    elif ((button1["text"] == "0") and (button4["text"] == "0") and (button7["text"] == " ")):
        button7["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == "0") and (button5["text"] == "0") and (button8["text"] == " ")):
        button8["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "0") and (button6["text"] == "0") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1
        # 1
    elif ((button1["text"] == "0") and (button4["text"] == " ") and (button7["text"] == "0")):
        button4["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == "0") and (button5["text"] == " ") and (button8["text"] == "0")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "0") and (button6["text"] == " ") and (button9["text"] == "0")):
        button6["text"] = "0"

        checkForWin()
        flag += 1
        # 2
    elif ((button1["text"] == " ") and (button4["text"] == "0") and (button7["text"] == "0")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == " ") and (button5["text"] == "0") and (button8["text"] == "0")):
        button2["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == " ") and (button6["text"] == "0") and (button9["text"] == "0")):
        button3["text"] = "0"

        checkForWin()
        flag += 1
        # 3

        # C
    elif ((button1["text"] == "0") and (button5["text"] == "0") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "0") and (button5["text"] == "0") and (button7["text"] == " ")):
        button7["text"] = "0"

        checkForWin()
        flag += 1
    # 1

    elif ((button1["text"] == "0") and (button5["text"] == " ") and (button9["text"] == "0")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "0") and (button5["text"] == " ") and (button7["text"] == "0")):
        button5["text"] = "0"

        checkForWin()
        flag += 1
        # 2

    elif ((button1["text"] == " ") and (button5["text"] == "0") and (button9["text"] == "0")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == " ") and (button5["text"] == "0") and (button7["text"] == "0")):
        button3["text"] = "0"

        checkForWin()
        flag += 1
        # 3

        # X
        # vertical
    elif ((button1["text"] == "X") and (button2["text"] == "X") and (button3["text"] == " ")):
        button3["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == "X") and (button5["text"] == "X") and (button6["text"] == " ")):
        button6["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == "X") and (button8["text"] == "X") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1
        # 1
    elif ((button1["text"] == "X") and (button2["text"] == " ") and (button3["text"] == "X")):
        button2["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == "X") and (button5["text"] == " ") and (button6["text"] == "X")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == "X") and (button8["text"] == " ") and (button9["text"] == "X")):
        button8["text"] = "0"

        checkForWin()
        flag += 1
        # 2
    elif ((button1["text"] == " ") and (button2["text"] == "X") and (button3["text"] == "X")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button4["text"] == " ") and (button5["text"] == "X") and (button6["text"] == "X")):
        button4["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button7["text"] == " ") and (button8["text"] == "X") and (button9["text"] == "X")):
        button7["text"] = "0"

        checkForWin()
        flag += 1
        # 3

        # Horizontal
    elif ((button1["text"] == "X") and (button4["text"] == "X") and (button7["text"] == " ")):
        button7["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == "X") and (button5["text"] == "X") and (button8["text"] == " ")):
        button8["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "X") and (button6["text"] == "X") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1
        # 1
    elif ((button1["text"] == "X") and (button4["text"] == " ") and (button7["text"] == "X")):
        button4["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == "X") and (button5["text"] == " ") and (button8["text"] == "X")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "X") and (button6["text"] == " ") and (button9["text"] == "X")):
        button6["text"] = "0"

        checkForWin()
        flag += 1

        # 2
    elif ((button1["text"] == " ") and (button4["text"] == "X") and (button7["text"] == "X")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button2["text"] == " ") and (button5["text"] == "X") and (button8["text"] == "X")):
        button2["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == " ") and (button6["text"] == "X") and (button9["text"] == "X")):
        button3["text"] = "0"

        checkForWin()
        flag += 1
        # 3

        # C
    elif ((button1["text"] == "X") and (button5["text"] == "X") and (button9["text"] == " ")):
        button9["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "X") and (button5["text"] == "X") and (button7["text"] == " ")):
        button7["text"] = "0"

        checkForWin()
        flag += 1
    # 1

    elif ((button1["text"] == "X") and (button5["text"] == " ") and (button9["text"] == "X")):
        button5["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == "X") and (button5["text"] == " ") and (button7["text"] == "X")):
        button5["text"] = "0"

        checkForWin()
        flag += 1
        # 2

    elif ((button1["text"] == " ") and (button5["text"] == "X") and (button9["text"] == "X")):
        button1["text"] = "0"

        checkForWin()
        flag += 1

    elif ((button3["text"] == " ") and (button5["text"] == "X") and (button7["text"] == "X")):
        button3["text"] = "0"

        checkForWin()
        flag += 1
        # 3

    elif (button5["text"] == " "):
        button5["text"] = "0"
        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] == " "):
        button3["text"] = "0"

        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] == " "):
        button1["text"] = "0"

        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] == " "):
        button9["text"] = "0"

        checkForWin()
        flag += 1

    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] != " " and
          button7["text"] == " "):
        button7["text"] = "0"

        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] != " " and
          button7["text"] != " " and button2["text"] == " "):
        button2["text"] = "0"
        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] != " " and
          button7["text"] != " " and button2["text"] != " " and button8["text"] == " "):
        button8["text"] = "0"
        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] != " " and
          button7["text"] != " " and button2["text"] != " " and button8["text"] != " " and button4["text"] == " "):
        button4["text"] = "0"

        checkForWin()
        flag += 1
    elif (button5["text"] != " " and button3["text"] != " " and button1["text"] != " " and button9["text"] != " " and
          button7["text"] != " " and button2["text"] != " " and button8["text"] != " " and button4["text"] != " " and
          button6["text"] == " "):
        button6["text"] = "0"

        checkForWin()
        flag += 1
    else:
        checkForWin()


def checkForWin():
    if (button1['text'] == 'X' and button2['text'] == 'X' and button3['text'] == 'X'):
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")

    elif button4['text'] == 'X' and button5['text'] == 'X' and button6['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")
    elif button7['text'] == 'X' and button8['text'] == 'X' and button9['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")
    elif button1['text'] == 'X' and button5['text'] == 'X' and button9['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")
    elif button3['text'] == 'X' and button5['text'] == 'X' and button7['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")

    elif button1['text'] == 'X' and button4['text'] == 'X' and button7['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")
    elif  button2['text'] == 'X' and button5['text'] == 'X' and button8['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")
    elif button3['text'] == 'X' and button6['text'] == 'X' and button9['text'] == 'X':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "X wins")






        #0 WINS

    elif (button1['text'] == '0' and button2['text'] == '0' and button3['text'] == '0'):
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")

    elif button4['text'] == '0' and button5['text'] == '0' and button6['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    elif button7['text'] == '0' and button8['text'] == '0' and button9['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    elif button1['text'] == '0' and button5['text'] == '0' and button9['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    elif button3['text'] == '0' and button5['text'] == '0' and button7['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")

    elif button1['text'] == '0' and button4['text'] == '0' and button7['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    elif button2['text'] == '0' and button5['text'] == '0' and button8['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    elif button7['text'] == '0' and button6['text'] == '0' and button9['text'] == '0':
        disableButton()
        tkinter.messagebox.showinfo("Tic-Tac-Toe", "0 wins")
    # elif(flag == 8):
    #     tkinter.messagebox.showinfo("Tic-Tac-Toe", "It is a Tie")

    elif button1['text'] != ' ' and button2['text'] != ' ' and button3['text'] != ' ' and button4['text'] != ' ' and button5['text'] != ' ' and button6['text'] != ' ' and button7['text'] != ' ' and button6['text'] != ' ' and button9['text'] != ' ':

        tkinter.messagebox.showinfo("Tic-Tac-Toe", "It is a Tie")

buttons = StringVar()

# label = Label( tk, text="Player 1:", font='Times 20 bold', bg='white', fg='black', height=1, width=8)
# label.grid(row=1, column=0)
#
#
# label = Label( tk, text="Player 2:", font='Times 20 bold', bg='white', fg='black', height=1, width=8)
# label.grid(row=2, column=0)

button1 = Button(tk, text=" ", font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button1))
button1.grid(row=3, column=0)

button2 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button2))
button2.grid(row=3, column=1)

button3 = Button(tk, text=' ',font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button3))
button3.grid(row=3, column=2)

button4 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button4))
button4.grid(row=4, column=0)

button5 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button5))
button5.grid(row=4, column=1)

button6 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button6))
button6.grid(row=4, column=2)

button7 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button7))
button7.grid(row=5, column=0)

button8 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button8))
button8.grid(row=5, column=1)

button9 = Button(tk, text=' ', font='Times 20 bold', bg='gray', fg='white', height=4, width=8, command=lambda: btnClick(button9))
button9.grid(row=5, column=2)

tk.mainloop()