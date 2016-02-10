# Your Computer and *You*

For some of you, using your computer is second nature. For others, it's an entirely new experience. We want to share some knowledge and tips that will hopefully help everyone spend more time coding and less time stressing about their machines.

### OSX Tips

1. **Spotlight Search**
  - You can quickly get to almost anything on your computer by pressing `⌘ + space`, and typing in the name of what you're looking for.
  - This works for System Preferences like `Displays` & `Security & Privacy`, Applications like `Slack` or `iTerm2`, and even your browser history, emails, etc.
2. **The System Preferences are Your Friend**
  - System Preferences are there to make your computer *really yours*.
  - Take some time to navigate them and see what they all do. Pretty much everything here is a dropdown with a few options, or a checkbox. Play around with the options and see what you like.
  - If something serious might happen by toggling a preference, you will get a warning form the computer.
  - (One preference that can be awkward at first, but makes a big difference after a while is turning on `Scroll Direction: Natural` under `Trackpad > Scroll & Zoom`)
3. **Take Advantage of Desktops, Spaces, and Windows**
  - To add a Desktop or Space, try swiping up with 3 or 4 fingers (depends on your preferences) and pressing the '+' icon to the right of the bar that appears at the top of the screen.
  - To navigate between them, swipe with 3 or 4 fingers left or right at any point.
  - You can put open windows in any Space you want by dragging the window into another desktop after you swipe up to open the Spaces view.
  - Turn off `Automatically rearrange Spaces based on most recent use`, under `Mission Control` in the System Preferences. (this will put in more control of what Space goes where)
  - You can assign an application to a specific Desktop by right clicking its icon from the Dock and selecting one of the `Assign To` choices under `Options`.
4. **Make The Dock Work for You**
  - Maybe your Dock is a little big for your taste? Grab the dividing bar over near the trash icon and drag it up or down to resize the entire Dock.
  - You can pin any folder to the Dock (Applications, Documents, DPL folder...), and by right-clicking on the folder, you can change how it interacts (I personally like `Display as: 'Folder'` & `View content as: 'Grid'`).
  - Don't use Contacts or Calendars a lot? Remove them from the Dock! Pin the apps you use a lot instead! (Maybe iTerm2, your editor, etc.)
5. **Option Click All the Things**
  - Don't want notifications popping up while you're trying to work, but don't want to turn them off permanently? Hold `option` and click the notification icon in the top-right corner of your screen (looks like three lines with bullet points), when it's grey, you won't get notifications on your screen. Option click again to turn them back on.
  - Option clicking can also reveal a lot of normally hidden data in your toolbar. Try option clicking the speaker, WiFi, or Bluetooth icons.

### Workspace Tips

Before getting too far into keeping a clean workspace, lets clear up a point of confusion.

__*Memory vs Storage*__

It's easy to mix the two up, and a technical explanation doesn't always clear it up. But on a very basic level:
- Memory is your computer's capacity to think. Memory in most computers today is measured in gigabytes (GB), and typically comes in multiples of 4. Most MacBooks now come with 4, 8, or 16 GB of memory, or RAM. Memory is taken up by running processes on your computer. Think running Applications, watching a video, listening to music.
- Storage is the room that your computer has to store data. This is taken up by Applications, Music, Photos, Movies, Documents, etc. Think of things that you save as the use for your storage. Your storage space is determined by the capacity of your `hard drive` (HDD or SSD). Common capacities include 128GB, 256GB, 512GB, 1TB, etc.

__*Keep Your Computer Running Clean and Lean*__

1. **Manage Your RAM**
  - The less memory your computer has available, the more you should do to manage it. [Memory Monitor](https://itunes.apple.com/us/app/memory-monitor-speed-up-your/id748212890?mt=12) is an application that will run in your toolbar, visualizing your memory usage and helping to show you what processes are taking more memory than others. It is recommended that you install Memory Monitor no matter what amount of RAM your computer has to work with.
  - Your computer spends memory and CPU rendering open tabs and windows. The more tabs you have open (Chrome, Sublime, Atom, Firefox, etc.) the slower (and hotter) your machine will be. Get into the habit of closing things you aren't using, and your computer will thank you by running faster and cooler. (This will also extend your computer's lifespan significantly)
2. **Clean Your Machine**
  - Get into the habit of being organized. Try to have a place for everything on your computer other than cluttering up your Desktop. If you can get into the habit of cleaning up your Desktop and Downloads once a week, chances are you'll wind up with more free storage space in the long run.
  - As for cleaning out the harder to reach spots on your machine, [Disk Expert](https://itunes.apple.com/us/app/disk-expert-space-usage-analyzer/id488920185?mt=12) & [DaisyDisk](https://itunes.apple.com/us/app/daisydisk/id411643860?mt=12) are two popular paid solutions for visualizing available disk space and managing what is stored on your machine.
  - [Gemini](https://itunes.apple.com/us/app/gemini-the-duplicate-finder/id463541543?mt=12) will search out and show you all duplicate files on your machine and is great for freeing up storage space in places like Photos, iTunes, & Downloads.
3. **Start Up Efficiently**
  - Over time, you may start to notice a lot of icons accumulating in your toolbar. In your System Preferences, under `Users & Groups > Login Items` you will see a list of some of your startup applications. See something in there you don't use regularly? Applications like `ScreenHero`, `Google Drive`, & `Dropbox` will still work if you turn off their startup on login functions. Turn off things you don't use regularly to make room for the things that you do.
  - Speaking of starting up, you will probably notice that your computer feels like it's running a little more smoothly after you turn it off and back on again. Turning your computer off or even just restarting it can be very good for its health, and it runs a little quicker when you do! Try to restart at least a few times a week.
4. **For Your Convenience**
  - [Caffeine](https://itunes.apple.com/us/app/caffeine/id411246225?mt=12) is a small toolbar application that will turn of your computer's sleep timer, allowing you to keep your screen awake if you're doing lots of looking but not much typing. (Great for pair programming, watching logs, movies, etc.)
  - Use `iTerm` ! It offers a lot of small conveniences that OSX's `Terminal` does not, and looks better doing it.
  - As you get better with your keyboard, you might find that your cursor doesn't zip around as quickly as you might like. Your system preferences will let you turn your key repeat rate down pretty low, but not the *lowest*. Opening your command line and running:
  ```
  defaults write NSGlobalDomain KeyRepeat -int 0
  ```
   will set your key repeat rate as low as possible, so your cursor will be moving as quickly as possible, keeping you coding and not tapping the arrow keys.
  - Try to come up with a file structure that works well for you. A strongly recommended structure that can help lead to fewer Github headaches down the road is to have all of your work for this course in one over-arching folder (`DPL` in this example):
    - Inside `DPL` we have a folder for each week of the course e.g. `Week1`, `Week2`, `Week3` ... (Don't use spaces when naming folders anymore. If you must, use_an_underscore)
    - Each of these `Week` folders will be where you work for the week. If you are working on small single page scripts (.rb/.js files, etc.) put them all in a folder named something like `Scripts` inside the `Week`'s folder. If you are working on something a little bigger like a webpage that uses more than one file to run, or a Rails app, put it in its own folder inside that `Week`'s folder.
    - This file structure allows you to organize everything neatly, but will also help to avoid problems once we start using git and Github.
    - Example:
    ```
    /DPL
    -- /Week1
    ----- /Scripts
    ----- /Notes
    ----- /Examples
    -- /Week2
    ----- /Scripts
    ----- /my_first_webpage
    ----- /Notes
    -- /Week3
    ----- /Scripts
    ----- /rails_app
    ----- /another_rails_app
    ----- /Notes
    ```
