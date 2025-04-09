# Step 2: Attach Build to Production

## Overview:
In this step, When deploying a React application to Azure Web App, I'm not pushing your raw source code, but pushing the final, production-ready version of the site. That’s what the build/ folder is for.

### Steps:
1. **Web App Overview**:
   - After the Web App is created, automatically the overview page is loaded
   - Go to `Search` > `Advanced Tools` > `Go`.
2. **Paste Build Folder**:
   - At the top, click `Dubug Console`, `CMD`.
   - Click `Site` folder, `wwwroot`.
   - Delete any files in the folder.
   - Go to `Build` folder and copy the contents, paste in the `wwwroot` folder.
