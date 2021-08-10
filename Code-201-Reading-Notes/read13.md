# LOCAL STORAGE
The localStorage and sessionStorage properties allow to save key/value pairs in a web browser<br>.

The localStorage object stores data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.<br>

The localStorage property is read-only<br>

check for HTML5 Storage<br>
function supports_html5_storage() {<br>
  try {<br>
    return 'localStorage' in window && window['localStorage'] !== null;<br>
  } catch (e) {<br>
    return false;<br>
  }
}


#### you can use Modernizr to detect support for HTML5 Storage.

if (Modernizr.localstorage) {<br>
  // window.localStorage is available!
} else {<br>
  // no native support for HTML5 storage :(<br>
  // maybe try dojox.storage or a third-party solution<br>
}

<img src = "https://res.cloudinary.com/practicaldev/image/fetch/s--rSskJpsi--/c_imagga_scale,f_auto,fl_progressive,h_900,q_auto,w_1600/https://dev-to-uploads.s3.amazonaws.com/i/2imjutnczd4f3jdhgbdx.png">


### syntax
window.localStorage

### Syntax for SAVING data to localStorage:
 localStorage.setItem("key", "value");
 
### Syntax for READING data from localStorage:
var lastname = localStorage.getItem("key");

###Syntax for REMOVING data from localStorage:
localStorage.removeItem("key");

<img src = "https://www.tuto.dev/img/js_localstorage-og-linkedin.png">





