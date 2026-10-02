# Changing a password

From the SimpliCollect home page, you can change your password:

![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20210315-171216.png){ width=272 }

1.  Click Password.

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20210315-171047.png){ width=272 }

2.  Enter your new password.

3.  Enter your new password a second time to confirm that you entered it correctly.

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20210315-171252.png){ width=272 }

4.  Click Apply.

5.  The application returns to the Home screen once the new password has been saved.

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20210315-171328.png){ width=272 }

6.  A message appears if the passwords are not identical.

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20210315-171359.png){ width=272 }

## Resetting a lost password

If a user has lost their password, including the **admin** account, and it must be reset, you must open a session on Windows or Linux.

### Procedure in Windows

1.  Open a session on the gateway (see the procedure at the following link: Session Windows 10 )

2.  In Windows, click the "magnifying glass" in the lower left corner and type the command **cmd** to open a command window

3.  At the prompt, type the command **\SCollect\WEB\SITE\StartVENV.bat** to open the development environment

4.  Type the command **cd \SCollect\WEB\SITE\\**

5.  Type the command **python manage.py changepassword "user name"**, for example

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20211107-174133.png){ width=306 }

6.  The system asks you to enter the new password and to repeat it

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20211107-174258.png){ width=306 }

7.  The password is now changed

### Procedure for Linux

1.  Open a session on the gateway (see the procedure at the following link: (Confluence page not migrated) )

2.  At the prompt, type the command **source /scollect/venv/bin/activate** to open the development environment

3.  Type the command **cd /scollect/site/scollect**

4.  Type the command **python manage.py changepassword "user name"**, for example

5.  ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20211107-175102.png){ width=788 }

    The system asks you to enter the new password and to repeat it

    ![Screenshot](../../assets-en/changement-de-mot-de-passe/image-20211107-175154.png){ width=784 }

6.  The password is now changed
