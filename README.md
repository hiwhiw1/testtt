def get_int(prompt):
    while True:
        try:
            return int(input(prompt))
        except ValueError:
            print("กรุณาใส่ตัวเลข (Please enter a valid integer).")

name = input("Enter your name: ")
score = get_int("Enter your score: ")

result = "ผ่าน" if score > 50 else "ไม่ผ่าน"
print(f"สวัสดีครับ {name}! คะแนนของคุณคือ {score}")
print(f"ผลการเรียน: {result}")
