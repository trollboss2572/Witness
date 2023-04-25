# Witness
An Android App to play the out of print board game Witness.

I'm very new to this whole "programming" outside of a class framework so I don't really know what I should put here but here I go.

The basic structure is simple. Each activity is hardcoded. The only potential change is the change in text or inclusion of different images.

The menu/character selection/HowToPlay/GameMenu is hardcoded.

The actual game consists of 5 screens; a confirmation screen, the introduction screen, the hidden information screen, the question screen, and the solution screen.

Each of these activities works similarly, so I will consider an arbitrary activity.

The activity has a certain template. (Usually some text and an image) When the user selects a scenario from the game menu screen, it passes that information
via intent to the game. The arbitrary activity then searches the resource files for the array of the specific type, and the index of that array.
For instance, if the Question activity is to be loaded, and we are playing scenario 10, the string to be printed to the user is given in 
Question[10].

There are different pieces of hidden information with regards to the characters, so each character has a specific hidden information array which is referenced.

The above process applies for all scenarios and activites. Any non-hardcoded string will follow the process of getting the index of the correct array for its string/image
resource.

This is a pretty small project. That's all the documentation I can think of.
