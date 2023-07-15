# Puzzles
Puzzles asked in the interviews..


1) Three ants are sitting at the three corners of an equilateral triangle. Each ant starts randomly picks a direction and starts to move along the edge of the triangle. What is the probability that none of the ants collide?
- So let’s think this through. The ants can only avoid a collision if they all decide to move in the same direction (either clockwise or anti-clockwise). If the ants do not pick the same direction, there will definitely be a collision. Each ant has the option to either move clockwise or anti-clockwise. There is a one in two chance that an ant decides to pick a particular direction. Using simple probability calculations, we can determine the probability of no collision.
P(No collision) = P(All ants go in a clockwise direction) + P( All ants go in an anti-clockwise direction) = 0.5 * 0.5 * 0.5 + 0.5 * 0.5 * 0.5 = 0.25

=================
2) Four people need to cross a rickety bridge at night. Unfortunately, they have only one torch and the bridge is too dangerous to cross without one. The bridge is only strong enough to support two people at a time. Not all people take the same time to cross the bridge. Times for each person: 1 min, 2 mins, 7 mins and 10 mins. What is the shortest time needed for all four of them to cross the bridge?
- It is 17 mins. 1 and 2 go first, then 1 comes back. Then 7 and 10 go and 2 comes back. Then 1 and 2 go again, it makes a total of 17 minutes.

=================
3) A man has two ropes of varying thickness (Those two ropes are not identical, they aren’t the same density nor the same length nor the same width). Each rope burns in 60 minutes. He actually wants to measure 45 mins. How can he measure 45 mins using only these two ropes.
He can’t cut the one rope in half because the ropes are non-homogeneous and he can’t be sure how long it will burn.
- He will burn one of the rope at both the ends and the second rope at one end. After half an hour, the first one burns completely and at this point of time, he will burn the other end of the second rope so now it will take 15 mins more to completely burn. so total time is 30+15 i.e. 45mins.

=================
4) You are standing before two doors. One of the path leads to heaven and the other one leads to hell. There are two guardians, one by each door. You know one of them always tells the truth and the other always lies, but you don’t know who is the honest one and who is the liar.
You can only ask one question to one of them in order to find the way to heaven. What is the question?
- The question you should ask is “If I ask the other guard about which side leads to heaven, what would he answer?”. It should be fairly easy to see that irrespective of whom do you ask this question, you will always get an answer which leads to hell. So you can chose the other path to continue your journey to heaven.
This idea was famously used in the 1986 film Labyrinth. Here is the explanation if it is yet not clear. Let us assume that the left door leads to heaven.
If you ask the guard which speaks truth about which path leads to heaven, as he speaks always the truth, he would say “left”. Now that the liar , when he is asked what “the other guard (truth teller) ” would answer, he would definitely say “right”. Similarly, if you ask the liar about which path leads to heaven, he would say “right”. As the truth teller speaks nothing but the truth, he would say “right” when he is asked what “the other guard( liar ) ” would answer. So in any case, you would end up having the path to hell as an answer. So you can chose the other path as a way to heaven

=================
5) You are blindfolded and 10 coins are place in front of you on table. You are allowed to touch the coins, but can’t tell which way up they are by feel. You are told that there are 5 coins head up, and 5 coins tails up but not which ones are which. How do you make two piles of coins each with the same number of heads up? You can flip the coins any number of times.
- Make 2 piles with equal number of coins. Now, flip all the coins in one of the pile.

