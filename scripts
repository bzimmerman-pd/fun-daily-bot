import requests
import datetime

def get_dad_joke():
    headers = {'Accept': 'application/json'}
    response = requests.get('https://icanhazdadjoke.com/', headers=headers).json()
    return f"😂 Dad Joke: {response['joke']}"

def get_fun_fact():
    response = requests.get('https://uselessfacts.jsph.pl/random.json?language=en').json()
    return f"🤓 Fun Fact: {response['text']}"

def main():
    joke = get_dad_joke()
    fact = get_fun_fact()
    today = datetime.datetime.now().strftime('%A, %B %d')
    final_message = f"🎉 Happy {today}!\n\n{fact}\n\n{joke}"
    print(final_message)

if __name__ == "__main__":
    main()
