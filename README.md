#Project Title : CHATBOT 

##Summary:
My Project is baised on CHATBOT its work throught Openai. 
In this project first import a Openai.To run a openai create a key.taken a function "chat_with_gpt".The modle of Openai is "gpt-3.5-turbo".
passes a messages in a object. user to have complition i had taken "return......"
For runing pyhton file directly written"if_name_".for asking a question from user Used "While". after "breaking" I had created a "response" then Used "Print".

#Code :
```
import openai 

openai.api_key = "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"

def chat_with_gpt(prompt):
    response = openai.ChatCompletion.create(
        modle="gpt-3.5-turbo",
        messages=[{"role": "user", "content": prompt}]
    )
    return response.choices[0].message.content.strip()

    if__name__ == "__main__":
        while True:
            user_input = input("You: ")
            if user_input.lower() in ["quite", "exit", "bye"]:
                break
            
            response = chat_with_gpt(user_input)
            print("chatbot: ", response)
```

##Data Sources:
For Api_key : [api_key](https://platform.openai.com/settings/profile?tab=api-keys)

##What Next?

This is a normal chatbot code i wana create a extream level of chatbot . That chatbot can give a Image, links & many sources should avlailable. i am working on it !