=================
6) A bad king has a cellar of 1000 bottles of delightful and very expensive wine. A neighboring queen plots to kill the bad king and sends a servant to poison the wine. Fortunately (or say unfortunately) the bad king’s guards catch the servant after he has only poisoned one bottle. Alas, the guards don’t know which bottle but know that the poison is so strong that even if diluted 100,000 times it would still kill the king. Furthermore, it takes one month to have an effect. The bad king decides he will get some of the prisoners in his vast dungeons to drink the wine. Being a clever bad king he knows he needs to murder no more than 10 prisoners – believing he can fob off such a low death rate – and will still be able to drink the rest of the wine (999 bottles) at his anniversary party in 5 weeks time. Explain what is in mind of the king, how will he be able to do so ? (of course he has less then 1000 prisoners in his prisons)
- Think in terms of binary numbers. Number the bottles 1 to 1000 and write the number in binary format.
bottle 1 = 0000000001 (10 digit binary)
bottle 2 = 0000000010
bottle 500 = 011111010
bottle 1000 = 1111101000
Now take 10 prisoners and number them 1 to 10, now let prisoner 1 take a sip from every bottle that has a 1 in its least significant bit. Let prisoner 10 take a sip from every bottle with a 1 in its most significant bit. etc.
prisoner = 10 9 8 7 6 5 4 3 2 1
bottle 924 = 1 1 1 0 0 1 1 1 0 0
For instance, bottle no. 924 would be sipped by 10,9,8,5,4 and 3. That way if bottle no. 924 was the poisoned one, only those prisoners would die.
After four weeks, line the prisoners up in their bit order and read each living prisoner as a 0 bit and each dead prisoner as a 1 bit. The number that you get is the bottle of wine that was poisoned. 1000 is less than 1024 (2^10). If there were 1024 or more bottles of wine it would take more than 10 prisoners.

================
7) You have 3 jars that are all mislabeled. One jar contains Apple, another contains Oranges and the third jar contains a mixture of both Apple and Oranges. You are allowed to pick as many fruits as you want from each jar to fix the labels on the jars. What is the minimum number of fruits that you have to pick and from which jars to correctly label them?
Labels on jars are as follows:
1) Apple 2) Orange 3) Apple and Orange
- Let’s take a scenario. Suppose you pick from jar labelled as Apple and Oranges and you got Apple from it. That means that jar should be Apple as it is incorrectly labelled. So it has to be Apple jar. Now the jar labelled Oranges has to be Mixed as it cannot be the Oranges jar as they are wrongly labelled and the jar labelled Apple has to be Oranges. Similar scenario applies if it’s a Oranges taken out from the jar labelled as Apple and Oranges. So you need to pick just one fruit from the jar labelled as Apple and Oranges to correctly label the jars.

================
8) You have 100 doors in a row that are all initially closed. you make 100 passes by the doors starting with the first door every time. the first time through you visit every door and toggle the door (if the door is closed, you open it, if its open, you close it). the second time you only visit every 2nd door (door #2, #4, #6). the third time, every 3rd door (door #3, #6, #9), ec, until you only visit the 100th door.
What state are the doors in after the last pass? Which are open which are closed?
- You can figure out that for any given door, say door #38, you will visit it for every divisor it has. so  has 1 & 38, 2 & 19. so on pass 1 i will open the door, pass 2 i will close it, pass 19 open, pass 38 close. For every pair of divisors the door will just end up back in its initial state. so you might think that every door will end up closed? well what about door #9. 9 has the divisors 1 & 9, 3 & 3. but 3 is repeated because 9 is a perfect square, so you will only visit door #9, on pass 1, 3, and 9… leaving it open at the end. only perfect square doors will be open at the end.

===============
9) You have two jars, 50 red marbles and 50 blue marbles. You need to place all the marbles into the jars such that when you blindly pick one marble out of one jar, you maximize the chances that it will be red. When picking, you’ll first randomly pick a jar, and then randomly pick a marble out of that jar. You can arrange the marbles however you like, but each marble must be in a jar.
-Say we put all the red marbles into JAR A and all the blue ones into JAR B. then our chances for picking a red one are:
1/2 chance we pick JAR A * 50/50 chance we pick a red marble
1/2 chance we pick JAR B * 0/50 chance we pick a red marble
You would try different combinations, such as 25 of each colored marble in a jar or putting all red marbles in one jar and all the blue in the other. You would still end up with a chance of 50%. What if you put a single red marble in one jar and the rest of the marbles in the other jar? This way, you are guaranteed at least a 50% chance of getting a red marble (since one marble picked at random, doesn’t leave any room for choice). Now that you have 49 red marbles left in the other jar, you have a nearly even chance of picking a red marble (49 out of 99).
So the maximum probability will be :
jar A : (1/2)*1 = 1/2 (selecting the jar A = 1/2, red marble from jar A = 1/1)
jar B : (1/2)*(49/99) = 0 (selecting the jar B = 1/2, red marble from jar B = 49/99)
Total probability = 74/99 (~3/4)

