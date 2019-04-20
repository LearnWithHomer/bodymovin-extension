# bodymovin-extension
Bodymovin UI extension panel

## Getting Started

You will need to locate the CEP extensions folder on your machine. On Windows, this is typically located at `C:\Program Files (x86)\Common Files\Adobe\CEP\extensions\` and on Mac it is typically located at /Library/Application Support/Adobe/CEP/extensions. Create a folder there called com.bodymovin-homer.bodymovin-homer.

You will need to adjust your registry so that Adobe knows you are attempting to debug an extension. [This link](https://github.com/Adobe-CEP/Getting-Started-guides/tree/master/Client-side%20Debugging#set-the-debug-mode) covers how to do that. Please note that as of this writing, the link is out of date. You will need to replace CSXS.8 with CSXS.9 in those instructions.

Copy the .env.sample file into this same directory as .env. Then paste the location to the CEP extension folder after `EXTENSION_DESTINATION=` with no quotes.

You should be ready to start development now. Go ahead and run `npm run start-dev` in a terminal. If you have After Effects open, please restart it. Go to Window > Extensions > Bodymovin-Homer and click it. You should see the extension. If you make any changes in the src directory, you should see the window refresh and those changes appear live.
