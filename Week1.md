🐍 Week 1: Python Foundations (July 16-22, 2025)
------------------------------------------------

### 📌 Daily Tasks Breakdown

### Day 1: Setup & Basics (Wed, July 16):
• Install Python 3.12 + VS Code
• Learn variables/IO
• Build user profile script
```python
# user_profile.py
name = input("Your name: ")
age = int(input("Your age: "))
print(f"Hello {name}! You'll be {age+5} in 5 years.")
```
### Day 2: Control Flow (Thu, July 17):
• Master conditionals
• Build weather adviser
• Add error handling
```python
# weather_adviser.py
temp = float(input("Current temperature (°C): "))
if temp > 35:
    print("🔥 Extreme heat warning!")
elif 25 <= temp <= 35:
    print("😎 Perfect beach weather!")
else:
    print("🧥 Bring a jacket.")
```
### Day 3: Loops (Fri, July 18):
• Create multiplication trainer
• Implement range()
• Add input validation
```python
# multiplication_trainer.py
while True:
    try:
        num = int(input("Learn table of: "))
        break
    except ValueError:
        print("Please enter a valid integer!")

for i in range(1, 11):
    print(f"{num} × {i} = {num*i}")
```
### Day 4: Functions (Sat, July 19):
• Define reusable functions
• Build geometry helper
• Add docstrings
```python
# geometry_helper.py
def circle_area(radius: float) -> float:
    return 3.14159 * radius ** 2

def triangle_area(base: float, height: float) -> float:
    return 0.5 * base * height

print(f"Circle area: {circle_area(5):.2f} cm²")
```
### Day 5: Data Structures (Sun, July 20):
• Create contact manager
• Use lists/dicts
• Implement CRUD ops
```python
# contact_manager.py
contacts = []

def add_contact():
    name = input("Name: ")
    phone = input("Phone: ")
    contacts.append({"name": name, "phone": phone})
    print(f"✅ {name} added!")

add_contact()
```
### Day 6: File I/O (Mon, July 21):
• Build journal app
• Read/write files
• Use context managers
```python
# journal_app.py
import os

entry = input("Today's journal entry: ")

if not os.path.exists("journal.txt"):
    open("journal.txt", "w").close()

with open("journal.txt", "a") as f:
    f.write(f"{entry}\n")
print("📝 Entry saved!")
```
### Day 7: Project (Tue, July 22):
• Create text adventure game
• Implement health system
• Add save/load feature
```python
# adventure_game.py
health = 100
inventory = []

print("🌲 You wake in a forest. Paths: [1] Cave [2] River")
choice = input("Choose: ")

if choice == "1":
    print("🕳️ Dark cave... torch? [y/n]")
    if input() == "y":
        print("🔦 You see treasure! +50 gold")
        inventory.append("gold")
    else:
        print("😱 Bats attack! -20 health")
        health -= 20
```
### Repository Structure
```text
/python-foundations
├── .gitignore
├── README.md
├── requirements.txt  # python>=3.12
├── day1_user_profile.py
├── day2_weather_adviser.py
├── day3_multiplication_trainer.py
├── day4_geometry_helper.py
├── day5_contact_manager.py
├── day6_journal_app.py
└── day7_adventure_game.py
```

