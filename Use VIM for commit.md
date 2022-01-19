

This is mostly a question about using VIM, so let's to it.

First, you need to setup Git to use Vim as the editor, if that's not the default for you.

You can do that by adding to the git config of your choice (none which is local, --global or --system):

**git config --global core.editor vim**

Then when you commit, you don't add the -m parameter, leave it blank:

**git commit**

// or

**git commit -a**


After that, you are in VIM, in escape mode. You then need to start insert mode to write. 
The simplest way is to type **i**, and a message will appear on the bottom (-- INSERT --). 
You are in insert mode and you can now type in your message.

After that, you must exit insert mode, and you do that by pressing Esc once. 
The -- INSERT -- message on the bottom should vanish. 
You are now in escape mode again, and you must save and quit.

That is done by using the **":"** key to enter command mode and typing the command **wq** or **x**, leaving you with either **:wq** or **:x** typed at the bottom.

**w** stands for write and **q** for quit, so **wq** is write and quit. **x** is an alias for **wq**.

After that you just press Enter and you're done, out of VIM.

If you have any doubts post a comment and I'll add it up.

FROM https://stackoverflow.com/questions/48208487/how-to-add-commit-message-using-vim
