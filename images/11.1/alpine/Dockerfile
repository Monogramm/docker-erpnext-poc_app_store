FROM monogramm/docker-erpnext:11-alpine

LABEL maintainer="Monogramm Maintainers <opensource at monogramm dot io>"

### For public repository > Start ###

RUN set -ex; \
    bench get-app --branch master https://github.com/AminovE99/erpnext_app_store

### For public repository > End ###


### For private repository > Start ###
#
#### get git password from docker build argument or use default
##### this is not the best practice to put password in dockerfile
##### so please be super careful with your code and docker-image
##### PLEASE MAKE SURE YOUR REPOSITORY IN BOTH GITHUB AND DOCKERHUB IS SET TO PRIVATE
#ARG git_password=
#
#### install expect (used to run private install script)
#### run install script
#RUN set -ex; \
#    sync && /home/$FRAPPE_USER/install_private_app.sh \
#        $git_password \
#        your_app_name \
#        https://github.com/your_account/your_repository \
#        your_git_branch \
#    ;
#
### For private repository > End ###
