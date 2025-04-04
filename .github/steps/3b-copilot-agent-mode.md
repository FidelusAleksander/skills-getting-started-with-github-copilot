### :keyboard: Bonus Activity - Preview of GitHub Copilot Agent Mode

Nice! You found this hidden bonus level! 🎮 👾

If you have been keeping an eye on Github, you may have heard about **Agent** mode.
It's a public preview feature for GitHub Copilot.

But... it's only for _Insiders_! 😎🤫

But... good news. Anyone can access the Insiders version if they know the tricks. Yay! 🧐🎉

> [!IMPORTANT]
> This activity is optional and ungraded.
> Since the Insiders version is updated daily, please expect to see differences or have breaking changes.

### What is "Agent" Mode?

**Agent** mode enhances Copilot by automatically providing it feedback, typically the types of feedback you would provide after reviewing Copilot's suggested edits.

**Agent** mode gives Copilot a feedback loop, enabling it to inspect its own results for issues, bugs, inconsistency, etc. in the code and even the terminal! This allows it to automatically revise its work in many situations. Similarly this means **Agent** mode can
typically handle more complex and multi-step tasks.

That's just a brief intro and there is much more to learn, but that's for a dedicated future exercise. (hint)

Now, let's give **Agent** mode a try! 👩‍🚀

### :keyboard: Activity: Switch to Insiders mode

If you are not familiar with the Insiders program, please use the below steps to switch your VS Code to the **Insiders** version and your Copilot extension to the **Pre-release** version.

> [!NOTE]
> While switching you will may likely receive an error messages about extension incompatability. This will be resolved after both versions are changed.

1. Ensure you are in a browser-based instance of VS Code (your Codespace).

   > **Tip:** This allows switching to **Insiders** mode without installing another version on your local computer.

1. In the bottom left, click the **Manage** icon and select the **Switch to Insiders Version...** option.

   <img width="300" alt="image" src="https://github.com/user-attachments/assets/11580b67-9891-4aa9-9a7c-04aff1e7ef9c" />

1. In the left navigation, select the **Extensions** tab.
   Find the **GitHub Copilot** entry, click the **Manage** icon, and select **Switch to Pre-Release Version**.

   <img width="300" alt="image" src="https://github.com/user-attachments/assets/39e1d9ae-ba50-4cd7-b6b6-eb51aa0a35aa" />

   A greeen tag will be added in the top left to indicate the pre-release version.

   <img width="160" alt="image" src="https://github.com/user-attachments/assets/21ee8307-0c6d-4e8e-965d-cfd729edfe4c" />

### :keyboard: Activity: Test out Copilot Agent mode! 🧑‍🚀

Let's experiment with some more open-ended requests that will add more functionality to our web application. Remember, AI assistants often produce different results, even if the same prompt is provided. If you don't get the desired results, you can try other models or provided followup feedback to refine the results.

1. Ensure you using **both** the insiders version of VS Code and the pre-release version of the GitHub Copilot extension.

1. Open the **Copilot** side panel and use the dropdown menu to switch to **Agent** mode.

   <img width="250" alt="image" src="https://github.com/user-attachments/assets/201e08ab-14a0-48bf-824e-ba4f8f43f8ab" />

1. Time for our test! Let's ask Copilot to add functionality for removing participants.

   > <img width="13px" src="https://github.com/user-attachments/assets/98fd5d2e-ea29-4a4a-9212-c7050e177a69" /> **Prompt**
   >
   > ```prompt
   > #codebase Please add a delete icon next to each participant and hide the bullet points.
   > When clicked, it will unregister that participant from the activity.
   > ```

   - If you try this prompt in **Edit** mode, you will propbably find that the changes to the frontend and backend were made in a theoretical way. Although no syntax or runtime errors occurred, the changes were not compatible and didn't achieve the goal.
   - In **Agent** mode, Copilot reviewed its own work and refined it to ensure all changes were error free and coordinated together.

1. When Copilot is finished, restart the debugger and inspect the results. If you like the results, press the **Keep** button. If not, try providing Copilot some feedback to refined the results.

1. Ask Copilot to fix a registration bug.

   > <img width="13px" src="https://github.com/user-attachments/assets/98fd5d2e-ea29-4a4a-9212-c7050e177a69" /> **Prompt**
   >
   > ```prompt
   > #codebase I've noticed there seems to be a bug.
   > When a participant is registered, the page must be refreshed to see the change on the activity.
   > ```

   - If you try this prompt in **Edit** mode, it may or may not work.

1. When Copilot is finished, inspect the results. If you like the results, press the **Keep** button. If not, try providing Copilot some feedback.

### :keyboard: Activity: Test out Copilot Agent mode, _again_! 🧑‍🚀🚀

Just for fun, let's try something even more difficult and open-ended to see what happens!

> [!TIP]
> In our experiments, we got working results most of the time, but not every time.
> You might try other models or pausing to provide Copilot feedback.

1. (optional) If it is available for you, you might try another model such as `Claude 3.5 Sonnet`.

   <img width="250" alt="image" src="https://github.com/user-attachments/assets/16125b88-8428-4f62-9c1b-5761e26ed888" />

1. Ask Copilot to install a local database service.

   > <img width="13px" src="https://github.com/user-attachments/assets/98fd5d2e-ea29-4a4a-9212-c7050e177a69" /> **Prompt**
   >
   > ```prompt
   > Please install a local mongodb server for development reasons.
   > Afterward, run a command that lists the collections to verify the service is active and working.
   > Do not modify our program yet.
   > ```

   - We purposly made the default development environment not ready for installing a local MongoDB server.
   - You will see Copilot make mistakes, analyze the error messages, and ask to run various extra commands to make the environment suitable. Nice!

1. Ask Copilot to change our app to use the database service. 🤯

   > <img width="13px" src="https://github.com/user-attachments/assets/98fd5d2e-ea29-4a4a-9212-c7050e177a69" /> **Prompt**
   >
   > ```prompt
   > #codebase I don't like that we are storing the data in memory.
   > Let's switch to using mongodb.
   > For now use the local development instance.
   > Please prepopulate the database with the existing hardcoded json activities, keeping the activity name as the key.
   > ```

1. That's your preview for now. We hope it was fun and please check back soon on the [Skills page](https://skills.github.com) for a dedicated exercise to explore even more of Agent Mode! 🧑‍🚀 🚀
