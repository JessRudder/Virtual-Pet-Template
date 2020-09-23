Create your own site using VirtualPet (designed by [CyberPig123](https://github.com/CyberPig123) and coded by [platy11](https://github.com/platy11) and you)!

1) To adopt your very own Pet Egg click "Use this template"
2) Enter <your-user-name>.github.io as the repository name (for instance, I would put JessRudder.github.io)
3) Click "Create repository from template"
4) Go to <your-user-name>.github.io and start playing with your new Pet Egg! See (JessRudder.github.io)[jessrudder.github.io] as an example.

Note: If your new friend isn't there yet, don't worry (sometimes shipping is delayed). Just wait a few moments and refresh the page until the egg arrives.

![Pet Egg](images/egg_happy_256.png)

Once you've learned your pet's habits, it's time to start hacking on the code!

Right now your pet only has one type of food to eat. If we check the code in `index.js` it looks like there are other foods, but we can't see them yet because our pet isn't at a high enough level.

```
  function checkFoodsUnlocked() {
    if (Number(localStorage.getItem('expLevel')) > 9) {
      document.querySelector('.food2').classList.remove('hidden')
    }
    if (Number(localStorage.getItem('expLevel')) > 39) {
      document.querySelector('.food3').classList.remove('hidden')
    }
  }
```
We could wait until level 9, but that's sooooooo far away and we want our eggy friend to have a new treat sooner! Lets change that to level 1 instead!

In GitHub, go to the repository that has the code for your Pet Egg. This should be at github.com/<your-user-name>/<your-user-name>.github.io.
 
You should see a list of files. Click on `index.js`.

Click on the edit icon (it's the pencil on the top right of the page). You're now in edit mode and can modify this file!

Go to the `checkFoodsUnlocked` method (around line 75).

Swap the 9 for a 0. The method should now look like this:

```
  function checkFoodsUnlocked() {
    if (Number(localStorage.getItem('expLevel')) > 0) {
      document.querySelector('.food2').classList.remove('hidden')
    }
    if (Number(localStorage.getItem('expLevel')) > 39) {
      document.querySelector('.food3').classList.remove('hidden')
    }
  }
```

Scroll to the bottom of the page and click "Commit changes"

Refresh the page your Pet Egg lives on and marvel at the new foods you have to feed it!

Ready to hack some more. Here are some ideas:
- Add another food for your pet to eat. Remember that you'll need to change the code AND and images for this new treat.
- Change the starting color of your egg. Why should it always be yellow in the beginning?
- Make the egg follow your mouse automatically instead of waiting for you to click on the screen.
- Why should we only have pet eggs? Add the ability to adopt a pet carrot too!