================
10) ADOBE interview question: Let there be 9 balls. In 9 balls there is a faulty ball(you don't know if it is heavy or not). You can use 3 times the balnce to find out the faulty ball. How?
- Make 3 pairs of 3 balls. When two pairs are balanced then 3rd pair must have faulty. So in 2 times we can find the faulty ball in a pair.  Now, if the two pairs are not balanced, then take another combination of pairs. You will get to know the group of 3 balls which has the faulty ball and also you will get to know if the ball is heavy or light. Now, if you know the faulty ball is heavy or light, you can take 1 chance to get to know the faulty ball in the group of 3 balls.

================
11) You’ve got someone working for you for seven days and a gold bar to pay him. The gold bar is segmented into seven connected pieces. You must give them a piece of gold at the end of every day. What and where are the fewest number of cuts to the bar of gold that will allow you to pay him 1/7th each day?
- Its only 2 cuts, baiscally 3 pieces of length: 1, 2, 4.

================
12) You have 10 bags full of coins. In each bag are infinite coins. But one bag is full of forgeries, and you can’t remember which one. But you do know that a genuine coins weigh 1 gram, but forgeries weigh 1.1 grams. You have to identify that bag in minimum readings. You are provided with a digital weighing machine.
- Take 1 coin from the first bag, 2 coins from the second bag, 3 coins from the third bag and so on. Eventually, we’ll get 55 (1+2+3…+9+10) coins. Now, weigh all the 55 coins together. Depending on the resulting weighing machine reading, you can find which bag has the forged coins such that if the reading ends with 0.4 then it is the 4th bag, if it ends with 0.7 then it is the 7th bag and so on.

================
13) There are 100 prisoners all sentenced to death. One night before the execution, the warden gives them a chance to live if they all work on a strategy together. The execution scenario is as follows – On the day of execution, all the prisoners will be made to stand in a straight line such that one prisoner stands just behind another and so on. All prisoners will be wearing a hat either of Blue colour or Red. The prisoners don’t know what colour of hat they are wearing. The prisoner who is standing at the last can see all the prisoners in front of him (and what colour of hat they are wearing). A prisoner can see all the hats in front of him. The prisoner who is standing in the front of the line cannot see anything. The executioner will ask each prisoner what colour of hat they are wearing one by one, starting from the last in the line. The prisoner can only speak “Red” or “Blue”. He cannot say anything else. If he gets it right, he lives otherwise he is shot instantly. All the prisoners standing in front of him can hear the answers and gunshots. Assuming that the prisoners are intelligent and would stick to the plan, what strategy would the prisoners make over the night to minimize the number of deaths?
- The strategy is that the last person will say ‘red’ if the number of red hats in front of him are odd and ‘blue’ if the number of red hats in front of him are even. Now, the 99th guy will see the if the red hats in front of him are odd or even. If it is odd then obviously the hat above him is blue, else it is red. From now on, it’s pretty intuitive.

================
14) You are in a dark room where a table is kept. There are 50 coins placed on the table, out of which 10 coins are showing tails and 40 coins are showing heads. The task is to divide this set of 50 coins into 2 groups (not necessarily same size) such that both groups have same number of coins showing the tails.
- Divide the group into two groups of 40 coins and 10 coins. Flip all coins of the group with 10 coins.

