# Mac-OS

<a href="/downloads/Mac/Alpha9.zip">Latest Download</a>


Install Directions:

> - Download the lastest Version, or another version of your choice
> - IMPORTANT Unzip the file in `finder`, MacOs lets you open and use zip files without opening them, but this will fail if you dont extract everything
> - Once unziped `right click` on the unzipped folder -> `New terminal at Folder`
> - Type these commands:
    >     - `chmod +x ./` Just press tab it should auto complete the file name for you, hit _enter_ after
    >     - `chmod -R 755 .` <- yes a '.' and Press _enter_
> - Go back to finder open the folder and click on the file it will fail to open
> - Go to `settings` -> `Privacy/Security`, scroll to the bottom and you'll see the file there and a button that says `open anyway` press this

What this all did 'chmod +x ./[filename]' this adds execute permissions since the build is made from a windows pc it doesn't get this permission.
'chmod -R 755 .' adds the correct read write execute permission necessary to run a file.
Settings Privacy/Security is apples Gatekeeper, apple doesn't like files that it doesn't already know so this is the bypass Gatekeeper method.

---

All Versions:

- <a href="/downloads/Mac/Alpha3.zip">Alpha 3</a>
- <a href="/downloads/Mac/Alpha4.zip">Alpha 4</a>
- <a href="/downloads/Mac/Alpha9.zip">Alpha 9</a>