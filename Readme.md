Areas are added as JS object into array. 
{
    name: "Area Name",
    url: "link to http page about area",
    pos: "one of se,ne,nw,sw - position of text relatively to area marker, optional",
    symbol: '?',
    x:0, y:0  - optional, coords,
    location:'15 n, 10 e, 6 n', - dirs to area, optional. If area does not have x, y, dirs from cs are used to compute direction
}

Area placement is done using string functions. There are problems with that so areas a) have to be placed sorted by X, right side first, to correctly place markers. b) in some cases text overlaping might ocur, so use pos to change location of text. 
The browser console will show  computed coords for area, it is better to use fixed cords in long run, as computing dirs might have issues. 