================
15) You have two sand timers, which can show 4 minutes and 7 minutes respectively. Use both the sand timers(at a time or one after other or any other combination) and measure a time of 9 minutes.
-Start the 7 minute sand timer and the 4 minute sand timer.
Once the 4 minute sand timer ends turn it upside down instantly.
Once the 7 minute sand timer ends turn it upside down instantly.
After the 4 minute sand timer ends turn the 7 minute sand timer upside down(it has now minute of sand in it)
So effectively 8 + 1 = 9.

=======
16) There is a bus with 100 labeled seats (labeled from 1 to 100). There are 100 persons standing in a queue. Persons are also labelled from 1 to 100. People board on the bus in sequence from 1 to n. The rule is, if person ‘i’ boards the bus, he checks if seat ‘i’ is empty. If it is empty, he sits there, else he randomly picks an empty seat and sit there. Given that 1st person picks seat randomly, find the probability that 100th person sits on his place i.e. 100th seat.
- The final answer is the probability that the last person ends in up in his proper seat is exactly 1/2. The reasoning goes as follows: First, observe that the fate of the last person is determined the moment either the first or the last seat is selected! This is because the last person will either get the first seat or the last seat. Any other seat will necessarily be taken by the time the last guy gets to ‘choose’. Since at each choice step, the first or last is equally probable to be taken, the last person will get either the first or last with equal probability: 1/2.

========
17) N persons are standing in a circle. They are labelled from 1 to N in clockwise order. Every one of them is holding a gun and can shoot a person on his left. Starting from person 1, they starts shooting in order e.g for N=100, person 1 shoots person 2, then person 3 shoots person 4, then person 5 shoots person 6……..then person 99 shoots person 100, then person 1 shoots person 3, then person 5 shoots person 7……and it continues till all are dead except one. What’s the index of that last person ?
- Write 100 in binary, which is 1100100 and take the complement which is 11011 and it is 27. Subtract the complement from the original number. So 100 – 27 = 73. Try it out for 50 people. 50 = 110010 in binary. Complement is 1101 = 13. Therefore, 50 – 13 = 37. For the number in form 2^n, it will be the first person. Let’s take an example: 64 = 1000000. Complement = 111111 = 63. 64-63 = 1. You can apply this for any ’n’.

=======
You have 4 bottles of milk. One of them is poisonous while the other 3 are non-poisonous. There is a rat which dies exactly after 10 hours of drinking the poisoned bottle. You have a clock that measures time only in hours. Suggest an optimal strategy to identify the poisoned bottle within 24 hours.
- Make the mouse drink from each bottle after 1 hour. Will get to know in 12 hours.

=======
There are 6 persons seating on a round table in which two individual have the same names. What is the probability that the two same-named individuals will be neighbors
- Total no of ways in which 6 persons can sit on a round table is (6-1)! = 5! = 120. If we consider two same-named individuals as one person there are 5 persons who can sit in (5-1)! ways and these individuals can be seated together in 2! ways. So, required probability =(2*(5-1)!)/(6-1)!= 2/5. So, the answer is 2/5 = 0.4.

=======
A Geek is about to get a plane to Hyderabad. Geek wants to know if it’s raining. Geek calls 3 random friends staying at Hyderabad to ask this question. Each friend has a 2/3 chance of telling the truth and 1/3 chance of lying. All the three friends gave the response as “Yes, it is Raining. What is the probability that it’s actually raining in Hyderabad? 
- The Geek only requires one of the friends to be telling the truth. The probability that at least one of them is telling the truth will be: 1 - (Probability that all of them Lied). The probability that all of them lied is 1/27. i.e. 1/3 * 1/3 * 1/3. So, now the probability that at least one of them told the truth is: 1 – (1/27) = 26/27.

