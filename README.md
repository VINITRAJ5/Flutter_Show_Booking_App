# Screenshot of This App Below <h1>

## This is the Main Screen of App <h2>
   
<img src="https://github.com/VINITRAJ5/Meals_App/blob/master/ScreenShots/1%20(1).jpg" width="280">

 1. it have favourite icon choose your Favourite
   1. and has Categories Of different Types of food
   
  ## This is the Drawer Section of App <h2> 
   This Screen Contain Information of Following

> 1.  2 button for 2 Screen
   
<img src="https://github.com/VINITRAJ5/Meals_App/blob/master/ScreenShots/1%20(2).jpg" width="280">

 *Filter in form of toggle button for Different Categories*   
   
<img src="https://github.com/VINITRAJ5/Meals_App/blob/master/ScreenShots/1%20(3).jpg" width="200">
   
  ## This is the Detail Page Of Food <h2>
   **You can Add New see Whole List of same Categories**

<img src="https://github.com/VINITRAJ5/Meals_App/blob/master/ScreenShots/1%20(4).jpg" width="280">

 ## This is the Detail Page Of  Single Food <h2>
    This Screen Contain Information of Following
> 1.  Required Food Ingredients
   >> 2. Steps For Making that food
   
<img src="https://github.com/VINITRAJ5/Meals_App/blob/master/ScreenShots/1%20(5).jpg" width="280">

 
 For Installation of this App 
   Clone The code and or Download ZIP File
   then Run first this command in your editor terminal `flutter pub get` then  `flutter run`
   
### Snippets Of `main.dart`
 
  ```
   class MyApp extends StatefulWidget {
  @override
  _MyAppState createState() => _MyAppState();
}

class _MyAppState extends State<MyApp> {
  Map<String, bool> _filters = {
    'gluten': false,
    'lactose': false,
    'vegan': false,
    'vegetarian': false,
  };
  List<Meal> _availableMeals = DUMMY_MEALS;
  List<Meal> _favoriteMeals = [];

  void _setFilters(Map<String, bool> filterData) {
    setState(() {
      _filters = filterData;

      _availableMeals = DUMMY_MEALS.where((meal) {
        if (_filters['gluten'] && !meal.isGlutenFree) {
          return false;
        }
        if (_filters['lactose'] && !meal.isLactoseFree) {
          return false;
        }
  
```
  
  IF you get issue or error  create a issue, i'll Love to help
   
