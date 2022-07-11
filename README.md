# BMI-Ver-2

# Write a program that interprets the Body Mass Index (BMI) based on a user's weight and height.
It should tell them the interpretation of their BMI based on the BMI value.
Under 18.5 they are underweight
Over 18.5 but below 25 they have a normal weight
Over 25 but below 30 they are slightly overweight
Over 30 but below 35 they are obese
Above 35 they are clinically obese.

# BMI = weight / height**2

# 🚨 Don't change the code below 👇
height = float(input("enter your height in m: "))
weight = float(input("enter your weight in kg: "))
# 🚨 Don't change the code above 👆

#Write your code below this line 👇

BMI = weight / height**2

round_bmi = round((BMI))

if BMI < 18.5:
    result = "underweight"
    print(f"Your BMI is {round_bmi}, you are {result}.")
elif  BMI > 18.5 and BMI < 25:
    result = "normal weight"
    print(f"Your BMI is {round_bmi}, you have a {result}.")
elif BMI > 25 and BMI < 30:
    result = "slightly overweight"
    print(f"Your BMI is {round_bmi}, you are {result}.")
elif BMI > 30 and BMI < 35:
    result = "obese"
    print(f"Your BMI is {round_bmi}, you are {result}.")
else:
    result = "clinically obese"
    print(f"Your BMI is {round_bmi}, you are {result}.")

