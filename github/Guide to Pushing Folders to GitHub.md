<p>Initialize a Git repository: If you haven't already, navigate to the folder you want to push to GitHub using your command line interface (CLI). Open your command line interface and change the directory to the folder you want to push by using the <code>cd</code> command:</p>

<pre><code class="language-bash">cd path/to/your/folder</code></pre>

<p>Once you're in the correct folder, initialize a Git repository by running:</p>

<pre><code class="language-bash">git init</code></pre>


<p>Add your files: Add the files you want to push to the repository. If you want to add an entire folder and its contents, you can use:</p>

<pre><code class="language-bash">git add .</code></pre>

<p>Commit your changes: After adding the files, commit them to the repository with a meaningful message:</p>

<pre><code class="language-bash">git commit -m "Initial commit"</code></pre>

<p>Create a repository on GitHub: Go to GitHub and create a new repository. Note the repository URL.</p>

<p>Set the remote URL: Connect your local repository to the GitHub repository by setting the remote URL:</p>

<pre><code class="language-bash">git remote add origin &lt;repository URL&gt;</code></pre>

<p>Push to GitHub: Finally, push your changes to GitHub:</p>

<pre><code class="language-bash">git push -u origin master</code></pre>

<p>If you're using a branch other than master, replace <code>master</code> with the name of your branch.</p>

<p>This sequence of commands will push your folder and its contents to GitHub. Remember to replace <code>&lt;repository URL&gt;</code> with the actual URL of your GitHub repository.</p>

<p></b>To get the repository link from GitHub, follow these steps:</b></p>

<ol>
  <li><strong>Navigate to your repository:</strong> Go to the repository on GitHub that you want to push your local files to.</li>
  <li><strong>Click on the "Code" button:</strong> You'll see a green button labeled "Code" near the top-right of the repository page.</li>
  <li><strong>Copy the HTTPS or SSH URL:</strong> When you click on the "Code" button, a dropdown menu will appear. Make sure the tab labeled "HTTPS" is selected, then click the copy button next to the URL to copy it to your clipboard. If you prefer to use SSH, you can select the "SSH" tab and copy that URL instead.</li>
</ol>

<p>That's it! You can now paste the copied URL into your terminal when setting the remote URL with the <code>git remote add origin &lt;repository URL&gt;</code> command.</p>
