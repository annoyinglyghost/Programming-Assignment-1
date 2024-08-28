### EXPERIMENT 1
## INTRODUCTION TO PYTHON PROGRAMMING
#### Name: Mariane Iszley V. Samar
#### Section: 2ECE-D


## ALPHABET SOUP PROBLEM

def alphabet_soup(a): 
    
    char_list = list(a) #to convert the string to list
    
    char_list.sort() #sorting the list
    
    sorted_string = ''.join(char_list) #to join the characters back into a list but alphabetically
    
    return sorted_string

print(alphabet_soup("hello"))  #Examples

print(alphabet_soup("hacker")) 



## EMOTICON PROBLEM

def emote(sentence):
    
    emoticons = {"smile": ":)", "grin": ":D", "sad": ":(", "mad": ">:("} #defining a dictionary to make the words convert to emoticons
    
    words = sentence.split() #split the sentence to words
    
    transformed_words = [emoticons.get(word, word) for word in words] #replace the words to emoticons
    
    return ' '.join(transformed_words) #join the words back into a string

print(emote("Make me smile"))  #Examples

print(emote("I am mad"))       


## UNPACKING LIST PROBLEM

lst = [1, 2, 3, 4, 5, 6] #the list

uno = lst[0] #to print first index
ultima = lst[-1] #to print the last index
medio = lst[1:-1] #removing the first number and last number to print in the output

print(f"first: {uno}") #printing results

print(f"middle: {medio}")

print(f"last: {ultima}")
