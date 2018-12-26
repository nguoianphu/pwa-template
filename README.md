# pwa-template
For setting up manifest.json, go to https://app-manifest.firebaseapp.com/ to generate manifest.json
  * "start_url": "/project-name/",
  * We don't need to set "scope" : '/'
### In sw.js, we need to modify these places:
  * const cacheName = 'project-name-v1.0'
  * navigator.serviceWorker.register('/project-name/sw.js', {scope: '/project-name/'})
  * Since we use cache with network update strategy, we don't need to manually add files to fileToCache array, just leave filesToCache = ['/project-name/index.html'], and Service Worker will automatically install all of the rest files to cache
  
  
