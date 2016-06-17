# HeroGS
HeroGS is a tool that helps you to produce your grid system in simple ways.

<svg xmlns="http://www.w3.org/2000/svg" width="58" height="101" viewBox="0 0 58 101">
  <path fill="#000000" fill-rule="evenodd" d="M28.307,32.211 C11.512,51.236 0.368,62.895 0.368,62.895 L14.768,65.292 L28.307,32.211 Z M56.764,43.634 C55.7,42.495 53.909,42.433 52.767,43.502 L46.377,49.469 L46.824,39.851 C46.894,38.29 45.687,36.966 44.129,36.894 C43.863,36.883 43.603,36.913 43.358,36.969 L35.375,33.979 L36.96,29.659 C37.54,31.506 38.862,33.116 40.755,34 C44.335,35.684 48.604,34.139 50.285,30.558 C51.966,26.977 50.425,22.71 46.841,21.028 C44.544,19.952 41.97,20.199 39.973,21.457 L46.11,4.723 C46.652,3.257 45.896,1.631 44.431,1.094 C42.963,0.556 41.337,1.307 40.801,2.773 L29.25,34.256 C29.232,34.306 29.215,34.358 29.202,34.408 L19.223,58.262 L19.259,58.283 C19.146,58.488 19.043,58.697 18.961,58.924 L5.895,95.239 C5.103,97.447 6.248,99.878 8.454,100.666 C8.927,100.84 9.412,100.92 9.889,100.92 C11.628,100.92 13.258,99.842 13.882,98.111 L26.823,62.135 L29.788,63.644 L23.146,75.021 C21.962,77.042 22.646,79.643 24.668,80.826 C25.341,81.219 26.077,81.404 26.801,81.404 C28.262,81.404 29.681,80.65 30.47,79.301 L40.104,62.805 C41.287,60.783 40.602,58.183 38.581,57.002 C38.265,56.815 37.932,56.684 37.594,56.588 L40.692,49.992 L40.408,56.149 C40.354,57.298 41.006,58.365 42.046,58.847 C42.426,59.021 42.833,59.108 43.232,59.108 C43.935,59.108 44.629,58.847 45.165,58.346 L56.63,47.63 C57.771,46.565 57.829,44.776 56.764,43.634 Z"/>
</svg>

## Inspired of amazing packages
- [flexiblegs-scss](https://github.com/flexiblegs/flexiblegs-scss) - Flexible Grid System Scss.
- [bootstrap-sass](https://github.com/twbs/bootstrap-sass) - Official Sass port of Bootstrap 2 and 3.

## Example
```sass
.grid {
  @include gs(wrap); // init wrapper
  @include gs(gutter, -30); // use negative value for setting gutter for wrapper
}
.grid__col {
  @include gs(col); // init column
  @include gs(gutter, 30); // use positive value for setting gutter for columns
  @media (min-width: 768px){
    @include gs(col, 1, 4); // set width for tablet devices and upper
  }
}
```

## Working with Gulp
- `cd path/to/HeroGS` Go to the project directory
- `npm install` Install npm dependencies
- `gulp` Connect to the server, build examples and watch for changes

then open [localhost:8080](http://localhost:8080) from your browser

## Browser support
IE8+ - Because [IE8 is back from the dead](http://www.webdesignerdepot.com/2016/01/ie8-is-back-from-the-dead/)

## Credits
- [Superhero by Moriah Rich from the Noun Project](https://thenounproject.com/search/?q=hero&i=12709)

## TODO
- [ ] Examples
- [ ] Masonry layout metodology
- [ ] Flexbox support for modern browsers
- [ ] Feature polyfills for old browsers
