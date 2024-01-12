<body>
    <h1>Git & Github-Manual</h1>
    <p>
        <h3>Git</h3>
        Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers who are collaboratively developing source code during software development.
        <h3>Github</h3>
        GitHub is a web platform that provides a centralized location for developers to store, manage, and collaborate on their code using Git.
    </p>
    <h2>HOW TO USE GIT & GITHUB?</h2>
    <h3>Getting Started:</h3>
    <ul>
        <li> Clone the repository to your local machine using the following command:<br>
        <code>git clone https://github.com/ruskinbk/ruskinbk.git</code></li>
    </ul>
    <h3>Making Changes:</h3>
    <ul>
        <li> After making changes to the code, add the files to the staging area using the following command:<br>
        <code>git add &lt;file_name&gt;</code></li>
        <li> Commit the changes with a meaningful message:<br>
        <code>git commit -m "Your commit message here"</code></li>
    </ul>
    <h3>Collaboration:</h3>
    <ul>
        <li> Push the changes to the remote repository:<br>
        <code>>git push origin &lt;branch_name&gt;</code></li>
        <li> Merge changes from another branch into your current branch:<br>
        <code>git merge &lt;branch_name&gt;</code></li>
    </ul>
    <h3>Understanding History:</h3>
    <ul>
        <li> To view the commit history:<br>
        <code>git log</code></li>
        <li> If you want to revert to a previous commit:<br>
        <code>git revert &lt;commit_hash&gt;</code></li>    
    </ul>
    <h3>Branch Operations:</h3>
    <ul>
        <li> To switch to a different branch:<br>
        <code>git checkout &lt;branch_name&gt;</code></li>
        <li> Create a new branch and switch to it:<br>
        <code>git checkout -b &lt;new_branch_name&gt;</code></li>
        <li> If you want to delete a branch:<br>
        <code>git branch -d &lt;branch_name&gt;</code></li>
    </ul>
    <p>Remember to adapt these commands to your specific workflow and project needs.</p>    
    <h2>GIT & GITHUB IN DETAIL:</h2>
    <h4>Configuring Git:</h4>
    <p>Configure your global Git settings with the following commands:</p>
    <pre><code>git config --global user.name "My name"</code></pre>
    <pre><code>git config --global user.email "myname@email.com"</code></pre>
    <pre><code>git config --list</code></pre>
    <h4>Clone & Status:</h4>
    <p>Clone a repository to your local machine using the following command:</p>
    <pre><code>git clone &lt;repository_link&gt;</code></pre>
    <p>Check the status of your code with:</p>
    <pre><code>git status</code></pre>
    <p>
        <ul>
        <li>Untracked: New files not tracked by Git</li>
        <li>Modified: Changed files</li>
        <li>Staged: Files ready for commit</li>
        <li>Unmodified: Unchanged files</li>
    </ul>
    </p>
    <h4>Add & Commit:</h4>
    <p>Add new or changed files to the Git staging area:</p>
    <pre><code>git add &lt;file_name&gt;</code></pre>
    <pre><code>git add .  # Add all files at once</code></pre>
    <p>Record changes with a meaningful message:</p>
    <pre><code>git commit -m "Your commit message here"</code></pre>
    <h4>Push Command:</h4>
    <p>Upload local repository content to the remote repository (GitHub):</p>
    <pre><code>git push origin main</code></pre>
    <h4>Init Command:</h4>
    <p>Initialize a new Git repository, set the remote, check branches, rename the main branch, and push:</p>
    <pre><code>git init</code></pre>
    <pre><code>git remote add origin &lt;repository_link&gt;</code></pre>
    <pre><code>git remote -v  # Verify remote</code></pre>
    <pre><code>git branch  # Check branch</code></pre>
    <pre><code>git branch -M main  # Rename branch</code></pre>
    <pre><code>git push origin maint</code></pre>
    <pre><code>git push -u origin main  # Set upstream for future pushes</code></pre>
    <h4>Workflow:</h4>
    <p>GitHub Repository ➔ Clone ➔ Make Changes ➔ Add ➔ Commit ➔ Push</p>
    <h4>Git Branches:</h4>
    <pre><code>git branch  # Check branch</code></pre>
    <pre><code>git branch -M main  # Rename branch</code></pre>
    <pre><code>git checkout &lt;branch_name&gt;  # Switch to a branch</code></pre>
    <pre><code>git checkout -b &lt;new_branch_name&gt;  # Create and switch to a new branch</code></pre>
    <pre><code>git branch -d &lt;branch_name&gt;  # Delete branch</code></pre>
    <h4>Merging Code:</h4>
    <h5>Way 1:</h5>
    <pre><code>git diff &lt;branch_name&gt;  # Compare commits, branches, files, and more</code></pre>
    <pre><code>git merge &lt;branch_name&gt;  # Merge two branches</code></pre>
    <h5>Way 2:</h5>
    <p>Create a pull request on GitHub to inform others about the changes you've pushed to a branch in the repository.</p>
    <h4>Pull Command:</h4>
    <p>Pull changes from the remote repository to your local machine:</p>
    <pre><code>git pull origin main</code></pre>
    <h4>Undoing changes:</h4>
    <p><strong>Case 1: Staged changes</strong></p>
    <pre><code>git reset &lt;file_name&gt;</code></pre>
    <pre><code>git reset</code></pre>
    <p><strong>Case 2: Committed changes (for one commit)</strong></p>
    <pre><code>git reset HEAD~1</code></pre>
    <p><strong>Case 3: Commit changes (for many commits)</strong></p>
    <pre><code>git reset &lt;commit_hash&gt;  # Soft reset</code></pre>
    <pre><code>git reset --hard &lt;commit_hash&gt;  # Hard reset</code></pre>
    <p><strong>Note:</strong> <code>git log</code> to check all commit history.</p>
    <h4>Fork:</h4>
    <p>A fork is a new repository that shares code and visibility settings with the original “upstream” repository.</p>
</body>
