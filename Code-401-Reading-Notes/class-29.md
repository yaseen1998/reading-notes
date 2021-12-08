# class_29
## Django Custom User
Creating our initial custom user model requires four steps:

* update config/settings.py
* create a new CustomUser model
* create new UserCreation and UserChangeForm
* update the admin

In settings.py we'll add the accounts app and use the AUTH_USER_MODEL config to tell Django to use our new custom user model in place of the built-in User model.
<br>

<img src='https://miro.medium.com/max/505/1*ZmWcb9ynmt9ENZIt3UWi2Q.png'/>

<br>
### Create User
We need new versions of two form methods that receive heavy use working with users. Stop the local server with Control+c and create a new file in the accounts app called forms.py.
<br>
<img src='https://i.stack.imgur.com/2gFZV.jpg' />

### User Admin 
Finally we update admin.py since the Admin is highly coupled to the default User model.<br>
          
class CustomUserAdmin(UserAdmin):<br>
    add_form = CustomUserCreationForm<br>
    form = CustomUserChangeForm<br>
    model = CustomUser<br>
    list_display = ['email', 'username',]<br>

admin.site.register(CustomUser, CustomUserAdmin) <br>         

### super User
It's helpful to create a superuser that we can use to log in to the admin and test out log in/log out. On the command line type the following command and go through the prompts.
<br>
(accounts) $ python manage.py createsuperuser

## DjangoX
### install & Setup
poetry add djangox

# Run Migrations
(djangox) $ python manage.py migrate

# Create a Superuser
(djangox) $ python manage.py createsuperuser

# Confirm everything is working:
(djangox) $ python manage.py runserver

# Load the site at http://127.0.0.1:8000
