# AI Art Auto-Animator
## Key Features

### Generation Automation
The goal of this package is to utilize https://www.wombo.art/ efficiently. Traditionally, users would enter a prompt using the UI,
and then hope for a good result. Using this package, we can programatically generate hundreds of variants without manual effort 
(e.g., opening new tabs, copy pasting prompts, hitting enter, etc). This will programatically hit the end point, rather than
use the public UI.

### Animation
Furthermore, using the traditional UI, the output is only a single, final resultant png. But what if we want to see the process that the 
AI went through to generate this final output? Luckily, the API generates "stages" that the generation went through, which we can download,
and then combine later to generate an animation from frame 0 to frame N (where N is the final frame of the generation). This allows for more 
interesting usages of the output.

## Future work
1. Parse most popular pages on Reddit / other platforms to gather text input files (e.g., an entire /r/AskReddit post)
2. Convert audio files to a text transcript
3. Parse some input text file (may need to be a CSV instead of a pure .txt file) and analyze sentiment to gather words of interest for use in generation
4. Morph between words of interest, rather than simply start from scratch each time.
5. Automatically combine frames into a video of some desired length (e.g., 40 fps over 10 seconds requires 400 frames of animation)
6. (if applicable) Overlay an input .mp3 file over the video generated in step 3 (likely 1080x1920)
7. (if applicable) Generate deepfake voiceover for use in converting text -> audio.
8. (if applicable) Automatically generate text animations to place over the visuals generated
9. Automate publishing to YouTube Shorts

## Credit 
- Art generation: https://www.wombo.art/ 
- Wombo API: https://github.com/leopoldhub/wombo-dream-api (need to move to https://github.com/cdgco/dream-api as it is more active)

## Installation 
- TODO: write installation guide. 
- TODO: remove `node_modules` folder once installation guide is written

Required: Node.js
