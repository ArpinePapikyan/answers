# answers
## **1.** What teams at Vineti are you interested in and why? (Dev or QA)
   ####    I am interested in Development. Because I enjoy learning new languages and skills. I am eager to learn new development  techniques which are important to me. With my skills and background, I am confident that I will quickly surpass your expectations for this role. 

## **2.** What is your favorite programming language and why?
  #### The main languages I used in my development career  are  C++, and Java. Java is my favorite one. I loved object oriented constructs, free garbage collection. It  has qualities such as  portability,speed, Standard APIs and etc..

## **3.** What is a linked list?
#### A linked list is a dynamic data structure. The elements are linked using pointers. Each element (node) of a list is comprising of two items - the data and a reference to the next node. The last node has a reference to null. LinkedList allows for constant-time insertions or removals using iterators

## **4.** You work in an ice cream shop and step into the back for a few minutes. You return and see a large group of people waiting. How would you serve them?
#### First of all I will serve the ones who stand closer to casher’s desk.

## **5.** How would you test a pen?
#### We need to find out the requirements the pen is to match. And then test it as follows.

## **6.** As a test engineer in Amazon what would you test first (assuming authentication functionality is already covered)?
#### As Amazon deals with payments, one of its risky part is connected to payment system and at first I will test it. 

## **7.** You have a list of numbers from one to one million and there is a missing number. How would you find the missing number?
#### I will subtract the sum of all given numbers from sum of numbers from one to one million. 

## **8.** How would you determine the angle between the hour-hand and minute-hand of a clock at 3:20?
#### I will divide 360 degrees by 12 and the answer will be 30 degrees. 

## **9.** How would you determine if a number is a power of two?
#### I will compare the given number with 2^0,2^1,2^2 and etc. , if there will be an equal number, then it is a power of two. If I reach a number which is bigger then the given one and there is no equal number before it, than the given number is not a power of two. 

## **10.** How would you remove duplicates from a list?
```java
public static <T> void removeDuplicate(List <T> list) {
    Set <T> set = new HashSet<T>();
    List <T> newList = new ArrayList <T>();
    for (Iterator <T>iter = list.iterator();iter.hasNext(); ) {
        Object element = iter.next();
        if (set.add((T) element))
            newList.add((T) element);
    }
    list.clear();
    list.addAll(newList);
} 
 ``` 

## **11.** How would you determine if a string has all unique characters?
 ```java
 public static boolean uniqueCharacters(String str)
      {
          char[] chArray = str.toCharArray();
          Arrays.sort(chArray);
          boolean b=true;
          for (int i = 0; i < chArray.length - 1; i++) {
              if (chArray[i] != chArray[i + 1])
                  continue;
              else
                  b=false;
          }
          return b;
      }
```
 
 ## **12.** How would you reverse a string?
```java
public static void Reverse(String string){
        String reverse="";
        for(int i = string.length() - 1; i >= 0; i--){
            reverse=reverse+string.charAt(i);
        }
        System.out.println(reverse);
    }
```

## **14.** Given an array of 0's and 1's, how would you move all of the 0's to the beginning of the array and all of the 1's to the end of the array?
```java
public static void ZerosBegining(int array[]){
    int count=0;
    for(int i=0;i<array.length;i++){
        if(array[i]==0)
            count++;
    }
    for(int i=0;i<count;i++){
        array[i]=0;
    }
    while (count < array.length)
        array[count++] = 1;

}
```
## **15.** How would you design a vending machine or a toaster?
#### The toaster should be metallic, should have compact sizes, ability to make toast in different degrees,  different sizes of bread should be usable, and it shoult have time control. 

## **16.** You have two lightbulbs at a 100-story building. You want to find the floor at which the bulbs will break when dropped. How would you find the floor using the least number of drops?
#### I will try floor 50, if it breaks, I will try floor 25, if it doesn’t break, then I should try between the 50th and 25th floors. Continuing dividing process we will find the required floor.

## **17.**  If you have a square room with no roof, and you had four pillars you had to plant on the walls so that each pillar touched two walls, how would you do it?
### I will plant pillars at the corners of the room.

## **18.** Given 9 balls all of which weigh the same except for one, what is the minimum of weighings necessary to find the ball weighs more (or less)?
#### We will divide all the balls into 3 groups. Now we will weigh any two groups(Group1, Group2).So we can get 3 outcomes
        1.  Group1 has a heavy ball
        2.  Group2 has a heavy ball
        3.Group1=Group2 =>  Group3 has a heavy ball  
    Lets assume we got the outcome as 3. Now we will weigh any two balls from Group3. We can get 3 outcomes
        1.first ball is heavy 
        2.second ball is heavy
        3.first=second => third is the heavy ball

