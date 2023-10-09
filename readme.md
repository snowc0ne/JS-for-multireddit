Step 1:
To get all of your old Subreddits, follow this guide:


If you created a new Reddit account and want to join all the same communities from your old account, follow the steps below on reddit.com: 

Log in to your old Reddit account. 
Visit www.reddit.com/subreddits/mine.
On the right-hand side under HOME FEED SUBREDDITS, right click on multireddit of your subscriptions, copy link address, and edit the URL so it says old.reddit.com instead of reddit.com, and copy the URL.
Log out of your Old Reddit account then in an incognito session, Log in to your new Reddit account and paste the copied URL. 




Step 2:
Here is the Javascript you will have to input into the console to iterate through every join button on that page:
"
// Get all the "join" buttons on the page
const joinButtons = document.querySelectorAll('a.active.add.login-required');

// Loop through each "join" button and click it
for (const button of joinButtons) {
  button.click(); // Click the button
  await new Promise(resolve => setTimeout(resolve, 1000)); // Wait for a second (adjust the delay as needed)
}
"

You will just have to paste the above script in the console pane on the multireddit of all your SubReddits.

