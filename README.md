# pwa-template
For setting up manifest.json, go to https://app-manifest.firebaseapp.com/ to generate manifest.json
  * "start_url": "/project-name/",
### In sw.js, we need to modify these places:
  * Change cacheName variable to project name
  * navigator.serviceWorker.register('/project-name/sw.js', {scope: '/project-name/'})
Since we use cache with network update strategy, we don't need to manually add files to fileToCache array, because Service Worker will automatically install files to cache
  
  
