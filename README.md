# javascript-search-plugin
It is a javascript plugin which can filter html table rows according to user input.
### Usage
* Add textbox in your html file
```
<input type="search" style="width:15%;" placeholder="Search...." id="txt_search" />
```
* Inside window load event or document ready event (if you are using jQuery) add below code
    * In javascript :-
      ```
        window.onload = function(){
          var searchBox = document.getElementById("txt_search");
          searchBox.addEventListener("input",function(){
            tableSearch("tableId",document.getElementById("txt_search").value,"No match found");
          });
        }
      ```
    * In jQuery :- 
      ```
        $(document).ready(function(){
          var searchBox = document.getElementById("txt_search");
          searchBox.addEventListener("input",function(){
            tableSearch("tableId",document.getElementById("txt_search").value,"No match found");
          });
        });
      ```
 * In above code you can pass both table id or table class. When you pass table class it will work on multiple html tables.     
 ## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details

## Acknowledgments
 * The sample data in html table is generated using https://www.generatedata.com/
