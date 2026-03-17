# Course-Recommendations
Gives course recommendations to students based on grade, preference, and skill level.
math = "math"
advanced_math = "Algebra 2"
intermediate_math = "Pre-Algebra"
beginner_math = "Geometry"

ela = "ela"
advanced_ela = "US History"
intermediate_ela = "Constitution 101"
beginner_ela = "Revolutionary War"

science = "science"
beg_science = "Forces and Motion"
inter_science = "Biology"
adv_science = "Physics"

art = "Art History"
tech = "Intro to Coding"
space = "Space Science"
life_skills = "Finance"

print("No caps please.")

grade = int(input("What grade are you in? "))
    
favorite_subject = input("What is your favorite subject? ")

level = input("Are you a beginner, intermediate, or advanced learner?: ")

rec = ""
if grade > 6:
    if favorite_subject == math:
        if level == "beginner":
            rec = beginner_math
        elif level == "intermediate":
            rec = intermediate_math
        else:
            rec = advanced_math
    elif favorite_subject == ela:
        if level == "beginner":
            rec = beginner_ela
        elif level == "intermediate":
            rec = intermediate_ela
        else:
            rec = advanced_ela
    elif favorite_subject == science:
        if level == "beginner":
            rec = beg_science
        elif level == "intermediate":
            rec = inter_science
        else:
            rec = adv_science

if grade < 6:
    if favorite_subject == art:
        rec = art
    elif favorite_subject == tech:
        rec = tech
    elif favorite_subject == space:
        rec = space
    else:
        rec = life_skills

print("We recommend this course: " + rec)

