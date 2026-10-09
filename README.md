# Big Bang Boggle

A free multiplayer Boggle game for phones. There's no server, no accounts and no cost.

## Publish it on GitHub Pages (about 5 minutes)

1. Sign in at https://github.com, or create a free account.
2. Click **+** → **New repository**. Name it `boggle`, set it to **Public**, then click **Create repository**.
3. Click **uploading an existing file**, drag in these three files, then click **Commit changes**:
   - `index.html`
   - `words.txt`
   - `qrcode.min.js`
4. Go to **Settings** → **Pages**. Under *Build and deployment*, choose **Deploy from a branch**, then **main** and **/ (root)**, and click **Save**.
5. Wait 1–2 minutes. Your game is live at `https://<your-username>.github.io/boggle/`

## Running it on the day

- **On the big screen:** open `https://<your-username>.github.io/boggle/?host`
- Pick a round length and a join time, then click **Create round 1**. Use 30 seconds or more for round 1, so people have time to scan.
- Players scan the QR code with their phone camera, or open the link on a laptop and type the code. Then they enter their name.
  The board appears for everyone at the same moment.
- When time's up, players screenshot their score screen and post it in the chat. The highest score wins the round.
- Click **Start round 2**. You get a new board and a new QR code with the same settings.
  Players either scan the new QR code, which takes them straight in because their name is remembered, or type the new code into the **Next round** box on their results screen.
- Repeat for round 3. **Change round settings** goes back to the setup screen.
- **Started by accident?** While a round is counting down or being played, use **↺ Restart round**, which gives a new board and new join link but keeps the same round number. Or use **✕ Cancel round** to go back to setup; the round won't count.
  Players who already joined keep seeing the old round, so post the new join link in the chat.
- **Resetting for a new game:** after any round, click **Finish game & reset to round 1**. The setup screen also has a **Start again from round 1** link.
- **Playing on the host laptop:** use the **Play on this computer** button. The big-screen board is for display only.

## How it works

- The round code (for example `K7QZ3`) encodes the start time and length, and the board is generated from that code.
  So everyone with the same code gets the same board and timer, without any server.
- Words are checked against a built-in English dictionary of about 170,000 words, including British spellings.
- Scoring: 3 letters = 1 point, 4 = 2, 5 = 3, and so on (letters minus 2). The "Qu" tile counts as 2 letters.
- **Timer sync relies on device clocks.** Phones and laptops set their time automatically, so they're usually within a second of each other.
  If someone's board appears noticeably early or late, their device clock is wrong.
