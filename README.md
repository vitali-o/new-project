1. Log in into your GitHub account. 
2. Create repository "new-project" 
3. Go to project settings and add deploy keys with write access. 

More information here: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/managing-deploy-keys

4. Return to console, go to working directory and run commands:

$ echo "test" >> README.md

$ git init

$ git remote add origin git@github.com:YOUR_ACCOUNT/new-project.git

$ git add .

$ git commit -m "init"

5. Push commit to your github project to test write access:

$ git push origin main

6. Create development branch and switch to it

$ git checkout -b development

7. Write your code, add it to stage, commit. Push it to github with command:

$ git push origin development

8. To merge development to main branch:

$ git checkout main

$ git merge development

$ git git push origin main
