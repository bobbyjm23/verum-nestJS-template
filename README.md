![App Screenshot](https://verum.nz/wp-content/uploads/2021/03/Verum-logo-dark.svg)


### *****Templating Note******
Please Remove this section on initial commit once setup

Files that will need to be modified for the template with project specific content

package.json

    * NAME
    * DESCRIPTION
    * REPO URL
    * NODE_VERSION (If different to NVMRC)

sync_variables.json

webpack.mix.js  

.nvmrc
 

# PROJECT_NAME 

Description of the tech stack and any plugins / gotchas that a developer may need to be aware of. Only a top level business logic reasoning here. 
Use the Developer's notes to articulate the technical implications and solution. 

Description of the site's functionality
Including additional repos and the basics as to how they interact. 
If other repos are required, please use those repos readmes to explain in detail the functionality.


### Links

 * Project - N/A
 * DNS - https://www.cloudflare.com/
 * Hosting - N/A
 * Local https://localhost:8080
 * UAT - N/A
 * Production - N/A


### Installation
 1. `git clone https://github.com/VerumDigital/path-to-project-name`
 2.  `git submodule update --init --recursive` Pull down the sync tool repo for use.
    Note because submodules are not pulled down on a standard clone you will need to run this additional command to pull down the sync tool 
 3. `docker compose up -d --build` you only need to run the --build flag if you either are setting up first time or have removed image.  
    We use docker volumes to add the appropriate .htaccess file. this can be modified and found the in the root directory of the repo.
 6. Copy ```.env-example``` -> ```.env ```
    Local development only uses the ```.env``` file.    

 ### JS / CSS Build tools
 * `nvm use` to switch to Node.js v20
 * `yarn`
 * `yarn run watch` to build & watch js/css,
 * `yarn run prod` to just compile assets
 * `yarn run dev` to compile uncompressed assets without watching

### Syncing the project with uploads and database. 

We use a sync tool contained as a submodule within all our wordpress repos. 
For details on how to use the tool please refer to the readme in the following repo. 

https://github.com/VerumDigital/verum-wordpress-sync-tool

# Developer's Note

Used to elaborate on a per repo basis any gotchas such as possibly a different 



