

For full details reference: http://designers.hubspot.com/docs/tools/local-hubl-server
(copied below)

----

Local HubL server
The Local HubL Server allows web developers that are comfortable with markup and the HubL templating language to build and test HubSpot COS templates locally. The server runs 100% locally with no external dependencies.  Once running, you will be able to build and test templates without loading templates into the HubSpot interface. 
This tool is designed for developers comfortable with (OS X, Windows, or Linux) shell commands, and requires installation of Java 8 (or later) development kit to run. Also note that this tool is only meant to allow rendering content locally. It does not connect to HubSpot or load files into the HubSpot system. However, it can be used in conjunction with FTP or stand alone.
Installation

Before following these instructions, please ensure that you have the Java 8 (or later) developers kit installed. Follow these steps to set up the Local HubL Server:

1. Download the package

Download the latest version of the package.
2. Unzip the package

Unzip the file. This will create a local-hubl-server directory. You can move this folder to a directory of your choosing.
3. Change directory

Open Terminal or Command Prompt and change directory to local-hubl-server. In Terminal the command is:

cd local-hubl-server
Please note that the path to the file will vary based on where you unzip and move the directory. Alternatively, you can navigate to the server folder via Finder or Windows Explorer.
4. Run the server

In Terminal or Command Prompt run the following command:

./bin/local-hubl-server
If you do not have the Java 8 Developers Kit installed, you will be prompted to download and install it. If successful the browser will open to 127.0.0.1:8080.

As an alternative, if you accessed the local-hubl-server directory via Finder or Windows Explorer, run the local-hubl-server executable in the 'bin' directory.

HubSpot Help article screenshot
5. Explore the default template content

List of templates
While running the server, the IP address 127.0.0.1:8080 will show you a list of templates that have been created in your working directory. The default distribution comes with a codified hubtheme to play with.

You can see that the 'conf/config.yaml' is set up to point at 'work/hubthemes/vast as a baseDir', which is where everything all of the default tempates live. If you wish to change the baseDir, you will need to edit the config.yaml file.

You may notice that the folder structure of the work/hubthemes/vast directory resembles the folder structure of Design Manager. When you create new HTML files, in your working directory, you will see them automatically added to the list of links available at 127.0.0.1:8080.
Local HubL Server + FTP

You can use the HubL Local Server with an FTP client to sync both the local and remote 'custom' directories. To learn more, check out this article.