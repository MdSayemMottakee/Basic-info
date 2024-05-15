<p><strong>Clone the Repository:</strong></p>

<p>Open Git Bash and navigate to the directory where you want to clone the repository (or use <code>cd</code> to navigate to the desired directory). Then, use the <code>git clone</code> command followed by the repository URL:</p>

<pre><code class="language-sh">git clone <em>repository_URL</em></code></pre>

<p>This command will clone the repository from GitHub to your local machine.</p>

<p><strong>Navigate into the Repository Directory:</strong></p>

<p>Once the cloning process is complete, navigate into the cloned repository directory using <code>cd</code>:</p>

<pre><code class="language-sh">cd <em>folder</em></code></pre>

<p>This command changes your current directory to the cloned repository directory.</p>


<p><strong>GitHub Branch Merge and Cleanup Guide</strong></p>

<p>To merge a branch in GitHub and perform cleanup tasks, follow these steps:</p>

<ol>
  <li><strong>Merge Branches into Main</strong></li>
</ol>

<p><strong>Step 1: Check out the main branch</strong></p>

<p>First, switch to the main branch (commonly named main or master).</p>

<pre><code class="language-sh">git checkout main</code></pre>

<p><strong>Step 2: Merge each branch into main</strong></p>

<p>Merge each branch into the main branch one by one.</p>

<pre><code class="language-sh">git merge branch_name</code></pre>

<p>Repeat this for each branch you want to merge. Resolve any merge conflicts that arise during this process.</p>

<ol start="2">
  <li><strong>Push Changes to Remote Repository</strong></li>
</ol>

<p>Push the merged changes to the remote main branch on GitHub.</p>

<pre><code class="language-sh">git push origin main</code></pre>

<ol start="3">
  <li><strong>Delete Local Branches</strong></li>
</ol>

<p>Once merged, you can delete the local branches.</p>

<pre><code class="language-sh">git branch -d branch_name</code></pre>

<p>If the branch hasn't been fully merged, and you still want to delete it, use:</p>

<pre><code class="language-sh">git branch -D branch_name</code></pre>

<ol start="4">
  <li><strong>Delete Remote Branches</strong></li>
</ol>

<p>Next, delete the branches on the remote repository.</p>

<pre><code class="language-sh">git push origin --delete branch_name</code></pre>

<p>Alternatively, you can delete the branches through the GitHub website:</p>

<ul>
  <li>Go to your repository on GitHub.</li>
  <li>Click on the "Branches" tab.</li>
  <li>Delete the branches you no longer need by clicking the trash can icon next to each branch.</li>
</ul>

<p><strong>Handling Unrelated Histories Error</strong></p>

<p>If you encounter an error related to unrelated histories, it means the branches have diverged and Git cannot automatically merge them. In this case, you can either open Git Bash in the file directory or clone the repository again using the following command:</p>


<p>To merge a branch in GitHub, follow these steps:</p>

<ol>
  <li><strong>Merge the branch:</strong> Merge the branch into your current branch using the following command. This example merges the 'master' branch from the remote 'origin' repository. Replace 'master' with the name of the branch you want to merge.</li>
</ol>

<pre><code class="language-bash">git merge origin/master --allow-unrelated-histories</code></pre>

<ol start="2">
  <li><strong>Commit the merge:</strong> After merging, commit the changes with a meaningful message.</li>
</ol>

<pre><code class="language-bash">git commit -m "Merge unrelated histories"</code></pre>

<ol start="3">
  <li><strong>Push the changes to GitHub:</strong> Finally, push the changes to the remote repository. Replace 'main' with the name of your target branch.</li>
</ol>

<pre><code class="language-bash">git push origin main</code></pre>
