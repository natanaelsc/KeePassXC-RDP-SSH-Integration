# KeePassXC RDP/SSH Integration

1. Install [KeepassXC](https://keepassxc.org) and [Putty 64bit](https://www.putty.org/) for ssh connection.

2. Run **rdp.bat** and **ssh.reg** in order to create uri scheme for *rdp://* and *ssh://* links.

3. Create two folders in KeePassXC named RDP and SSH.

4. Use following **Auto-Type** Sequence for RDP folder.

   ```entry
   {USERNAME}{TAB}{PASSWORD}{ENTER}
   ```

5. Use following **Auto-Type** Sequence for SSH folder.

   ```entry
   {USERNAME}{ENTER}{PASSWORD}{ENTER}
   ```

6. While creating new entries use *ssh://192.168.5.244* or *rdp://192.168.5.244* in URL field.

7. For SSH Edit **Entry** -> **Auto-Type** add "*.*" as Window Title without quotes.

8. For RDP **EditEntry** -> **Auto-Type** add "Remote Desktop Connection" as Window Title without quotes.

9. Usage

   1. Open URL from KeePassXC

   2. Press *CTRL+Shift+V* or clik **Auto-Type** Button in order to trigger **Auto-Type** for credentials.

        note: You might want to clear your RDP history, it's explained well in this link.  
        <http://woshub.com/how-to-clear-rdp-connections-history/>
