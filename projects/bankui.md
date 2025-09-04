---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Bank UI"
date: 2025 - 04 - 26
published: true
labels:
  - C
  - C++
  - Unix
summary: "This was my project for ICS 212."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

The purpose of this ICS 212 project was to demonstrate our ability to write code in both C and C++ also coding in unix, including the use of g++ and makefiles. This project spanned the entire course, building upon the previous homework assignments. Initially, we implemented the Bank UI to handle credit card numbers, including functionalities to save, search, print all, and delete records. Later, we converted the program from C to C++, maintaining all previous functionalities. Additionally, the C++ version introduces the use of pointers for data handling and a debug mode menu for easier testing and verification.


Here is some code that illustrates how we read values from the line sensors:

```cpp
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse News Announcement](https://manoa.hawaii.edu/news/article.php?aId=2857).
