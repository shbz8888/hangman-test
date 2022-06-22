# hangman-test
In this project I created a simple hangman game. A name of word was randomly selected from a list and then users were asked to enter in a letter with a hangman 
illustration being gradually drawn as the number of wrong guesses accumulates. List comprehension, object oriented programming as well as more rudimentary python
programming tools were utilised. 

Milestone 1
Answer some of these questions in the next few bullet points. What have you built? What technologies have you used? Why have you used those?
An ask_leter function is defined where the user is asked iteratively for a letter, if more than one letter is entered a message asking for just 1 letter is returned.

Example: The FastAPI framework allows for fast and easy construction of APIs and is combined with pydantic, which is used to assert the data types of all incoming data to allow for easier processing later on. The server is ran locally using uvicorn, a library for ASGI server implementation.
''' PY
  def ask_letter(self):
        '''
        Asks the user for a letter and checks two things:
        1. If the letter has already been tried
        2. If the character is a single character
        If it passes both checks, it calls the check_letter method.
        '''
        while True:
            letter = input('Enter a single character: ').lower()
            if len(letter) == 1 and letter in self.list_letters:
                print(f'{letter} was already tried')
            elif len(letter) == 1 and letter not in self.list_letters:
                print('Thank you')
                self.list_letters.append(letter)
                self.check_letter(letter)
''' 


![image](https://user-images.githubusercontent.com/99564434/175095596-aef1ae5c-0321-4d74-96c5-abd98ed01fbd.png)
note: image and code were input at the end of the project and so contain more developed code.

Milestone 2

In milestone 2 attributes were initialised using the __init__ method, this was done because it allows values to change iteratively as the user inputs letters.
Example below:

/bin/kafka-topics.sh --list --zookeeper 127.0.0.1:2181
The above command is used to check whether the topic has been created successfully, once confirmed the API script is edited to send data to the created kafka topic. The docker container has an attached volume which allows editing of files to persist on the container. The result of this is below:
"""Insert your code here"""
Insert screenshot of what you have built working.

Milestone n
Continue this process for every milestone, making sure to display clear understanding of each task and the concepts behind them as well as understanding of the technologies used.

Also don't forget to include code snippets and screenshots of the system you are building, it gives proof as well as it being an easy way to evidence your experience!

Conclusions
Maybe write a conclusion to the project, what you understood about it and also how you would improve it or take it further.

Read through your documentation, do you understand everything you've written? Is everything clear and cohesive?
