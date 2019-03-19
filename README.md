# The Addiction Code

_An experiment in the analysis of Addiction using Code_

## Purpose

After starting my recovery from alcoholism in November 2019, I began to explore my understanding of how addiction truly functions. My experience in computer programming lead me to write this essay on using non-functional example code (known as **pseudocode**) to better understand how and why addiction affects thoughts and actions. My goal is that by sharing my understanding, it may help others struggling with addiction and seeking treatment. 

## Understanding Addiction Using Code

To understand addiction is to understand the nature of thoughts. I find it helpful to think of the human brain as a computer, a logic machine that consumes input, processes data, and returns output. 

Instead of familiar tools like code, compilers, and computer screens, the brain consumes sensory data and returns a human action.

If we were able to read the source code for the human brain, we could understand how the complex things we experience become the lives we live. We could also debug the program, to better understand and treat terrible human conditions such as alcoholism.

## Code For Thoughts

Since we have yet to write a decompiler for the brain, lets use pseudocode to represent the logic behind human behavior. Here's my (extremely) high-level code for a `Thought` object that stores an arbitrary idea:

```
object Thought(idea):
  this.idea = idea
```

As the brain processes all bodily stimuli, it condenses them into `Thoughts`. For example:

```
thought_1 = new Thought("That commercial for pizza looked tasty.")

thought_2 = new Thought("When is the new season of my favorite show?")

thought_3 = new Thought("I stayed up too late last night.")
```

## Thoughts Into Actions

The brain converts these thoughts into decisions and action. For my code to do the same, we store the above example `Thoughts` in a stack called `currentThoughts`. Here's my code to convert `Thoughts` into `Actions`.

```
function currentThoughtsIntoActions():
    action = new Action()
    foreach thought in currentThoughts:
        action.consider(thought.idea)
    action.execute()
```

The predicted human behavior for this stack of `currentThoughts` would involve ordering pizza, checking Netflix, and getting to bed early.

## The Code For Addiction

Addiction is a mutation in the `Thought` code that appends a an additional `Thought` for a constant `ADDICTIVE_DESIRE`. 

```
define ADDICTIVE_DESIRE = "I should drink alcohol."

object Thought(idea):
    this.idea = idea
    if idea is not ADDICTIVE_DESIRE:
        new Thought(ADDICTIVE_DESIRE)
```

In the addicted mind, the stack of `currentThoughts` becomes inundated with `Thoughts` of the `ADDICTIVE_DESIRE`. 

```
foreach thought in currentThoughts
   print thought.idea

> "That commercial for pizza looked tasty."
> "I should drink alcohol."
> "I stayed up too late last night."
> "I should drink alcohol."
> "When is the new season of my favorite show?"
> "I should drink alcohol."
```

## The Slow Crush Of Repetition

These `Thoughts` of `ADDICTIVE_DESIRE` seem like harmless noise, even easy to ignore. The brain continues to process stimuli into human behavior, without any sign of general malfunction. Irrational and dangerous behavior is excused as being occasional and unusual, an anomaly in an otherwise heathy system.

However, because `Thoughts` of `ADDICTIVE_DESIRE` are being created in equal numbers to normal `Thoughts`, eventually the `Actions` become irresponsible, unhealthy, and dangerous. Here's another stack of example `Thoughts`:

```
currentThoughts = [
  new Thought("Time to drive to work."),
  new Thought("I have to finish that important report by the end of today."),
  new Thought("The meeting this afternoon will be long and boring.")
]
```

In a mind with an `ADDICTIVE_DESIRE`, these `currentThoughts` could lead to `Actions` with disasterous consequences.

```
foreach thought in currentThoughts
   print thought.idea

> "I have to finish that important report by the end of today."
> "I should drink alcohol."
> "The meeting this afternoon will be long and boring."
> "I should drink alcohol."
> "Time to drive home from work."
> "I should drink alcohol."
```

This illustrates the subversive and overwhelming nature of addiction. 

## Complications In Recovery

### The Addicted Thought Paradox

The mutation of `Thought` makes an addict struggle to take `Actions` to get help. Because the addict has to believe, and therefore have `Thoughts`, that they should not do what the `ADDICTIVE_DESIRE` leads them to do, the very nature of the disease inhibits its cure. 

```
foreach thought in currentThoughts
   print thought.idea

> "I should stay home and not party tonight."
> "I should drink alcohol."
> "I'm too hungover to get anything done today."
> "I should drink alcohol."
> "I should stop drinking."
> "I should drink alcohol."
```

Unfortunately, until a human's addiction is fully understood and diagnosed, all their selfish and destructive human behavior is interpreted — both by others and by the addict themselves — to be willing decisions. To the addict, the `ADDICTIVE_DESIRE` just seems like a normal part of thinking. Their inability to overcome their `Thought` mutation is seen as personal weakness, or worse, indifference. 

### Indulgence's Downward Spiral

When exposed to the `ADDICTIVE_DESIRE` itself, the recursive nature of the mutation eventually overwhelms the addict's `currentThoughts`. Here's an example of addictive `Thoughts` leading into dangerous `Actions` once indulging.

```
foreach thought in currentThoughts
   print thought.idea

> "I'll have a beer.",
> "I should drink alcohol.",
> "I'll order a shot too.",
> "I should drink alcohol.",
> "I'll order more beers and shots.",
> "I should drink alcohol.",
> "I'm feeling dizzy.",
> "I should drink alcohol.",
> "I can't walk straight.",
> "I should drink alcohol."
```

An addict who continues this pattern will inevitably end up in a psychiatric institution, in jail, or dead.

## How The Mind As Code Can Help Recovery

I've found this method of addiction analysis extremely helpful in my own recovery. 

The logic of the code explained why it's impossible for the addict to overcoming their addiction by themselves. I was competing ineterally against something that hijacked half my thoughts. I needed outside help and support to bring balance to the percentage of thinking about my `ADDICTIVE_DESIRE`.

Using code also allowed me to externalize the addiction from normal `Thoughts`, to separate it from myself and give me space to condemn my situation without condemning myself. I now too could now be angry and disappointed with the actions I had committed, without bearing the entire weight of responsibility.

It also makes it vividly clear why abstaining from the `ADDICTIVE_DESIRE` is paramount to recovery. The mutation, by its nature, abhors the idea of abstinence, as its sole purpose is to consume endlessly. Recovery depends on the strength of thoughts leading away from the `ADDICTIVE_DESIRE` in all its forms.  

## Conclusion

Until we can truly decompile, understand, and patch the inner workings of the human brain, we won't be able to truly fix addiction. But by using a computer model of the brain as a way of understanding thoughts and behavior, we can develop new methods of successful addiction treatment. 

