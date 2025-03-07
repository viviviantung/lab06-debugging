# lab06-debugging

https://www.shadertoy.com/view/csXXzn

Bug 1: compiler error (line 95) - fixed by adding "2" to "vec"

Bug 2: spheres are squished down (line 11) - fixed by computing H by dividing by iResolution.y instead of iResolution.x

Bug 3: sphere positions are too close to the camera and off-center (line 100) - fixed by raycasting using uv2 instead of uv

Bug 4: no specular reflection (line 75) - fixed by reflecting dir instead of eye

Bug 5: ground does not extend far enough (line 18) - fixed by increasing the number of iterations we march from 64 to 200

# Setup 

Create a [Shadertoy account](https://www.shadertoy.com/). Either fork this shadertoy, or create a new shadertoy and copy the code from the [Debugging Puzzle](https://www.shadertoy.com/view/flGfRc).

Let's practice debugging! We have a broken shader. It should produce output that looks like this:
[Unbelievably beautiful shader](https://user-images.githubusercontent.com/1758825/200729570-8e10a37a-345d-4aff-8eff-6baf54a32a40.webm)

It don't do that. Correct THREE of the FIVE bugs that are messing up the output. You are STRONGLY ENCOURAGED to work with a partner and pair program to force you to talk about your debugging thought process out loud.

Extra credit if you can find all FIVE bugs.

# Submission
- Create a pull request to this repository
- In the README, include the names of both your team members
- In the README, create a link to your shader toy solution with the bugs corrected
- In the README, describe each bug you found and include a sentence about HOW you found it.
- Make sure all three of your shadertoys are set to UNLISTED or PUBLIC (so we can see them!)
