# CBAR Design Tokens

Community BuildAR supports the [Design System Package (DSP)](https://github.com/AdobeXD/design-system-package-dsp) for importing and exporting CBAR Design Tokens, currently based on the [Material Design Tokens](http://m3.material.io/foundations/design-tokens/overview). DSP can be used in designer and developer workflow tools. 

Unfortunately the DSP doesn't currently cover the full design system, so take a look under the css directory for a theme that has the broader list of css variables that can be used in a web environment.

That being said, let’s dive into how you can use CBAR Design Tokens (DSP) within the [VSCode extension](https://marketplace.visualstudio.com/items?itemName=Adobe.xd) to generate code.


## Getting Started

Make sure you have the latest version of VSCode installed on your machine. VSCode is free to download and is open source.

[Download VSCode](https://code.visualstudio.com/)

After VSCode is installed, navigate to the marketplace on the extensions tab and search for Adobe.

![alt_text](/assets/image9.png)

[Download Adobe XD VSCode extension](https://marketplace.visualstudio.com/items?itemName=Adobe.xd)

Click on install and you may have to reopen or reload VSCode. After the extension is successfully installed, you can open Adobe XD by searching for Adobe in the command palette or clicking the “XD” icon in the bottom right.

![alt_text](/assets/image13.png)


After the plugin opens it should look like the following screenshot.

![alt_text](/assets/image2.png)

## Opening a DSP

Download default CBAR Theme values from [this repo](https://code.communitybuildar.com/community-buildar/cbar-design-tokens) and save it to your computer.

Open up the folder in VSCode by either dragging it onto the open window or selecting “Open Folder”.

![alt_text](/assets/image7.png)

Open the Adobe XD plugin and select “Edit Package” on the bottom left, then select “Select Folder”. There should be a notification on the bottom left that should say “Existing package found…” and click on “Open”.

![alt_text](/assets/image5.png)


## Exploring the DSP

With the DSP opened in the plugin you should see the following screenshot.

![alt_text](/assets/image10.png)


The CBAR Design Tokens (DSP) is made up of a few sections (Light, Dark, Default, Palette, Typography).

## Generating Code

After inspecting the DSP you can generate code in the form of tokens to be used in your application.

Select “Start Editing” and then “Finish Editing” to trigger code generation. If it is the first time you are doing it there will be a notification to install Style Dictionary.

![alt_text](/assets/image1.png)


Select “Install” then you will see another notification asking to export tokens.

![alt_text](/assets/image8.png)


Select “Export tokens” then you will see a notification asking you to open the folder.

![alt_text](/assets/image3.png)


Opening the folder you will see the following sub directories.

![alt_text](/assets/image11.png)

This directory is located in the current directory under a newly generated folder “dist”.

![alt_text](/assets/image4.png)


Opening up the “variables.css” for example you will see the following flat list of tokens used to theme your application.

![alt_text](/assets/image6.png)


The “android/colors.xml” should look similar.

![alt_text](/assets/image12.png)


Using the CBAR Design Tokens (DSP) will ensure your styles are shared throughout your designer and developer workflow. 

Learn more about the [Material Design Tokens](http://m3.material.io/foundations/design-tokens/overview) that we used as our base.
