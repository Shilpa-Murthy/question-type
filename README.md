# question-type

def check_type(sentence,list):
    
    j=0
    s=sentence.split(" ")
    
    if s[0] in affirmation:
            print('Question type: affirmation')

    else:
        
        for i in s:
            
              if i in list:
                 print('Question Type: ',i)
                 break
              else:
                 print('Question Type : Unknown')


sentence = input('Enter question : ')
list = ['who' , 'what' , 'when']
affirmation = ['would' , 'can' , 'does' , 'is' , 'do' , 'are' , 'could' , 'will' , 'has']
check_type(sentence,list)
