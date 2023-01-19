# Server settings on `/data`
Clone this directory on a `/data` disk.

# Directory usage
- `batches` : contains all batches for starting, stopping and operating the GEN server,
- `code` : contains the current build codes (`/code/initial`) and their previous versions (`/code/versions`). The build code name has the following format <github commit code>.tar.gz
- `mongo` : contains the following directories
	- `/mongo/gen_dev/data` : not pushed in git : contains the data base data.
-	`nginx`
-	`static` : symbolic link for static file done on `start` : `sudo ln /media/francois/DATA/data/static/ static -s`

# How to :
## Start the GEN server
## Start the GEN server
## To dump Mongo DB
Use the batch `sudo sh gen_dev_MongoDump` or `sudo sh gen_prod_mongoDump`. The dump of of the GEN_DEV or GEN_PROD database will be under `server_settings/mongo/gen_dev/dump/<timestamp>/gen_dev/` or `server_settings/mongo/gen_prod/dump/<timestamp>/gen_prod/`
## Reload the mongo DEV or PROD server

# To do

- NGINX : reroute vers specific page when server not available
- add mongoRestore from initialWindowsData for dev
- add automatic/manual mongo backup

