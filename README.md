Download Link: https://assignmentchef.com/product/solved-ados-assignment-1-file-explorer
<br>
Build a fully functional File Explorer Application, albeit with a restricted feature set

<strong>Prerequisites: </strong>

<ol>

 <li>Basic usage and architectural know-how of file explorer features</li>

 <li>Preliminaries such as C/C++ code compilation, execution &amp; debugging</li>

</ol>

<strong>Requirements: </strong>

Your File Explorer should work in two modes –

<ol>

 <li>Normal mode (default mode) – used to explore the current directory and navigate the filesystem</li>

 <li>Command mode – used to enter shell commands</li>

</ol>

The root of your application should be the directory where the application was started.

The application should display data starting from the top-left corner of the terminal window, line-by-line. You should be able to handle text rendering if the terminal window is resized. The last line of the display screen is to be used as a status bar.




<strong>Normal mode: </strong>

Normal mode is the default mode of your application. It should have the following functionalities –

<ol>

 <li>Display a list of directories and files in the current folder

  <ol>

   <li>Every file in the directory should be displayed on a new line with the following attributes for each file –

    <ol>

     <li>File Name</li>

     <li>File Size</li>

    </ol></li>

  </ol></li>

</ol>

<ul>

 <li>Ownership (user and group) and Permissions iv. Last modified</li>

</ul>

All of this should be displayed in human readable format

<ol>

 <li>The file explorer should show entries “.” and “..” for current and parent directory respectively</li>

 <li>The file explorer should handle scrolling in the case of vertical overflow using keys <strong>k</strong>​ &amp; ​ <strong>l</strong>​</li>

 <li>User should be able to navigate up and down in the file list using the corresponding up and down arrow keys</li>

</ol>

<ol start="2">

 <li>Open directories and files</li>

</ol>

When enter key is pressed –

<ol>

 <li>Directory – Clear the screen and navigate into the directory and show the directory contents as specified in point 1</li>

 <li>File – Open the file in vi editor</li>

</ol>

<ol start="3">

 <li>Traversal

  <ol>

   <li>Go back – Left arrow key should take the user to the previously visited directory</li>

   <li>Go forward – Right arrow key should take the user to the next directory</li>

   <li>Up one level – Backspace key should take the user up one level</li>

   <li>Home – <strong>h</strong>​ key should take the user to the home folder (the folder where the application​ was started)</li>

  </ol></li>

</ol>




<strong>Command Mode: </strong>

The application should enter the Command button whenever “:” (colon) key is pressed. In the command mode, the user should be able to enter different commands. All commands appear in the status bar at the bottom.

<ol>

 <li>Copy – ‘copy &lt;source_file(s)&gt; &lt;destination_directory&gt;’ Move – ‘move &lt;source_file(s)&gt; &lt;destination_directory&gt;’</li>

</ol>

Rename – ‘rename &lt;old_filename&gt; &lt;new_filename&gt;’

<ol>

 <li>Eg – copy foo.txt bar.txt baz.mp4 ~/foobar​     move foo.txt bar.txt baz.mp4 ~/foobar    rename foo.txt bar.txt</li>

 <li>Assume that the destination directory exists and you have write permissions.</li>

 <li>Copying/Moving directories should also be implemented</li>

 <li>The file ownership and permissions should remain intact</li>

</ol>

<ol start="2">

 <li>Create File – ‘create_file &lt;file_name&gt; &lt;destination_path&gt;’</li>

</ol>

Create Directory – ‘create_dir &lt;dir_name&gt; &lt;destination_path&gt;’

<ol>

 <li>Eg – ​ ​create_file foo.txt ~/foobar create_file foo.txt .    create_dir foo ~/foobar</li>

</ol>

<ol start="3">

 <li>Delete File – ‘delete_file &lt;file_path&gt;’ Delete Directory – ‘delete_dir &lt;dir_path&gt;’</li>

</ol>

The file/dir path should be relative to the root from where the application is run

<ol start="4">

 <li>Goto – ‘goto &lt;location&gt;’

  <ol>

   <li>Eg – goto &lt;directory_path&gt;​</li>

   <li>Absolute path wrt application root will be given</li>

  </ol></li>

</ol>




<ol start="5">

 <li>Search – ‘search &lt;file_name&gt;’ or ‘search &lt;directory_name&gt;’

  <ol>

   <li>Search for a given file or folder under the current directory recursively</li>

   <li>Output should be True or False depending on whether the file or folder exists</li>

  </ol></li>

 <li>On pressing ​<strong>ESC</strong>​ key, the application should go back to Normal Mode</li>

</ol>

<strong> </strong>