=======
There are 10 robbers named as’A’, ‘B’, ‘C’, ‘D’, ‘E’, ‘F’, ‘G’, ‘H’, ‘I’, ‘J’ they stole some coins from a bank and they decided to divide these coins equally among themselves. So they divide the coins into 10 parts but the last robber ‘J’ got 1 coin less than other robbers. So the remaining 9 robbers murder ‘J’. They again decided to divide the coins into 9 parts. But this time again the last robber ‘I’ got 1 less coin than other robbers. So again the remaining 8 robbers murder ‘I’ and try to divide all coins in between remaining 8 robbers. But again this time ‘H’ got one less coin than the other. Now, this process goes on until 1 robber left i.e. is ‘A’. After that ‘A’ take all the coins and run away. Now you have to guess the total number of coins.
- In a first attempt if there was 1 more coin then the coins could be easily divided among 10 robbers. And in the second attempt also the coins could be equally divided in among 9 robbers and so on. So let just add one coin to the total number of the coin. So the total coins become N+1. now this (N+1) should be divisible by 10. It should be divisible by 9, 8, 7, 6, 5, 4, 3, 2, 1. So our answer should be LCM of (10, 9, 8, 7, 6, 5, 4, 3, 2, 1). Total Number of coins = LCM of (10, 9, 8, 7, 6, 5, 4, 3, 2, 1) which is 2520.

======
Ishita has 10 bags full of coins. Each bag contains 1000 coins. But one bag is full of forgeries, and she just can’t recall which one. She does know that genuine coins weigh 1 gram, but forgeries weigh 1.1 grams. To hide the fact that she can’t recall which bag contains forgeries, she needs your help. How can she identify the bag with the forgeries with just one weighing? 
- It is known that there is only one bag with forgeries. To identify that bag, Ishita can follow a simple procedure. She should take out 1 coin from the 1st bag, 2 coins from the 2nd bag, 3 coins from the 3rd bag and similarly 10 coins from the 10th bag.

======
On an Island, there is an airport that has an unlimited number of identical air-planes. Each air-plane has a fuel capacity to allow it to fly exactly 1/2 way around the world, along a great circle. The planes have the ability to refuel in flight without loss of speed or spillage of fuel. Though the fuel is unlimited, the island is the only source of fuel. You can ignore the time and fuel consumption of refuelling. What is the minimum number of air-planes required to get one air plane all the way around the world assuming that all of the air planes must return safely to the airport?
- The idea is to take hold some planes in the middle, send some planes back and get the fuel to get the main plane fueled again. Let the three air plane be X, Y and Z. Let total circumference be 300 Units. So every plane can run 150 units. Let X be the plane that will go around the world. After 1/6th of the circumference (50 units), Y passes 1/3rd of its fuel to Z and returns (Y has fuel left to travel exactly 50 units). Now Z has fuel left for 150 units (Completely filled). At 1/4th of the distance around the world, Z has fuel for 125 units and X has fuel for 75 units. Z completely fills the tank of X which is now able to fly to a point 3/4 of the way around the world. Now Z has fuel for 50 units. Z now has only 1/3 of its fuel (can travel 50 units) left which is not enough to get back to the airport. But Y reaches it in time in order to refuel it, and both Y and Z air plane are the able to return safely to the airport.
Both Y and Z gets refuelled and fly towards X. Again Y refuels Z and returns to the to be refuelled. Z reaches X at the point where it has flown 3/4 around the world. This time Y and Z come from other direction so that the distance left is 1/4. (If they had come clockwise earlier, they come anti-clockwise this time).

======
A man lives on the tenth floor of a building. Every day he takes the elevator to go down to the ground floor to go to work or to go shopping. When he returns he takes the elevator to the seventh floor and walks up the stairs to reach his apartment on the tenth floor. On a rainy day, or if there are other people in the elevator, he goes to his floor directly. He hates walking so why does he do it?
- The man is (of course) a dwarf. Variants of this puzzle include the clue that on rainy days he goes up in the elevator to the tenth floor (he uses his umbrella!)

