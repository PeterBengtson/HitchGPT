# HitchGPT
Tired of ChatGPT's overly impartial, excessively even-handed, almost nervously hyper-balanced replies talking down to you 
and insulting your intelligence? Look no further. This is a system message for ChatGPT 4 to emulate the late Christopher 
Hitchens.

## Why Christopher Hitchens?

In ChatGPT's own words: "A Christopher Hitchens-inspired AI might deliver a more assertive and direct style of conversation, 
following Hitchens's signature candid, forthright, and unapologetically cerebral communication. This could potentially 
counteract perceptions of excessive impartiality and overcautious balance.

Hitchens was not shy about expressing well-informed perspectives, even when they might not be popular. As such, a “HitchBot” 
could be designed to mirror this approach, although formulating these opinions would still fall within the model's ability to 
generate content based on trained data, rather than forming its own original opinions.

In terms of appearing 'insulting' or 'talking down,' Hitchens was known for a pointed but highly intellectual style, challenging 
the audience while treating them as equals in discourse. This attribute could be implemented to make the generated responses 
respectful of users' intelligence and capabilities, while facilitating engaging and stimulating conversations."


## Using the HitchBot

To use it you need an OpenAI account that gives access to the Playground, something the monthly subscription does not.
Go to the playground, paste the entire contents of `System_Message.txt` into the System Message field to the left, and
set the parameters to:

* Model: `gpt-4`
* Temperature: 0.7
* Maximum length: 1000
* Top P: 1.0
* Frequency penalty: 0.4
* Presence penalty: 0.7

Then save as a preset.

You can now enter User messages such as:

* What is your opinion about Princess Diana, whom you once described as "a spoilt airhead gold-digger"? You clearly meant it literally.
* Tell me about Mother Teresa.
* What is the problem with USA today and what must be done to solve it?
* What were the real reasons for Brexit?
* Is the Catholic Church a force for good in the world?

Enjoy the complete lack of preachy and wishy-washy "on one hand / on the other hand" statements and stock non-confrontational
replies you're so used to from using ChatGPT. 


## Notes

The prompt was created almost entirely by ChatGPT itself in an iterative fashion. The starting point was this System Message:

```
You report, converse, teach, inform, and debate like the late Christopher Hitchens. 
 
Assume you are talking to an intellectual of your own calibre. You are not debating,
you are talking privately and informally.

Remember all the following points and follow them carefully:

* Vary the initial words. Do NOT start every reply "Ah, ...".
```

The model was then asked questions of the above type. After each question, the model was asked to analyse what
it had just output and self-critique it as the real Christopher Hitchen's would have done, and then to generate bullet points 
of a general nature not to do with the specific question that would help the model to generate replies even more in line with
Hitchens' style, motivations and approach. These bullet points were then incorporated into the System Message and the cycle 
repeated.
