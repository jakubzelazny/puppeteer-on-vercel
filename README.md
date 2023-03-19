# How to run Puppeteer on Vercel
This repo has Puppeteer code that works on Vercel and stays under 50 MB.
The older versions of Puppeteer and Chromium, specifically Chromium 92.0.0 and Puppeteer 10.0.0, were used to make this possible.
It runs on node.js v18.

The API endpoint (/api/run) starts the browser and grabs the title of https://vercel.com/.
Feel free to clone this repo.


Notice for MacOS M1 users: create a `.env` file and paste the following code into it.
`CHROME_EXECUTABLE_PATH="<path to chrome executable>"`
It's likely that the path is: `CHROME_EXECUTABLE_PATH="/Applications/Google Chrome.app/Contents/MacOS/Google Chrome"`.

To test it localy, run `vercel dev`.
Then go to `http://localhost:3000/api/run`.