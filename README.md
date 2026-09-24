**Live project:** [Play Little Buddy](https://jp4890-coder.github.io/little-buddy/)

**GitHub repository:** [jp4890-coder/little-buddy](https://github.com/jp4890-coder/little-buddy)

# Little Buddy — Interactive Virtual Pet

**Group 5: Little Buddy**

## Main idea

My idea was to create a small, playful virtual pet experience using HTML, CSS, and JavaScript. Users first choose a cat, dog, or rabbit and give it a name. They can then feed it, play with it, or click directly on it to give it a gentle pat. A happiness meter and changing facial expressions show how the pet responds to their care.

I wanted each animal to have its own personality: the cat purrs through a text reaction, the dog wags its tail, and the rabbit wiggles its ears. Floating hearts, bouncing movements, and a colorful design make the interactions feel friendly and approachable.

As the project developed, I added a request bubble so users need to pay attention to what their pet wants. Feeding a hungry pet or playing with a bored pet increases happiness. Choosing the mismatched action lowers happiness, and repeated mismatches change its expression from sad to angry to furious. Reaching 100 happiness unlocks a lucky message.

## Selected prompts

These excerpts show the main steps in developing the experience with OpenAI Codex:

1. **Initial concept:** “Create a small interactive virtual pet experience where users first choose a cat, dog, or rabbit and give it a name.”
2. **Planning and implementation:** “Help me plan the experience before building it.” / “Use HTML, CSS, and JavaScript. Keep the design simple and playful.”
3. **Reward:** “When the happiness level reaches 100, it gives users a lucky message.”
4. **Responding to needs:** “Add a bubble next to the pet showing its status” and “If there is a mismatch (e.g., hungry -> play), the happiness drops.”
5. **Stronger emotional feedback:** “When there is a mismatch, the facial expression should go from ‘sad -> angry -> ... getting worse’.”

## Reflection

*Draft reflection based on the project’s development.*

The project began as a simple pet-care experience where every interaction increased happiness. Adding hungry and bored requests gave users a reason to read the pet’s status and choose an appropriate action. The interaction became more meaningful because the same button could help or disappoint the pet depending on its current need.

I also wanted the feedback to be visible in the pet itself, rather than only in a number. The original expressions represented happiness levels, while the later sad-to-angry-to-furious progression communicates repeated mismatches. Meeting the requested need resets frustration, so users have a clear way to help the pet recover. The lucky message adds a small reward for reaching full happiness.

Codex helped plan the interaction, generate the HTML, CSS, JavaScript, and animal illustrations, and revise the behavior through my follow-up prompts. My role was to define the experience and decide how the pet should respond. The successive prompts helped turn a general idea into more specific rules and feedback.

The implementation was checked through browser interactions and programmatic checks of scoring, request matching, frustration, rewards, and resets. These checks do not replace testing with real users. I have not established whether users immediately understand the requests or find the emotional progression enjoyable.

There are still limitations. Needs alternate predictably between hungry and bored, and pats increase happiness without fulfilling either need, so users can reach the reward through repeated pats. Progress resets when the page reloads, and the cat’s purr is shown as text rather than sound. Future improvements could explore more varied requests and user feedback on how clearly the pet communicates its feelings.

## Run the project

The experience is contained in `index.html` and does not require installing packages. Open that file directly in a browser, or start a local preview from this project’s folder:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Then open [the local preview](http://127.0.0.1:8765/).
