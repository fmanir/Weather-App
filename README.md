### `npm install`

Install all dependencies for the app including react-ios-pwa-prompt, which prompts the user to 'Add to Home Screen'. Full documentation and list of props can be found at https://www.npmjs.com/package/react-ios-pwa-prompt.

I am under the impression that Android devices already prompt a user to download a PWA so the library above is to tackle iOS devices.

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

Notes:

I've done very little with styling to keep the application simple.

If you run Lighthouse in Dev Tools, the app should achieve 100% (fingers crossed!).

App should remain responsive across all device types.

Prompt to 'Add to Home Screen' will only show on iOS devices and will only show once (as per the props set) so you will need to either, clear cache or use a private browser to show the prompt thereafter. Of course, you can also pass the timesToShow prop to <PWAPrompt/> to show this more than once. E.g. <PWAPrompt timesToShow={3}/>.

I have left some comments and console.log in to show what is happening.

If you use Dev Tools to 'go Offline' (or disconnect device from WiFi/network), you will be presented with an offline page. offline.html is an example of where we would put content we want to render when the application is offline.

If you would like me to add some styling to make it aesthetically pleasing, just let me know!