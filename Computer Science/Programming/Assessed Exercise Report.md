## <u>Task A</u>

### Exercise 1:

![[Pasted image 20251126145210.png]]

### Exercise 2:


![[Pasted image 20251203171721.png]]

### Exercise 3:

![[Pasted image 20251203172548.png]]

### Exercise 4:
![[Pasted image 20251203173826.png]]
### Exercise 5:
| Inputs                       | Expected output              | Actual output                        | Changes made           |
| ---------------------------- | ---------------------------- | ------------------------------------ | ---------------------- |
| 1, 2, 3, 4, 5                | 3                            | ![[Pasted image 20251205102759.png]] | N/A                    |
| a,b,c,d,e                    | Program does nothing         | ![[Pasted image 20251205102914.png]] | input validation added |
| a,b,c,d,e                    | Program throws error message | ![[Pasted image 20251205103327.png]] | N/A                    |
| -3000,3.017897,3.1,4034000,1 | 806201                       | ![[Pasted image 20251205103529.png]] | N/A                    |
### Exercise 6:
| Inputs | Expected output                                   | Actual output                        | Changes made                                         |
| ------ | ------------------------------------------------- | ------------------------------------ | ---------------------------------------------------- |
| -4824  | No errors are thrown, calculates a negative value | ![[Pasted image 20251205104007.png]] | Modified input validation to include negative hours. |
| -4824  | Program throws error                              | ![[Pasted image 20251205104137.png]] | N/A                                                  |
| abcd   | Program throws error                              | ![[Pasted image 20251205104203.png]] | N/A                                                  |

### Exercise 7:
| Inputs | Expected output      | Actual output                        | Changes made |
| ------ | -------------------- | ------------------------------------ | ------------ |
| a      | Program throws error | ![[Pasted image 20251205105042.png]] | N/A          |
| -1039  | Program throws error | ![[Pasted image 20251205105118.png]] | N/A          |

### Exercise 8:
| Inputs                  | Expected output            | Actual output                                  | Changes made                    |
| ----------------------- | -------------------------- | ---------------------------------------------- | ------------------------------- |
| 1,2,3,4,5 and 6,7,8,9,0 | The words are not anagrams | ![[Pasted image 20251205105523.png]]           | N/A                             |
| apple, orange           | The words are not anagrams | ![[Pasted image 20251205105605.png]]           | N/A                             |
| fried, fired            | The words are anagrams     | ![[Pasted image not anagrams.png]]             | The program now sorts the lists |
| fried, fired            | The words are anagrams     | ![[Pasted image these words are anagrams.png]] | N/A                             |
### Exercise 9:
| Inputs     | Expected output | Actual output                        | Changes made |
| ---------- | --------------- | ------------------------------------ | ------------ |
| 45672      | 0 vowels        | ![[Pasted image 0 vowels.png]] | N/A          |
| aaeeiioouu | 10 vowels       | ![[Pasted image vowels.png]]         | N/A          |
| tomato     | 3 vowels        | ![[Pasted image tomato.png]]         | N/A          |

### Exercise 10:
| Inputs         | Expected output | Actual output                          | Changes made                                                               |
| -------------- | --------------- | -------------------------------------- | -------------------------------------------------------------------------- |
| 10, 9, 8, 7    | 7, 8, 9, 10     | ![[Pasted image four numbers.png]]   | N/A                                                                        |
| x, h, k, n     | h, k, n, x      | ![[Pasted image some letters.png]]     | N/A, letters are sorted alphabetically, unintended but makes no difference |
| -1, -2, -3, -4 | -4, -3, -2, -1  | ![[Pasted image negative numbers.png]] | N/A                                                                        |

### Exercise 11:
| Inputs | Expected output | Actual output                        | Changes made |
| ------ | --------------- | ------------------------------------ | ------------ |
| 0      | 0               | ![[Pasted image 0.png]] | N/A          |
| 2493   | 18              | ![[Pasted image 18.png]]             | N/A          |
| 24a3   | Invalid input.  | ![[Pasted image invalid input.png]]  | N/A          |

### Exercise 12:
| Inputs | Expected output | Actual output                        | Changes made |
| ------ | --------------- | ------------------------------------ | ------------ |
| Madam  | True            | ![[Pasted image also is palindrome.png]] | N/A          |
| M3d3m  | True            | ![[Pasted image is palindrome.png]]  | N/A          |
| M3d2m  | False           | ![[Pasted image not palindrome.png]] | N/A          |

