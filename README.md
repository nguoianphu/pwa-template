# pwa-template
### For setting up manifest.json, go to https://app-manifest.firebaseapp.com/ to generate manifest.json
  * "start_url": "/project-name/",
  * Add "description" and delete "scope", because we don't need to set "scope"
### In sw.js, we need to modify these places:
  * Change all 'project-name' variables to our project/folder name,
  * We don't need to manually add files to cache, simply leave filesToCache = ['/project-name/index.html']
  