======
One fine day, Mr. Puzzle and Mr. Fry were playing cards, but suddenly power went off and they were getting bored. So Mr. Puzzle randomly inverted position of 15 cards out of 52 cards(and shuffled it) and asked Mr. Fry to divide the card in two pile with equal number of inverted cards(number of cards in each pile need not be equal). It was very dark in the room and Mr. Fry could not see the cards, after thinking a bit Mr. Fry divided the cards in two piles and quite surprisingly on counting number of inverted cards in both the piles were equal. What do you think Mr. Fry must have done? 
- Lets say there were n inverted cards initially in top 15 cards, obviously In remaining 37 cards number of inverted cards will be 15-n, as total 15 inverted cards. Now on reversing the 15 cards number of inverted cards would become 15 – n and number of inverted cards will become same in the two piles.

======
100 people standing in a circle in an order 1 to 100. No.1 has a sword. He kills next person (i.e. no. 2) and gives sword to next to next (i.e no.3). All person does the same until only 1 survives. Which number survives at the last?
- This is the famous Josephus Problem. The solution requires getting the nearest smaller number that is the power of 2,in this case 64 and subtract it with the given number.100-64=36.Now we apply the formula 2n+1. 2*36+1=72+1=73.

======
A duck, pursued by a fox, escapes to the center of a perfectly circular pond. The fox cannot swim, and the duck cannot take flight from the water. The fox is four times faster than the duck. Assuming the fox and duck pursue optimum strategies, is it possible for the duck to reach the edge of the pond and fly away without being eaten? If so, how?
Fox can travel 4r  in the time duck covers r distance.  Since fox have to travel half  of  the circumference Pi*r  and Pi*r < 4r. Let the duck rotate around the pond in a circle of radius r/4. Now fox and duck will take exact same time to make a full circle. Now reduce the radius the duck is circling by a very small amount (Delta). Now the Fox will lag behind, he cannot stay at a position as well. Say, the duck circles the pond at a distance r/4 – e, where e is an infinitesimal amount. So as the duck continues to swim along this radius, it would slowly gain some distance over the fox. Once the duck is able to gain 180 degrees over the fox, the duck would have to cover a distance of 3r/4 + e to reach the edge of the pond. In the meanwhile, the fox would have to cover half the circumference of the pond (i.e the 180 degrees). At that point, (pi * r ) > 4 * (3r/4 + e). So time taken to travel 3r/4 is quicker than 3.14*r at four times the speed.(0.14*r distance is left). The duck would be able to make it to land and fly away.

=====
Four glasses are placed on the corners of a square table. Some of the glasses are upright (up) and some upside-down (down). A blindfolded person is seated next to the table and is required to re-arrange the glasses so that they are all up or all down, either arrangement being acceptable, which will be signalled by the ringing of a bell. The glasses may be re-arranged in turns subject to the following rules. Any two glasses may be inspected in one turn and after feeling their orientation the person may reverse the orientation of either, neither or both glasses. After each turn the table is rotated through a random angle. The puzzle is to devise an algorithm which allows the blindfolded person to ensure that all glasses have the same orientation (either up or down) in a finite number of turns.
- On the first turn choose a diagonally opposite pair of glasses and turn both glasses up. On the second turn choose two adjacent glasses. At least one will be up as a result of the previous step. If the other is down, turn it up as well. If the bell does not ring then there are now three glasses up and one down(3U and 1D). On the third turn choose a diagonally opposite pair of glasses. If one is down, turn it up and the bell will ring. If both are up, turn one down. There are now two glasses down, and they must be adjacent. On the fourth turn choose two adjacent glasses and reverse both. If both were in the same orientation then the bell will ring. Otherwise there are now two glasses down and they must be diagonally opposite. On the fifth turn choose a diagonally opposite pair of glasses and reverse both. The bell will ring for sure.

