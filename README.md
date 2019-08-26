# Two Factor Authentication
Purpose of this plugin is to add an extra security layer for your Liferay Portal. In addition to username and password, user requires to enter a one-time verification code (Google Authenticator), when signing in to Liferay Portal.

## Environment
1. Liferay 7.0 DXP 
2. Liferay 7.0 CE-GA5
3. Liferay 7.1 CE-GA1
4. Liferay 7.1 CE-GA2
5. Liferay 7.1 CE-GA3

### Features:
* Enable or disable Two factor authentication.
* Recovery option, useful if user lost security code.
* Security code is stored as encrypted.

## How to use
1. Download and install Two factor authentication plugin on your server. Make sure plugin is properly deployed on server.
2. Create public page name as configuration.
![01_create_public_page](https://user-images.githubusercontent.com/27973508/63684132-cb2d6c00-c819-11e9-931c-22cdd6ec9a99.JPG)
![02_configure_page](https://user-images.githubusercontent.com/27973508/63684133-cb2d6c00-c819-11e9-9759-66a51fca6807.jpg)
3. Put Two Factor Config portlet on configuration page.
![03_put_config](https://user-images.githubusercontent.com/27973508/63684138-cc5e9900-c819-11e9-99e2-0f1a7dfabf41.jpg)
4. You can set page permission as you want, so that only intended user can have access to this feature.
5. Create another public page name as verify-otp.
![04_verify_page](https://user-images.githubusercontent.com/27973508/63684137-cbc60280-c819-11e9-9457-a6ad433bf6e2.jpg)
	- **Note**:  This page name must be 'verify-otp' and make sure you turned ON "Hide from Navigation Menu"
6. Put Two Factor Verify portlet on verify-otp page.
![05_put_verify](https://user-images.githubusercontent.com/27973508/63684131-ca94d580-c819-11e9-9fc8-6cda23da6cd0.jpg)
7. Set permission of page "verify-opt" in such a way that it should only be accessible after login.
8. To enable/disable Two Factor authentication user has to enable this feature using below screen.
![06_user_configuration](https://user-images.githubusercontent.com/27973508/63690276-d4bed000-c829-11e9-9b3a-5c5ead01f3e6.jpg)
9. Once user enable this feature and after providing correct username/password portal should ask for verification code as shown below. 
![07_verify_otp_page](https://user-images.githubusercontent.com/27973508/63687136-66760f80-c821-11e9-8498-787389cabba8.JPG)
