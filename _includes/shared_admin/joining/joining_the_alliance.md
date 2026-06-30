# Joining the Alliance

Joining the OntoPortal Alliance means setting up and operating your own portal based on the OntoPortal technology. This section describes the steps involved from installing your own instance, to customizing it and self-declaring your portal on the OntoPortal website so it appears alongside the other portals of the Alliance.

## 0. Install OntoPortal

Before customizing your portal, you first need to install your own instance of OntoPortal. See the [Installation Steps]({{site.baseurl}}/administration-guide/steps/) section for detailed instructions.

## 1. Setup your GitHub environment

Deploying a customized version of OntoPortal — with the same functionalities but with your own look and feel, name, footer, etc., and served at your own specific URL — requires modifying the code's configuration files and re-deploying your own version of the code. This therefore has to be done at least once manually, or by setting up a CI/CD pipeline to automate the build and deployment of your portal.

For this reason, we ask that your code repositories be, whenever possible, **forks of the upstream OntoPortal repositories**. This makes it easier for you to pull in updates and to contribute your changes back to the Alliance. At a minimum, you need to fork the following two repositories:

* <https://github.com/ontoportal/ontoportal_web_ui>
* <https://github.com/ontoportal/ontologies_api>
  * Make sure you fork the **agroportal** branch as well.

## 2. Portal Appearance Customization

### 2.1 Choose colors for the portal 

We need 4 colors for the portal:

1. Primary color
2. Hover color
3. Secondary color
4. Light color

 ![](https://wiki.agroportal.eu/api/files.get?sig=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJrZXkiOiJ1cGxvYWRzLzVmNTFjMmUyLTZlMDMtNGQzZS04ZWNiLTE2NzJkYTcxN2ZmYi85MDhlNTRiZS1mMGEyLTQzNmYtOTczNy1jMjhiNDg4N2NiMDYvU2NyZWVuc2hvdCAyMDI2LTA2LTA5IGF0IDEyLjAxLjAzLnBuZyIsInR5cGUiOiJhdHRhY2htZW50IiwiaWF0IjoxNzgyODM4MTUxLCJleHAiOjE3ODM0NDI5NTF9.YylvG_Rr_onSm_5gfD2zNpJezl7YtL0Wnd-CI3uwPyI " =431x400")

Then we change them here:

<https://github.com/ontoportal/ontoportal_web_ui/blob/master/app/assets/stylesheets/theme-variables.scss.erb>

### 2.2 Choose the logos to display in the homepage 

* choosing the logos to display and upload them to <https://github.com/ontoportal/ontoportal_web_ui/tree/master/app/assets/images>

 ![](https://wiki.agroportal.eu/api/files.get?sig=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJrZXkiOiJ1cGxvYWRzLzVmNTFjMmUyLTZlMDMtNGQzZS04ZWNiLTE2NzJkYTcxN2ZmYi8xNDlkYTNhNi03ZDIxLTQ0MjItOGYyNS00NmZjMzc4ZmU0NTcvU2NyZWVuc2hvdCAyMDI2LTA2LTA5IGF0IDExLjMzLjEyLnBuZyIsInR5cGUiOiJhdHRhY2htZW50IiwiaWF0IjoxNzgyODM4MTUxLCJleHAiOjE3ODM0NDI5NTF9.SdzqzntEquH_KXkSqeVI6UAhWj0JxtBab8uPuVcj5f0 " =1199x202")

### 2.3  Modify the config file

<https://github.com/ontoportal/ontoportal_web_ui/blob/master/config/bioportal_config_env.rb.sample>

## 3. Portal Text Customization

The portal text is internationalized, and all changes must be added to these YAML files

* <https://github.com/ontoportal/ontoportal_web_ui/blob/master/config/locales/en.yml>
* <https://github.com/ontoportal/ontoportal_web_ui/blob/master/config/locales/fr.yml>

## 4. Add yourself to the Alliance Poster

* Add your logo to the alliance poster here : <https://www.figma.com/design/n2tOIfgVlVvFAr3F00Ab5m/Ontoportal-alliance?node-id=0-1&t=xwBAXIAKOH2QTQSf-1>
* Make a PR to: <https://github.com/ontoportal/website>

* To be displayed here: <https://ontoportal.org/about/>

## 5. Setup Google reCAPTCHA

* <https://www.google.com/recaptcha/admin/create>
