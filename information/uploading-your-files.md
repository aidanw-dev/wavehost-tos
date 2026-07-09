# Uploading your files

If you have files from your project and looking to move them here, there is 2 ways to do this,

1. Go to the files tab and click upload&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-11-21 at 23-10-33 Test File Manager (1).png" alt=""><figcaption></figcaption></figure>

Then choose the folder of where your files are located, select the files and then select open and they will upload. The downside of this is it doesn't upload folders.

2. In this example we are using [WinSCP](https://winscp.net). If you do not have a SFTP application, [WinSCP ](https://winscp.net)is a free SFTP application and very easy to use.

Go to your server settings and click Launch SFTP&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-11-21 at 23-15-44 Test Settings (1).png" alt=""><figcaption></figcaption></figure>

Once you have click "Launch SFTP" For WinSCP you get this prompt, the password is the same as your panel password.&#x20;

<figure><img src="../.gitbook/assets/Screenshot 2024-11-21 at 23-41-48 Uploading your files - Wave Hosting Docs (1).png" alt=""><figcaption></figcaption></figure>

Once you have logged in you will see this

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

On the left is you computers files and on the right is your servers files, Find your projects files, select all of them and copy and paste it to the server side.



Note: If you have a Discord bot that uses Node JS, you do not need to copy the node\_modules & package-lock.json, when you start the bot, those files will be made again  but you do need to keep the package.json