### Exercise 13:
| Inputs     | Expected output | Actual output                        | Changes made |
| ---------- | --------------- | ------------------------------------ | ------------ |
| aaa        | Weak            | ![[Pasted image weak.png]]           | N/A          |
| 111111A    | Weak            | ![[Pasted image 20251205144626.png]] | N/A          |
| 111111A$   | Medium          | ![[Pasted image 20251205144651.png]] | N/A          |
| 11111111A$ | Strong          | ![[Pasted image 20251205144757.png]] | N/A          |
### Exercise 14:
| Inputs                       | Expected output                  | Actual output                        | Changes made |
| ---------------------------- | -------------------------------- | ------------------------------------ | ------------ |
| inputs given in the lab file | average: 73.125, letter grade: b | ![[Pasted image 20251207162656.png]] | N/A          |
| removed one of the subjects  | 80.83333...., B                  | ![[Pasted image 20251207162735.png]] | N/A          |
| removed another subject      | 78.75, B                         | ![[Pasted image 20251207162754.png]] | N/A          |

### Exercise 15:
| Inputs                               | Expected output | Actual output                        | Changes made |
| ------------------------------------ | --------------- | ------------------------------------ | ------------ |
| [1,5 ,600], [100 ,7, 3 , 29, 39]     | 597             | ![[Pasted image 20251207164512.png]] | N/A          |
| [1,5 ,600], [100 ,7, 3 , 602, 39]    | 601             | ![[Pasted image 20251207164543.png]] | N/A          |
| [-100,5 ,600], [100 ,7, 3 , 602, 39] | 702             | ![[Pasted image 20251207164624.png]] | N/A          |

### Exercise 16:
| Inputs                           | Expected output | Actual output                                                                      | Changes made                                              |
| -------------------------------- | --------------- | ---------------------------------------------------------------------------------- | --------------------------------------------------------- |
| inputs from the brightspace file | N/A             | Each error you make in programming is an opportunity to become a better developer$ | The for statement only iterates through n instead of n-1. |
| inputs from brighspace           | N/A             | Each error you make in programming is an opportunity to become a better developer! | N/A                                                       |

### Exercise 17:
| Inputs | Expected output | Actual output                        | Changes made              |
| ------ | --------------- | ------------------------------------ | ------------------------- |
| 60000  | 48568           | ![[Pasted image 20251207172806.png]] | subtractions were changed |
| 60000  | 48568           | ![[Pasted image 20251207173204.png]] | N/A                       |
| 600000 | 348825          | ![[Pasted image 20251207173558.png]] | N/A                       |

### Exercise 18:
| Inputs                           | Expected output                  | Actual output                        | Changes made |
| -------------------------------- | -------------------------------- | ------------------------------------ | ------------ |
| "apple", "banana", "orange", "," | ["apple", "banana", "orange"]    | ![[Pasted image 20251207174753.png]] | N/A          |
| "Hello, how are you?", " "       | ['Hello,', 'how', 'are', 'you?'] | ![[Pasted image 20251207174921.png]] | N/A          |

### Exercise 19:
| Inputs    | Expected output | Actual output                        | Changes made                                  |
| --------- | --------------- | ------------------------------------ | --------------------------------------------- |
| aaabbcaaa | (a, 3)          | ![[Pasted image 20251207181446.png]] | N/A                                           |
| hellooooo | (o, 5)          | ![[Pasted image 20251207181620.png]] | last tuple wasnt added when for loop finished |
| hellooooo | (o, 5)          | ![[Pasted image 20251207181652.png]] | N/A                                           |
| banana    | (b, 1)          | ![[Pasted image 20251207181706.png]] | N/A                                           |
| abc       | (a, 1)          | ![[Pasted image 20251207181718.png]] | N/A                                           |
### Exercise 20:
| Inputs                                                                           | Expected output           | Actual output                        | Changes made |
| -------------------------------------------------------------------------------- | ------------------------- | ------------------------------------ | ------------ |
| [("tv", 300), ("mobile phone", 800), ("laptop", 600), ("headphones", 200)], 1100 | tv, mobile phone, 0       | ![[Pasted image 20251207183808.png]] | N/A          |
| [("tv", 300), ("mobile phone", 800), ("laptop", 600), ("headphones", 200)], 1500 | mobile phone, laptop, 100 | ![[Pasted image 20251207183826.png]] | N/A          |
| [("tv", 300), ("mobile phone", 800), ("laptop", 600), ("headphones", 200)], 900  | tv, laptop, 0             | ![[Pasted image 20251207183900.png]] | N/A          |


## <u>Task B</u>
![[Untitled Diagram.drawio(2).png]]