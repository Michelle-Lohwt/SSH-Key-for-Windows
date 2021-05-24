# SSH-Key-for-Windows
This is regarding SSH-Key for Windows version, hope it helps :)

Main Reference: [Git and GitHub for Beginners - Crash Course](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&start_radio=1&t=829s)

Author: Michelle Loh

## Main Reference Recap
1. [14:30 cloning through VS Code](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=870s) - git clone *ssh from github*
2. [17:30 git commit command](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=1050s)  - git status
3. [18:15 git add command](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=1095s)   - git add.
4. [19:15 committing](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=1155s)  - git commit -m "*Title of changes*" -m "*Some descriptions*"
5. [20:20 git push command](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=1220s)  - git push
6. [20:30 SSH Keys](https://www.youtube.com/watch?v=RGOj5yH7evk&list=RDCMUC8butISFwT-Wl7EV0hUK0BQ&index=1&t=1230s)
    1. Generating SSH key</br>
        <details>
        <summary>Create a new key <strong>OR</strong></summary>
        a. Key in
        
          `ssh-keygen -t rsa -b 4096 -C "your_email@.com"` </br>
        b. Enter the key name（Let say you enter the key as **thekey**)
        </details>
        <details>
        <summary>Already have a key</summary>
        a. Key in （Let say you enter the key as <strong>thekey</strong>)
    
           ssh-keygen -t rsa -b 4096 -C "your_email@.com"
        b. Choose whether to overwrite the key
        </details>
        <strong>THEN</strong>
        <details>
        <summary>Enter the passphrase</summary>
            
        ```
            Enter passphrase (empty for no passphrase): [Type a passphrase]
            Enter same passphrase again: [Type passphrase again]
        ```
        (if no passphrase just leave it empty by clicking on the "Enter" key)
        </details>
     2. Check whether the SSH key is generated
        <details>
        <summary>ls <strong>OR</strong></summary>
        a. Key in 
    
            ls
        b. Notice that the last 2 rows are the generated key
        ```
        thekey -- private (only you can access)
        thekey.pub -- public (open to the public to access)
        ```
        </details>
        <details>
        <summary>ls -al ~/the-key-name.pub</summary>
        a. Key in
    
            ls -al ~/the-key-name.pub
           (change <i>the-key-name</i> to the name you generated)</br>
           In our case will be:
           ```
           ls -al ~/thekey.pub
           ```
        </details>
     3. Copy the public key


# References
<details>
    <summary>Reference Links</summary>
1. <a href="https://www.jcchouinard.com/learn-git-and-github/">Learn Git and Git Hub</a><br>
2. <a href="https://www.youtube.com/watch?v=ZeWx0XNUZWE">Setup Username and Email with Git and GitHub in Visual Studio Code on Windows</a><br>
3. <a href="https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh">Connecting to GitHub with SSH</a><br>
    <ol>
        <ol>
        <li><a href="https://docs.github.com/en/github/authenticating-to-github/checking-for-existing-ssh-keysd">Checking for existing SSH keys</a></li>
        <li><a href="https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent">Generating a new SSH key and adding it to the ssh-agent</a></li>
        <li><a href = "https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account">Adding a new SSH key to your GitHub account</a></li>
        <li><a href = "https://docs.github.com/en/github/authenticating-to-github/testing-your-ssh-connection">Testing your SSH connection</a></li>
        <li><a href = "https://docs.github.com/en/github/authenticating-to-github/working-with-ssh-key-passphrases">Working with SSH key passphrases</a></li>
        <li><a href = "https://docs.github.com/en/github/authenticating-to-github/working-with-ssh-key-passphrases#auto-launching-ssh-agent-on-git-for-windows">Auto-launching ssh-agent on Git for Windows</a></li>
        <li><a href = "https://docs.github.com/en/github/authenticating-to-github/error-permission-denied-publickey">Error: Permission denied (publickey)</a></li>
            </ol>
        </ol>
4. <a href= "https://stackoverflow.com/questions/60984908/how-can-i-delete-all-ssh-keys-from-my-mac">How can I delete all SSH keys from my Mac</a><br>
5. <a href= "https://stackoverflow.com/questions/18880024/start-ssh-agent-on-login">Start ssh-agent on login</a>
</details>
