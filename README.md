# OIBSIP_pythonprogramming_1
This is a beginner-level Python project that calculates Body Mass Index (BMI) using user-provided height and weight.  It includes input validation and categorizes BMI into standard health ranges.  The project demonstrates fundamental Python concepts such as user interaction, conditionals, and basic logic building.
print("BMI Calculator")

weight = float(input("Enter your weight in kg: "))
height = float(input("Enter your height in meters: "))

if weight <= 0 or height <= 0:
    print("Invalid input! Please enter positive numbers.")
else:
    bmi = weight / (height * height)
    bmi = round(bmi, 2)

    print("Your BMI is:", bmi)

    if bmi < 18.5:
        print("Category: Underweight")
    elif bmi < 25:
        print("Category: Normal weight")
    elif bmi < 30:
        print("Category: Overweight")
    else:
        print("Category: Obese")
