# Disable-View_page_source_code

When you put a lot of effort into creating a portfolio website, watch the demo live. The code of this website cannot be taken by anyone by looking at the "view source code". So you can turn off "ctrl + u" or f12 if you want. For that you can use the following script ( js )  in my mail file (HTML).

// f12 disble 
document.onkeypress = function (event) {
    event = (event || window.event);
    if (event.keyCode == 123) {
    return false;
    }
    }
    document.onmousedown = function (event) {
    event = (event || window.event);
    if (event.keyCode == 123) {
    return false;
    }
    }
    document.onkeydown = function (event) {
    event = (event || window.event);
    if (event.keyCode == 123) {
    return false;
    }
    }
// ctrl + u 
document.onkeydown = function(e) {
    if (e.ctrlKey && (e.keyCode === 67 || e.keyCode === 86 || e.keyCode === 85 || e.keyCode === 117)) {//Alt+c, Alt+v will also be disabled sadly.
        alert('not allowed');
    }
    return false;
};

For Demo https://serene-manatee-e12a3c.netlify.app/
