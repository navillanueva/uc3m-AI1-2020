# Markov Decision Model

Final project for artificial intelligence 1 course at Universidad Carlos 3 de Madrid in May 2020. Programmed in python.

In this class project we were handed a raw data file (.csv) that contained data of the road intersection. The road intersection we were working with was the following:

![map layout](https://user-images.githubusercontent.com/42673884/183933895-bbd56b1b-9c55-4efd-8f52-9abc6183b39a.png)

And the data in the .csv file was like this:

```
High;High;Low;E;High;High;Low
```
Where the first 3 values correspond to the traffic level in the lanes (West, East, North) in that order. Then the letter in the middle represents the traffic light that turned green (in the example its the traffic light of the East oriented lane) and the last 3 values represent the updated state of the traffic level in the lanes after applying that green light.

The first part of the code is mainly in charge of extracting and organizing the data to be able to get the probabilities of what happened when we applied an operator (letter in the middle // traffic light that turns green) to each initial state (first 3 values).

Once we had these probabilities we could build our markov decision model to create an algorithm that would know what operators to chose to achieve a low traffic level in all of the lanes.

