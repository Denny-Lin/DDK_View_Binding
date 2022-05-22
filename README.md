# DDK_View_Binding
View Binding in Android

# View Binding

```Java
import com.example.mynativeandroidapp.databinding.ActivityMainBinding;

private ActivityMainBinding binding;

binding = ActivityMainBinding.inflate(getLayoutInflater());
setContentView(binding.getRoot());
TextView tv = binding.sampleText;
```
...
![Screen Shot 2022-05-22 at 8 18 21 PM](https://user-images.githubusercontent.com/67073582/169694747-79ea278e-340d-44cc-ac3f-859c9336e7a1.png)

...
![Screen Shot 2022-05-22 at 8 20 19 PM](https://user-images.githubusercontent.com/67073582/169694810-7408b89b-57db-486a-9bbc-2cbda3e36ca7.png)


# References
1. https://developer.android.com/topic/libraries/view-binding
