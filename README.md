# assignment2-chintala

# Harika Chintala

---
###### Araku Valley

**Araku Valley** is a hill station and valley region in the southeastern Indian state of *Andhra Pradesh*. It's surrounded by the thick forests of the Eastern Ghats mountain range. The **Tribal Museum** is dedicated to the area's numerous indigenous tribes, known for their traditional **Dhimsa dance**, and showcases traditional handicrafts. A miniature train runs through Padmapuram Gardens, with its sculptures and tree-top huts.

I like it because as it is a hill station there are clouds where we can feel to touch and the  location is completely eye catchy.

---
# How to Travel?

***Well!! here are the Directions.***

1. Maryville - Kansas Airport    
2. Kansas Airport - Chennai Airport
3. Chennai Airport - Chennai Railway Station
    1. Alandur
    2. Nagapattinam
4. Chennai Railway Station - Araku
    1. Nellore
    2. Borra Guhalu

# What to carry?

***includes for men, women and kids***

* Shorts and short pants
* Long and Short Sleeve Shirts
* Suncreen Lotion
    * SPF 50
* Bug repellent
* Sandals
    * Men
    * Women
    * Kids
---
**[Click for AboutMe Link](AboutMe.md)**

---
# JustTry It!

***Foods/Drinks*** 


Here are the Foods/Drinks that I would recommend to try.

| Foods/Drinks | Location | Price(Rupees) |
| ------ | ------ | ------ |
| Sambar rice | Hderabad | 100 |
| French Omlet | Hyderabad | 150 |
| Oreo Milkshake | Maryville | 400 |
| Biryani | Hyderabad | 100 |

---
# Quotes

> “Be who you are and say what you feel, because those who mind don't matter and those who matter don't mind.” ... *Swamy Vivekananda*

> “The best way to predict the future is to invent it.” ... *Nelson Mandela*

---
# String Hashing

**Hashing algorithms** are helpful in solving a lot of problems.

We want to solve the problem of comparing strings efficiently. The brute force way of doing so is just to compare the letters of both strings, which has a time complexity of O(min(n1,n2)) if n1 and n2 are the sizes of the two strings. We want to do better. The idea behind strings is the following: we convert each string into an integer and compare those instead of the strings. Comparing two strings is then an O(1) operation. For the conversion, we need a so-called **hash function**.

```
long long compute_hash(string const& s) {
    const int p = 31;
    const int m = 1e9 + 9;
    long long hash_value = 0;
    long long p_pow = 1;
    for (char c : s) {
        hash_value = (hash_value + (c - 'a' + 1) * p_pow) % m;
        p_pow = (p_pow * p) % m;
    }
    return hash_value;
}

```

[Here is the link to know more about String Hashing](https://cp-algorithms.com/string/string-hashing.html) 



