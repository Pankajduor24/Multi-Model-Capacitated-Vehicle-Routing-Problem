# Capacitated-Vehicle-Routing-Problem

Many of us have been regularly ordering from Swiggy InstaMart (IM) and are pretty happy with the delivery experience from both scheduled & instant delivery. Have you ever wondered how Swiggy InstaMart (IM) fulfils your order by selecting the right Delivery Executive (DE) for your order? Or how is a trip (aka route or batch) decided for a given DE (i.e. if Mr. Bhim's order should be delivered first or Mr. Abhi’s)?
Consider, if Bhim and Abhi both ordered from the same IM store and only 1 DE is available, then we can fulfil their orders in the following combinations:

### • 𝐷𝐸 → 𝑆𝑡𝑜𝑟𝑒 → Bhim → Abhi
### • 𝐷𝐸 → 𝑆𝑡𝑜𝑟𝑒 → Abhi → Bhim
### • 𝐷𝐸 → 𝑆𝑡𝑜𝑟𝑒 → Bhim → 𝑆𝑡𝑜𝑟𝑒 → Abhi
### • 𝐷𝐸 → 𝑆𝑡𝑜𝑟𝑒 → Abhi → 𝑆𝑡𝑜𝑟𝑒 → Bhim

Now, imagine if you have just 100 DEs, then these combinations will be replicated for all DEs (besides combinations where each order can be delivered by separate DEs). Further, we also have multiple IM fulfilment stores. Even for a handful of orders and DEs, it becomes a daunting task to devise such plans within a short time manually. Imagine if you have to solve for more than 200K+ Orders with 150K+ DEs and 100+ IM stores every day. We definitely need an algorithm to automate this process, right?

The VRP is classified as an NP-hard problem. Hence, the use of exact optimization methods may be difficult to solve these problems in acceptable CPU times, when the problem involves real-world data sets that are very large. The vehicle routing problem comes under combinatorial problem. Hence, to get solutions in determining routes which are realistic and very close to the optimal solution, we use heuristics and meta-heuristics. Here, we will discuss the exact method and the heuristics and meta-heuristics used to solve the VRP and its variants.

We will be using ORTOOLS (developed by Google) library in Python to solve the Vehicle Routing Problem for Supply Chain Operations at 
***TVS SCS Limited***. 

There are two type of routings has to be done i.e., Incity and Upcountry. Kindly refer to the project report for more info.
