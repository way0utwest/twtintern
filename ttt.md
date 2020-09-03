TTT - Interns DevOpsin'

[Dry run of talk - 7/2/2020](https://msit.microsoftstream.com/video/4a1ba4ff-0400-8385-2ddd-f1eaed355c13)

[Director's cut of talk - REQUIRED VIEWING](https://web.microsoftstream.com/video/8855a1ff-0400-8388-b805-f1eaed5e6329)

[Deck - Sept 3, 2020](https://microsoft.sharepoint.com/:p:/t/StudentZoneatBuild2020/Ed8cjRuGkOVFmwDU_IO5HvwBr1pnO2HjO7I5IPAbfK-M7w?e=XgLa0k)

---

# Requirements

Your computer (windows/mac/linux) requires the following:

* Visual Studio Code (with terminal)
* Web Browser  
* GitHub repo forked (you need to run actions, your fork required)
* Azure Account (to create resources for deployment)
* [Hugo](https://gohugo.io/getting-started/installing/)

Prep for session:

1. ensure any existing old versions linked to your fork are deleted.

   1. ensure your fork does not have `.github\workflows` files (this will cause a conflict)

2. Desktop setup should be similar to the following:

   1. LEFT on monitor - browser
      1. Open fork of repo in tab
      2. Open Azure portal in tab
   2. RIGHT on monitor - VSCODE
      1. Have fork cloned locally and opened in this 
      2. have terminal open and in the hugo directory 

3. DEMO 1 -

   1. You're just showing the code and the minimal of how hugo works
   2. OPEN GITHUB REPO: https://github.com/jaydestro/twtintern
   3. Show them them **config.yaml** – explain that this is how the site is built using hugo and a theme
   4. Open VSCODE – show directory structure 
   5. explain Hugo is a cli tool, open source, go, can be installed anywhere
   6. Show in terminal – hugo binary – show a quick build (run `hugo` in terminal in root directory of repo fork) 
   7. – explain it renders the markdown into html/css/javascript – go back to deck -  continue presentation.

4. DEMO 2 - 

   ![image-20200902112334852](https://tva1.sinaimg.cn/large/007S8ZIlgy1gicpywuippj30qm0akdgm.jpg)

   1. Open Browser – Open Portal – Search for Static Web Applications in search at top
   2. Click "+" and create new SWA
   3. create new resource group, just explain minimal what it is
   4. create site name, example twtinterns2020 - explain it's not hostname - just logical name
   5. Select region, EAST US 2
   6. explain free due to preview
   7. click sign in with github (Make sure you auth your session for GitHub's integration at least once before to save time.)
   8. select org, select repo select branch, click build/next
   9. enter `/` for app location
   10. REMOVE details from API location
   11. enter `public` in artifact location
   12. click review and create – explain ARM will validate our request for this infrastructure (make sure everything we selected is valid)
        click create 
   13. Go to newly created SWA  Show URL SHOW WORKFLOW - - DESCRIBE WHAT’S IN YAML
   14. CLICK GITHUB ACTION RUNS, CLICK BUILD
       SHOW BUILD AND DEPLOY – EXPLAIN GITHUB ACTIONS STEPS – GO BACK TO PORTAL – SHOW OTHER CUSTOMIZING OPTIONS – OPEN WEBSITE FROM URL – SHOW WEBSITE. 

5. DEMO THREE

   1. open vscode
   2. `git pull` in terminal to update the repo with the new github workflow file.
   2. go to `content/news.md`
   3. Copy and paste a new "Loren Ipsum" block
   4. Save file and then run `hugo` in root of repo
   5. Just commit change to master - explain typical workflow includes branch/PR
   6. go to actions, show triggered build
   7. return to deck, finish session.

