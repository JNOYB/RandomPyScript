````
import tkinter as tk

def calculate_total():
    # Get the input numbers and sum them up
    numbers = entry.get().split()
    numbers = [int(num) for num in numbers]
    total = sum(numbers)
    
    # Update the output label with the total
    output.config(text="The sum of the numbers is: {}".format(total))

# Create the main window and widgets
window = tk.Tk()
window.title("Number Summation")

label = tk.Label(window, text="Enter numbers separated by spaces:")
label.pack()

entry = tk.Entry(window)
entry.pack()

button = tk.Button(window, text="Calculate", command=calculate_total)
button.pack()

output = tk.Label(window, text="")
output.pack()

# Start the event loop
window.mainloop()

````
