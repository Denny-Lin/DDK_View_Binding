# DDK_View_Binding
View Binding in Android

# Set build.gradle to enable View Binding
View Binding is enabled by default after we created a project. </br>
However, we can disable it to see what is going on.</br>

### Enable
![Screen Shot 2022-05-22 at 8 20 19 PM](https://user-images.githubusercontent.com/67073582/169694810-7408b89b-57db-486a-9bbc-2cbda3e36ca7.png)

### Disable
![Screen Shot 2022-05-24 at 11 25 43 PM](https://user-images.githubusercontent.com/67073582/170073743-b1367824-32f9-451e-b2cc-b49ff15d1719.png)

# View Binding

```Java
import com.example.mynativeandroidapp.databinding.ActivityMainBinding;

private ActivityMainBinding binding;

binding = ActivityMainBinding.inflate(getLayoutInflater());
setContentView(binding.getRoot());
TextView tv = binding.sampleText;
```
This object of ActivityMainBinding is from the file name of activity_main.xml. </br>
So if we have a xml called result_profile.xml, we can do "import com.example.mynativeandroidapp.databinding.ResultProfileBinding;". </br>
And then create an object for this xml, such as "private ResultProfileBinding binding2;" </br>

![Screen Shot 2022-05-24 at 11 52 31 PM](https://user-images.githubusercontent.com/67073582/170079072-e59c7dfa-df9a-4b7a-9b9a-a70a70fcd6aa.png)

Every binding class, such as ActivityMainBinding and ResultProfileBinding, has infate() and getRoot() method. </br>
inflate() is static, so we can call it directly. </br>
And assign the return value from inflate() to binding. </br>
It could be "ActivityMainBinding binding = ActivityMainBinding.inflate(getLayoutInflater());". </br>
Now we can use binding.getRoot() to get the "root view". </br>
The root view of activity_main.xml here we used is ConstraintLayout. </br>
Otherwise, we also have other choices below. </br>

![Screen Shot 2022-05-25 at 11 43 59 PM](https://user-images.githubusercontent.com/67073582/170303512-944a732e-3bba-44b8-81c6-b8284403a534.png)

For exampe, we have a TextView in activity_main.xml, id called sample_text, so we can use "TextView tv = binding.sampleText;". </br> 
And then do what we want. </br>
It is simillar to findViewById. </br>

![Screen Shot 2022-05-22 at 8 18 21 PM](https://user-images.githubusercontent.com/67073582/169694747-79ea278e-340d-44cc-ac3f-859c9336e7a1.png)


... </br>
![Screen Shot 2022-05-22 at 8 30 37 PM](https://user-images.githubusercontent.com/67073582/169695348-bac2eb88-4ee1-4538-9bf6-399475be01cd.png)


# References
1. https://developer.android.com/topic/libraries/view-binding
