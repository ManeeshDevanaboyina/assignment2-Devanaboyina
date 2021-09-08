# assignment2-Devanaboyina
Second assignment
I live in maryville
# Maneesh Devanaboyina
###### Paris
Paris is unlike any other location on Earth, **its beauty is unparalleled, the number of famous structures is incredible**, and its allure attracts a large number of people each year. It seemed impossible that such simple structures could have so much charm. **The Eiffel Tower is the most significant reason why I like Paris**.

*** 

## Directions from Maryville to Paris

1. One way from Maryville to Paris.
    1. Maryville to Kansas City by bus.
    2. Five Minutes walk to East Village - Bay A from Kansas city bus stop.
    3. 48 minutes bus from East Village - Bay A to Kci Airport Terminal B.
    4. From Kansas Airport there is a direct flight to Paris.
2. Alternative way from Maryville to Paris.
    1. Night bus from Maryville to Omaha by Bus.
    2. 15 minutes bus from Omaha busstop to  Eppley Airfield(Omaha Airport)
    3. From Omaha Airport there is a direct flight to Paris.

* Clothes
* Food
* Gaming console
* Laptop

![Image of a vintage car](IMG_0741.jpg)



[Link to AboutMe](https://github.com/ManeeshDevanaboyina/assignment2-Devanaboyina/blob/967c6fa3c853fa52845ef7912fef7c402a077c86/AboutMe.md)

***

## Some of my favourite foods and Drinks

Creating a table that shows food items & Drinks that I recommend someone to try which also includes Location and cost of that item.

| Items | Location | Cost |
| :---: | :---: | :---: |
| Croissants | Paris | 10$ |
| Macarons | Ladurée | 5$ |
| French Cheese | Alsena | 3$ |
| Gini | Suntury | 5$ | 

***

## My Inspirational Quotes

> Your time is limited, so don't waste it living someone else's life. Don't be trapped by dogma – which is living with the results of other people's thinking. -*Steve Jobs*

> If life were predictable it would cease to be life, and be without flavor. -*Eleanor Roosevelt*

***
## Code Fencing

> Combinatorics is an area of mathematics primarily concerned with counting, both as a means and an end in obtaining results, and certain properties of finite structures. It is closely related to many other areas of mathematics and has many applications ranging from logic to statistical physics, from evolutionary biology to computer science.

[Combinatorics](https://en.wikipedia.org/wiki/Combinatorics)

    int solve (int n, int r) {  
        vector<int> p;  
        for (int i=2; i*i<=n; ++i)  
            if (n % i == 0) {  
                p.push_back (i);  
                while (n % i == 0)  
                    n /= i;  
            }  
        if (n > 1)  
            p.push_back (n);  

        int sum = 0;  
        for (int msk=1; msk<(1<<p.size()); ++msk) {  
            int mult = 1,  
                bits = 0;  
            for (int i=0; i<(int)p.size(); ++i)  
                if (msk & (1<<i)) {  
                    ++bits;  
                    mult *= p[i];  
                }  

            int cur = r / mult;  
            if (bits % 2 == 1)  
                sum += cur;  
            else  
                sum -= cur;  
        }  

        return r - sum;  
    }  


[Code Source](https://cp-algorithms.com/combinatorics/inclusion-exclusion.html)