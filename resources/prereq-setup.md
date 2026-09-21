# Pre-Event Setup Guide — WIT IT^3 Conference: IBM Workshop — Bob-a-thon

> **Complete these steps before arriving on September 24.**
> The entire setup takes about 10–15 minutes. If you run into trouble, join an
> **office hours session on September 21 or September 22** and an IBM facilitator will help you.

> 📅 **Come to office hours on September 21 or September 22.** If anything in these steps doesn't work for you, don't wait until the day of the event. Office hours are specifically there to fix setup problems before the workshop — it's much easier to resolve issues before September 24 than on the morning of.

---

## Step 1 — Set up your IBMid accounts

> ⚠️ **Most participants need two separate IBMid accounts for this workshop** — one for TechZone/VM access and one for Bob login. Read this step carefully before doing anything.

This workshop uses two IBM services that require IBMid sign-in. For most participants they must use **different IBMid accounts**:

| Service | Which IBMid to use |
|---|---|
| TechZone (VM access) | IBMid tied to **the email you registered for the event with** |
| Bob login (inside the VM) | IBMid tied to a **personal email address** |

**Why two accounts?** Most participants registered with their corporate email, which has an identity provider (IdP) trust set up with IBMid. This works fine on corporate devices, but the lab VMs are not in the trusted corporate domain, so a corporate IBMid sign-in will fail when attempted from inside the VM. A personal-email IBMid bypasses this restriction entirely.

> 💡 **Registered for the event with a personal/Gmail address?** Your VM is already assigned to that personal email, so you only need one IBMid. Use it for both TechZone and Bob login — skip ahead to the "Send your personal IBMid to the event team" section below to make sure we have your address on file for the Bob license.

---

### 1a — TechZone access (event registration email IBMid)

IBM assigned your lab VM to the same email address you used when you registered for the event. This step confirms that IBMid account exists.

