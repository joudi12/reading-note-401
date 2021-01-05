# summery 
![image](https://res.cloudinary.com/practicaldev/image/fetch/s--eANtDxQ_--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/i/nbr70hzcog75k41e8gio.png)
### Django ships with a built-in User model for authentication, however the official Django documentation highly recommends using a custom user model for new projects. The reason is if you want to make any changes to the User model down the road--for example adding a date of birth field--using a custom user model from the beginning makes this quite easy. But if you do not, updating the default User model in an existing Django project is very, very challengin


## AbstractUser vs AbstractBaseUser
### There are two modern ways to create a custom user model in Django: AbstractUser and AbstractBaseUser. In both cases we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work. Seriously, don't mess with it unless you really know what you're doing. And if you did, you wouldn't be reading this tutorial, would you?
1. AbstractUser: Use this option if you are happy with the existing fields on the User model and just want to remove the username field.
2. AbstractBaseUser: Use this option if you want to start from scratch by creating your own, completely new User model.
### The steps are the same for each:

1. Create a custom User model and Manager
2. Update settings.py
3. Customize the UserCreationForm and UserChangeForm forms
4. Update the admin
### We'll use AbstractUser which actually subclasses AbstractBaseUser but provides more default configuration.
## Custom User Model
### reating our initial custom user model requires four steps:

- update config/settings.py

- create a new CustomUser model

- create new UserCreation and UserChangeForm

- update the admin

### In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model. We'll call our custom user model CustomUser.

### Within INSTALLED_APPS add accounts at the bottom. Then at the bottom of the entire file, add the AUTH_USER_MODEL config.