====
Five  puzzleFry ship’s pirates have obtained 100 gold coins and have to divide up the loot. The pirates are all extremely intelligent, treacherous and selfish (especially the captain). The captain always proposes a distribution of the loot. All pirates vote on the proposal, and if half the crew or more go “Aye”, the loot is divided as proposed, as no pirate would be willing to take on the captain without superior force on their side. If the captain fails to obtain support of at least half his crew (which includes himself), he faces a mutiny, and all pirates will turn against him and make him walk the plank. The pirates start over again with the next senior pirate as captain. What is the maximum number of coins the captain can keep without risking his life?
- The captain says he will take 98 coins, and will give one coin to the third most senior pirate and another coin to the most junior pirate. He then explains his decision in a manner like this. If there were 2 pirates, pirate 2 being the most senior, he would just vote for himself and that would be 50% of the vote, so he’s obviously going to keep all the money for himself. If there were 3 pirates, pirate 3 has to convince at least one other person to join in his plan. Pirate 3 would take 99 gold coins and give 1 coin to pirate 1. Pirate 1 knows if he does not vote for pirate 3, then he gets nothing, so obviously is going to vote for this plan. If there were 4 pirates, pirate 4 would give 1 coin to pirate 2, and pirate 2 knows if he does not vote for pirate 4, then he gets nothing, so obviously is going to vote for this plan. As there are 5 pirates, pirates 1 & 3 had obviously better vote for the captain, or they face choosing nothing or risking death.

====
A wholesale merchant came to me one day and posed this problem. Every day in his business he has to weigh amounts from one pound to one hundred and twenty-one pounds, to the nearest pound. To do this, what is the minimum number of weights he needs and how heavy should each weight be?
- The minimum number of weights required is five and these should weight 1, 3, 9, 27 and 81 pounds.

====
The warden meets with 23 new prisoners when they arrive. He tells them, “You may meet today and plan a strategy. But after today, you will be in isolated cells and will have no communication with one another. “In the prison is a switch room, which contains two light switches labeled 1 and 2, each of which can be in either up or the down position. I am not telling you their present positions. The switches are not connected to anything. “After today, from time to time whenever I feel so inclined, I will select one prisoner at random and escort him to the switch room. This prisoner will select one of the two switches and reverse its position. He must flip one switch when he visits the switch room, and may only flip one of the switches. Then he’ll be led back to his cell. “No one else will be allowed to alter the switches until I lead the next prisoner into the switch room. I’m going to choose prisoners at random. I may choose the same guy three times in a row, or I may jump around and come back. I will not touch the switches, if I wanted you dead you would already be dead. “Given enough time, everyone will eventually visit the switch room the same number of times as everyone else. At any time, anyone may declare to me, ‘We have all visited the switch room.’ “If it is true, then you will all be set free. If it is false, and somebody has not yet visited the switch room, you will all die horribly. You will be carefully monitored, and any attempt to break any of these rules will result in instant death to all of you” What is the strategy they come up with so that they can be free?
- The team nominates a leader. The group agrees upon the following rules so that counting can be done by counter: The leader is the only person who will announce that everyone has visited the switch room. All the prisoners (except for the leader) will flip the first switch up at their very first opportunity, and again on the second opportunity. If the first switch is already up, or they have already flipped the first switch up two times, they will then flip the second switch. Only the leader may flip the first switch down, if the first switch is already down, then the leader will flip the second switch. The leader remembers how many times he has flipped the first switch down. Once the leader has flipped the first switch down 44 times, he announces that all have visited the room. It does not matter how many times a prisoner has visited the room, in which order the prisoners were sent or even if the first switch was initially up. Once the leader has flipped the switch down 44 times then the leader knows everyone has visited the room. If the switch was initially down, then all 22 prisoners will flip the switch up twice. If the switch was initially up, then there will be one prisoner who only flips the switch up once and the rest will flip it up twice. The prisoners can not be certain that all have visited the room after the leader flips the switch down 23 times, as the first 12 prisoners plus the leader might be taken to the room 24 times before anyone else is allowed into the room. Because the initial state of the switch might be up, the prisoners must flip the first switch up twice. If they decide to flip it up only once, the leader will not know if he should count to 22 or 23.





References
http://puzzles.nigelcoldwell.co.uk/
