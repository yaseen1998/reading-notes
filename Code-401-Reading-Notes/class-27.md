# class_27
## Using Models 
### Model primer
#### Model definition
Models are usually defined in an application's models.py file. They are implemented as subclasses of django.db.models.Model, and can include fields, methods and metadata. <br>

<img src='https://d2gdtie5ivbdow.cloudfront.net/media/images/models.PNG'/>
     
**Fields**
    my_field_name = models.CharField(max_length=20, help_text='Enter field documentation')     <br>
A model can have an arbitrary number of fields, of any type — each one represents a column of data that we want to store in one of our database tables    

#### Common field arguments
The following common arguments can be used when declaring many/most of the different field types:

* help_text: Provides a text label for HTML forms (e.g. in the admin site), as described above.
* verbose_name: A human-readable name for the field used in field labels. If not specified, Django will infer the default verbose name from the field name.
* default: The default value for the field. This can be a value or a callable object, in which case the object will be called every time a new record is created.
* null: If True, Django will store blank values as NULL in the database for fields where this is appropriate (a CharField will instead store an empty string). The default is False.
* blank: If True, the field is allowed to be blank in your forms. The default is False, which means that Django's form validation will force you to enter a value. This is often used with null=True , because if you're going to allow blank values, you also want the database to be able to represent them appropriately.
* choices: A group of choices for this field. If this is provided, the default corresponding form widget will be a select box with these choices instead of the standard text field.
* primary_key: If True, sets the current field as the primary key for the model (A primary key is a special database column designated to uniquely identify all the different table records). If no field is specified as the primary key then Django will automatically add a field for this purpose.


#### Common field types
* CharField
* TextField 
* IntegerField
* DataField
* EmailField
* Filefield
* AutoField


#### metadata in django
You can declare model-level metadata for your Model by declaring class Meta<br>
ne of the most useful features of this metadata is to control the default ordering of records returned when you query the model type. You do this by specifying the match order in a list of field names to the ordering attribute, as shown above