1. Go to **[ibm.com/account](https://www.ibm.com/account)**
2. Click **Log in**
3. Enter the **email address you registered for the event with** and click **Continue**
4. If the sign-in succeeds, you will land on the IBM account page. You may see a message saying you have no accesses or no requests set up — **this is normal and expected**. Your IBMid is confirmed — **proceed to Step 1b**
5. If you see "No account found", register at **[ibm.com/account/reg/us-en/signup](https://www.ibm.com/account/reg/us-en/signup)** using that same registration email address, then verify and confirm sign-in works

> 💡 IBM assigned your lab VM to the email address you registered for the event with. A mismatch will prevent you from seeing your VM in TechZone.

---

### 1b — Bob login (personal email IBMid) ← required new step

Because Bob sign-in will not work with a corporate IBMid from inside the VM, you must have an IBMid registered to a **personal email address** (Gmail, Outlook.com, Yahoo, iCloud, etc.).

**Check whether you already have a personal IBMid:**

1. Go to **[ibm.com/account](https://www.ibm.com/account)**
2. Click **Log in**
3. Enter your **personal email address** and click **Continue**
4. If sign-in succeeds — you will land on the IBM account page. You may see a message saying you have no accesses or no requests set up — **this is normal and expected**. Proceed to **"Send your personal IBMid to the event team"** below
5. If you see "No account found", continue to **"Create a new personal IBMid"** below

---

#### Create a new personal IBMid

1. Go to **[ibm.com/account/reg/us-en/signup](https://www.ibm.com/account/reg/us-en/signup)**

   ![IBMid registration form](prereq-setup-images/s1-ibmid-registration-form.png)

2. Fill in the form:
   - **Email address** — enter your **personal email address** (not your work/corporate email)
   - **First name**, **Last name**, **Country/region**
   - Create a **password** (note it somewhere safe — you will need it during the workshop)

3. Click **Create account**

4. Check your **personal email inbox** for a **verification email from IBM** and click the **Verify** link to activate the account

5. Return to **[ibm.com/account](https://www.ibm.com/account)** and sign in with your personal email to confirm the IBMid works. You will land on the IBM account page — you may see a message saying you have no accesses or no requests set up. **This is normal and expected**; your account is active and ready to use.

---

#### Send your personal IBMid to the event team

> ⚠️ **This step is required before the workshop.** Bob licenses are provisioned per-account. If we do not have your personal email address on file, your Bob login will fail on the day of the event.

Once your personal IBMid is confirmed:

1. Email **[melissa.hadley@ibm.com](mailto:melissa.hadley@ibm.com)** with the subject line **"Bob personal IBMid — [Your Name]"**
2. In the body, include your **personal email address** (the one you just registered or verified)
3. Wait for a confirmation reply that your license has been set up before attending the event

> 💡 **Do this as early as possible.** Licenses are set up in batches. If you send your email the morning of September 24, there may not be time to provision your account before the workshop starts. Send it now.

---

## Step 2 — Access TechZone and find your VM

IBM assigned your lab VM to the email address you registered for the event with. Once assigned, it appears in
your TechZone account under **My TechZone → My Requests**.

> **Your reservation may not appear until a few days before the event** — IBM is
> provisioning and assigning VMs between September 18–21. If you check before September 18
> and don't see anything yet, that's expected. Check back closer to the event, and confirm
> access by the **September 21 or September 22 office hours sessions**.

> 📧 **You may receive an email from IBM Bob before the event.** Do not follow the instructions in that email — ignore it and follow the setup steps below instead.

---

### 2a — Sign in to TechZone

1. Go to **[techzone.ibm.com](https://techzone.ibm.com)**

2. Click **Sign in** in the top-right corner

3. Sign in with the **IBMid tied to the email you registered for the event with**

4. You should land on the TechZone home/dashboard page

   ![TechZone home page after sign-in](prereq-setup-images/s2a-techzone-home.png)

---

### 2b — Find your reservation

1. In the TechZone navigation, click **My TechZone** → **My Requests**

   ![TechZone navigation with My TechZone and My Requests highlighted](prereq-setup-images/s2b-my-techzone-nav.png)

2. Look for a reservation with a name similar to **"Bob IDE"** or containing **"Bob"**
   - Status should be **Ready** or **Active** once provisioning is complete

   ![My Requests page showing a Bob IDE reservation in Ready/Active state](prereq-setup-images/s2b-my-requests-reservation.png)

3. Click on the reservation to open its detail page

> **Don't see your reservation?**
> - Make sure you are signed in with the **IBMid tied to the email you registered for the event with** — not your personal one if they differ
> - If it's before September 18, your VM may simply not have been assigned yet — check back
>   in a day or two
> - If you still don't see it after September 18, reach out to your IBM contact or come to
>   an **office hours session on September 21 or September 22**

---

## Step 3 — Connect to your VM

Your lab environment is a Linux desktop you access directly in your browser — no VPN,
no SSH, no software to install.

1. On the reservation detail page, scroll down to the **Environments** table. Find the row
   for **OCP-V RHEL 9 VM - Bob IDE** and click the **twisty arrow** (▶) on the left to
   expand it

   ![Reservation detail page with the Environments table row for OCP-V RHEL 9 VM - Bob IDE expanded](prereq-setup-images/s3-reservation-environments-row.png)

2. In the expanded section, locate **"The console URL for accessing the virtual machine"**
   and click the link

   ![Expanded environment row showing the console URL link highlighted](prereq-setup-images/s3-console-url-link.png)

   > 💾 **Save the console URL and password now — before you click anything else.** Copy the console URL and any VM password shown on this reservation detail page and paste them into a Word document or plain text file saved on your local machine (not inside the VM). You may need them again if your browser tab closes, your session times out during the workshop, or you need to reconnect from a different device. Hunting back through TechZone for them mid-session wastes time — save them here.

3. A new browser tab opens showing the OCP-V console. You may be prompted to sign in with
   your **IBMid** again at this point — use the **same IBMid you used for TechZone** (the email you registered for the event with). Once
   signed in, find your VM in the list and click the **Console** button

   ![OCP-V console page showing the VM listed with the Console button highlighted](prereq-setup-images/s3-ocpv-console-vm.png)

4. Another tab opens showing the RDP connection page. Click **Connect with RDP**

   ![RDP connection page with the Connect with RDP button highlighted](prereq-setup-images/s3-rdp-connect-button.png)

5. The RHEL desktop will load — you should see the home screen with the desktop and taskbar

   ![RHEL home screen loaded in the browser, showing the desktop and taskbar](prereq-setup-images/s3-rhel-desktop-loaded.png)

> 💡 **Working with the OCP-V RDP Web Console & Sending Text:**
> - **Sending text / clipboard into the VM:** Because this is a browser-based RDP web console, standard local copy-paste (Ctrl+V / Cmd+V) may not directly transfer text into the remote desktop. Instead, use the **"Send Text"** button in the toolbar across the top of the console window to paste and send text into the VM.
> - **Login & Password prompts:** If you encounter a login or password prompt, you can use the **"Send Text"** button to send text into the prompt. Note that the toolbar also includes a dedicated button specifically to send/paste the password.
> - **Browser tips:** Chrome and Edge both work well. If any tab shows a blank or black screen, wait 30 seconds and refresh it.

---

## Step 4 — Launch Bob from the terminal

> ⚠️ **Important:** Do **not** double-click the Bob desktop icon. It must be launched
> from a terminal with a specific flag — otherwise Bob may freeze on the first launch.

1. Inside the browser tab (the RHEL desktop), click **Activities** in the top-left corner
   of the screen. A dock appears along the bottom — click the **terminal icon** (it looks
   like a black screen with a command prompt)

   ![RHEL desktop with Activities menu open and the terminal icon highlighted in the dock](prereq-setup-images/s4-rhel-activities-terminal.png)

2. In the terminal, type the following command and press **Enter**:

   ```bash
   bobide --password-store=basic
   ```

   > 💡 **Tip:** To paste this command into the VM rather than typing it manually, use the **"Send Text"** button in the toolbar at the top of the OCP-V console window — standard copy-paste (Ctrl+V / Cmd+V) won't work from your local machine into the VM.

3. Bob will launch. On the very first launch it may take 15–30 seconds to start — this
   is normal

4. **First-launch prompts** — Bob shows several one-time prompts the first time it opens.
   Handle each one as follows:

   - **"Import settings from other editors?"** — Click **Skip** (you do not need to import
     any settings from VS Code or other editors)

   - **"Migrate Bob v1.0.0 chats?"** — A modal window will ask if you want to migrate chats
     from a previous version. Click **Skip migration**

   - **"A new update is available!"** — A small notification may appear in the bottom-right
     corner of the Bob window. You can safely **ignore it or close it** — do not install the
     update during the workshop

5. When Bob finishes loading, you will see a **Log in to Bob** button. Click it

   ![Bob IDE showing the Log in to Bob button before authentication](prereq-setup-images/s4-bob-login-button.png)

   > 💡 **Security warning:** When you click **Log in to Bob**, your operating system or
   > browser may show a security prompt asking if you want to allow Bob to open a browser
   > window. Click **Allow** (or **Open**, depending on the prompt) to continue.

6. A browser window opens automatically. Sign in with your **personal email IBMid** — the personal email address and password you set up in Step 1b.

   > ⚠️ **Do not use your work/corporate email here.** Corporate IBMid sign-in will fail from inside the VM. You must use the personal IBMid you registered in Step 1b and sent to the event team.

7. After signing in, return to the Bob window. Bob should show the chat panel on the
   right side of the interface — you're authenticated and ready

   ![Bob IDE fully loaded with the chat panel visible](prereq-setup-images/s4-bob-chat-panel-ready.png)

---

## Step 5 — Load the lab files into Bob

The workshop labs are stored in a Git repository. You will clone it directly inside Bob
using the built-in Source Control view — no terminal needed.

1. In Bob, click the **Source Control icon** in the left sidebar (it looks like a branching
   line with a circle — third icon from the top)

2. Click **Clone Repository**

3. A text field appears at the top of the screen. Paste the lab repository URL:

   ```
   https://github.com/ibm-client-engineering/it3-bobathon
   ```

   *(Note: Since you are in the OCP-V web RDP console, use the **"Send Text"** button at the top of the console window to paste the repository URL into the VM if standard copy-paste does not transfer over).*

   Press **Enter**

4. A folder picker opens asking where on the VM disk to save the cloned repository. You can select any location on disk (such as `Documents` or your home directory), or optionally create a dedicated folder:
   - Navigate to **Documents** (or your preferred location)
   - Click **New Folder** (for example, named `boblabs` or similar) and select it
   - Click **Select as Repository Destination**

   > 💡 Creating a named folder like `boblabs` keeps your lab files clean and easy to find on the VM disk.

5. Bob will clone the repository. When it finishes, a prompt appears asking
   **"Would you like to open the cloned repository?"** — click **Open**

   > 💡 **What does "Open in Bob" mean?** This is Bob's way of asking whether to load the cloned folder into its workspace so it can read and work with the files. Click **Open** — you should then see the lab folder (`it3-bobathon`) appear in the Explorer panel on the left side of the Bob window.

6. Bob may display a permission prompt asking if it can access files in this folder — click **Allow** (or **Yes**) to continue. This is expected and required for Bob to read the lab files.

7. You may see a dialog asking **"Do you trust the authors of the files in this folder?"** — click **Yes, I trust the authors**. Without this, Bob cannot read or work with the lab files.

8. You may also see a prompt asking you to install an update — click **Skip** (or close the dialog). You do not need to update Bob before the lab.

   > 💡 **Hard double-click to expand folders.** In the Explorer panel, use a firm double-click to expand a folder — there may be a short delay before it opens. Wait a moment before clicking again.

9. Confirm the files loaded: in the Explorer panel on the left, you should see folders named `Lab 1 - Productivity`, `Lab 2 - Research`, `Lab 3 - Developer Efficiency`, and a `README.md` file at the top level. If you don't see these, ask your IBM facilitator.

> ✅ **Setup complete — stop here.** Bob is open, authenticated, and the lab files are
> loaded. **Do not send any prompts yet.** Every message to Bob uses Bobcoins, and you want
> to save them for the workshop labs. Leave Bob open until the event starts.

---

## Step 6 — Read the README before starting

Once you arrive at the event and are ready to begin:

1. In the Explorer panel on the left, click **`README.md`** at the top level of the `it3-bobathon` folder to open it
2. Read it in full — it explains the lab structure, how to use the Bob chat panel, permissions, and where to go for help
3. After reading the README, open `Lab 1 - Productivity/instructions.md` and start a new Bob chat — that's your starting point

---

## Troubleshooting

| Problem | What to do |
|---|---|
| IBMid registration email never arrived | Check spam/junk folder; try resending from the IBMid registration page |
| "No account found" at TechZone sign-in | Confirm you're using the IBMid tied to **the email you registered for the event with** (Step 1a) |
| No reservation visible in My Requests | If it's before Sep 18, check back later; if after Sep 18, contact your IBM event contact |
| Reservation shows but status is "Pending" | Provisioning is still in progress — check back in 30–60 min |
| No "OCP-V RHEL 9 VM - Bob IDE" row in Environments table | Scroll down on the reservation detail page; if missing, contact your IBM facilitator |
| Console URL link is missing from the expanded row | The VM may still be provisioning — wait a few minutes and refresh the page |
| Prompted to sign in again at the OCP-V console | Sign in with the **same IBMid you used for TechZone** (your event registration email) — this is expected |
| RDP connection tab shows a blank or black screen | Wait 30 sec then refresh; if it persists, close the tab and click the console URL again |
| VM disconnects during the workshop | Click the **Console** button on your TechZone reservation detail page to reconnect. When the VM loads, enter your password using the **"Send Text"** button in the top toolbar of the OCP-V RDP web console |
| VM shows a password/lock screen | The screen has locked due to inactivity. Use the **"Send Text"** button in the top toolbar to type your password and unlock it |
| Cannot paste text/URLs/passwords into VM | Use the **"Send Text"** button (or the dedicated password button) in the top toolbar of the OCP-V RDP web console |
| Bob freezes immediately on launch | Close Bob; reopen the terminal and run `bobide --password-store=basic` |
| "Log in to Bob" button doesn't appear | Wait 30 sec; if still missing, close Bob and relaunch with `bobide --password-store=basic` |
| Bob login fails / "account not found" error | You may be signed in with your corporate email — sign out and sign back in with your **personal email IBMid** (Step 1b) |
| Bob login says account is not licensed / no access | Your personal IBMid was not received by the event team in time. Contact your IBM event contact immediately |
| Security warning when clicking Log in to Bob | Click **Allow** or **Open** — this is expected and safe |
| Browser doesn't open when clicking Log in | Look for a browser window behind the Bob window, or open a browser manually and try signing in again |
| Bob asks for credentials you don't recognize | For Bob login use your **personal email IBMid** (Step 1b); for TechZone/OCP-V use your corporate email IBMid (Step 1a) |
| Can't find the terminal | Click **Activities** (top-left), then click the terminal icon in the dock at the bottom |
| "Clone Repository" shows an error or "repository not found" | Confirm you pasted the full URL: `https://github.com/ibm-client-engineering/it3-bobathon` — then try again |
| Haven't sent personal IBMid email to event team yet | Email **melissa.hadley@ibm.com** now with subject "Bob personal IBMid — [Your Name]" and your personal email address |

**Still stuck?** Come to an **office hours session on September 21 or September 22** or reach out to your
IBM event contact before the day of the workshop. Issues are much easier to resolve before
September 24 — please don't wait until you arrive.

---

*WIT IT^3 Conference: IBM Workshop — Bob-a-thon · September 24, 2026 · Charlotte & Atlanta*
