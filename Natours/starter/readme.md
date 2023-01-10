## devleopment process 
- watch compile sass file 
node-sass inputFile.scss outputFile.css -w
- run life server 
live-server
- start
npm-run-all tasksName spreated by comma
install npm run-all to run all above script together at the same time

## build process 
- compile sass to css
node-sass inputFile.scss outputFile.css 
- concat css files npm i concat
concat -o outputFileName.css inputFile1.css inputFile2.css
- add auto prefix to css npm i install postcss-cli
postcss --use autoprefixer -b 'last 10 versions' inputfileName.css -o outputFile.css
- compress css file
node-sass inputFile.css outputFile.css --output-style compressed
here we use the same packge for compile and watch sass files
- bulid >> run all the above steps in sequence by npm-run-all packge
npm-run-all tasksName spreated by comma

## important note
 this line of code should be in the htnl file at head;
  responsive web design does not work with this line,
  this line say our website should be rendered with width of the device
  width of the content should be the device content
<meta name="viewport" content="width=device-width, initial-scale=1.0" />

## selectors in css
- select the adjecent element 
for example : some time we need to select element when other element is focus or in other events like here
```
<form action="" class="search">
          <input type="text" class="search__input" placeholder="Search hotels" />
          <button class="search__button">
            <svg class="search__icon">
              <use xlink:href="img/sprite.svg#icon-magnifying-glass"></use>
            </svg>
          </button>
</form>
```
here when the input is focus we want to change the background color for the button
```
.search__input:focus + .search__button {
    background-color:red;
}
```
