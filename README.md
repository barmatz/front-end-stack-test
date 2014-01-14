# Front-end Stack Developer Test

> [HTML](#html)
>> [What is HTML5?](#what-is-html5)  
>> [What is a doctype?](#what-is-a-doctype)  
>> [What is the difference between standards mode and quirks mode?](#what-is-the-difference-between-standards-mode-and-quirks-mode)  
>> [What kind of issues might be when developing multilingual web pages?](#what-kind-of-issues-might-be-when-developing-multilingual-web-pages)  
>> [What is the difference between Canvas and SVG?](#what-is-the-difference-between-canvas-and-svg?)

> [CSS](#css)  
>> [How would you cause your page to render the same in all browsers/devices?](#how-would-you-cause-your-page-to-render-the-same-in-all-browsers-devices)  
>> [What is the difference between a reset and a normalize CSS file?](#what-is-the-difference-between-a-reset-and-a-normalize-css-file)  
>> [What is float?](#what-is-float)  
>> [What are the various clearing techniques?](#what-are-the-various-clearing-techniques)  
>> [What is a CSS sprite?](#what-is-a-css-sprite)  
>> [What is the difference between display:none and visibility:hidden?](#what-is-the-difference-between-display-none-and-visibility-hidden)  
>> [How would you implement non-standard fonts?](#how-would-you-implement-non-standard-fonts)  
>> [What is the box model?](#what-is-the-box-model)  
>> [What is the problem with the box model?](#what-is-the-problem-with-the-box-model)

> [JavaScript](#javascript)  
>> [What are global variables?](#what-are-global-variables)  
>> [When would you use global variables?](#when-would-you-use-global-variables)  
>> [What is the lifetime of variables?](#what-is-the-lifetime-of-variables)  
>> [What are data types and list existing ones in JavaScript?](#what-are-data-types-and-list-existing-ones-in-javascript)  
>> [What is the difference between undefined and null?](#what-is-the-difference-between-undefined-and-null)  
>> [What is a closure?](#what-is-a-closure)  
>> [What is a namespace?](#what-is-a-namespace)  
>> [Why would you use a namespace?](#why-would-you-use-a-namespace)  
>> [What is the difference between == and ===?](#what-is-the-difference-between-==-and-===)  
>> [What is event bubbling?](#what-is-event-bubbling)  
>> [What is event capturing?](#what-is-event-capturing)  
>> [Why would you use event bubbling/capturing?](#why-would-you-use-event-bubbling-capturing)  
>> [What is the difference between window.onclick, window.addEventListener(‘click’) and window.attachEvent(‘onclick’)?](#what-is-the-difference-between-window-onclick-window-addeventlistener-click-and-window-attachevent-onclick)  
>> [How do you handle errors?](#how-do-you-handle-errors)  
>> [Explain the following terms in object-oriented programming](#explain-the-following-terms-in-object-oriented-programming)  
>> [What type of inheritance does JavaScript implement?](#what-type-of-inheritance-does-javascript-implement)  
>> [What is the difference between cookies, sessionStorage and localStorage?](#what-is-the-difference-between-cookies-sessionstorage-and-localstorage)  
>> [What is this?](#what-is-this)  
>> [What is the difference between .call() and .apply()?](#what-is-the-difference-between-call-and-apply)  
>> [What does .bind() do?](#what-does-bind-do)  
>> [What is the same-origin policy?](#what-is-the-same-origin-policy)  
>> [What is the difference between AJAX and JSONP?](#what-is-the-difference-between-ajax-and-jsonp)  
>> [What are the issues with JSONP?](#what-are-the-issues-with-jsonp)  
>> [What solution is there to JSONP?](#what-solution-is-there-to-jsonp)  
>> [What is hoisting?](#what-is-hoisting)  
>> [Would you extend built in objects?](#would-you-extend-built-in-objects)  
>> [What is the difference between the document ready and load events?](#what-is-the-difference-between-the-document-ready-and-load-events)  
>> [What is “use strict”?](#what-is-use-strict)


## <a name="html"></a> HTML

### <a name="what-is-html5"></a> What is HTML5?
HTML5 is the latest evolution of the standard that defines HTML. The term represents two different concepts:  
It is a new version of the language HTML, with new elements, attributes, and behaviors, and a larger set of technologies that allows more diverse and powerful Web sites and applications. This set is sometimes called HTML5 & friends and often shortened to just HTML5.

### <a name="what-is-a-doctype"></a> What is a doctype?
A document type declaration, or DOCTYPE, is an instruction that associates a particular SGML or XML document (for example, a webpage) with a document type definition (DTD) (for example, the formal definition of a particular version of HTML). In the serialized form of the document, it manifests as a short string of markup that conforms to a particular syntax.  
The HTML layout engines in modern web browsers perform DOCTYPE "sniffing" or "switching", wherein the DOCTYPE in a document served as text/html determines a layout mode, such as "quirks mode" or "standards mode".  

### <a name="what-is-the-difference-between-standards-mode-and-quirks-mode"></a> What is the difference between standards mode and quirks mode?
In quirks mode, layout emulates nonstandard behavior in Navigator 4 and Internet Explorer 5 for Windows that is required not to break existing content on the Web. In standards mode, the behavior is (hopefully) the behavior described by the HTML and CSS specifications.  

### <a name="what-kind-of-issues-might-be-when-developing-multilingual-web-pages"></a> What kind of issues might be when developing multilingual web pages?
1. Language code - by not setting a language code or implementing the wrong code screen readers or Braille devices will not understand the content, making the page unaccessible. 
2. Language direction - some languages are written from right to left, requiring to create a mirror layout.
3. Character encoding - incorrect character encoding will cause non latin characters to render incorrectly.
4. Character rendering size - not all character sets look the same in the same font size, so different settings based on language need to be declared to restrict similar layouts.

### <a name="what-is-the-difference-between-canvas-and-svg"></a> What is the difference between Canvas and SVG?
Canvas is a pixel based rendering engine implemented via a JavaScript API. SVG is a set of HTML elements that render vector graphics.

## <a name="css"></a> CSS

### <a name="how-would-you-cause-your-page-to-render-the-same-in-all-browsers-devices-use-a-reset-stylesheet"></a> How would you cause your page to render the same in all browsers/devices?Use a “reset” stylesheet.

### <a name="what-is-the-difference-between-a-reset-and-a-normalize-css-file"></a> What is the difference between a reset and a normalize CSS file?
* Normalize.css preserves useful defaults rather than "unstyling" everything. For example, elements like sup or sub "just work" after including normalize.css (and are actually made more robust) whereas they are visually indistinguishable from normal text after including reset.css. So, normalize.css does not impose a visual starting point (homogeny) upon you. This may not be to everyone's taste. The best thing to do is experiment with both and see which gels with your preferences.
* Normalize.css corrects some common bugs that are out of scope for reset.css. It has a wider scope than reset.css, and also provides bug fixes for common problems like: display settings for HTML5 elements, the lack of font inheritance by form elements, correcting font-size rendering for pre, SVG overflow in IE9, and the button styling bug in iOS.
* Normalize.css doesn't clutter your dev tools. A common irritation when using reset.css is the large inheritance chain that is displayed in browser CSS debugging tools. This is not such an issue with normalize.css because of the targeted stylings.
* Normalize.css is more modular. The project is broken down into relatively independent sections, making it easy for you to potentially remove sections (like the form normalizations) if you know they will never be needed by your website.
* Normalize.css has better documentation. The normalize.css code is documented inline as well as more comprehensively in the GitHub Wiki. This means you can find out what each line of code is doing, why it was included, what the differences are between browsers, and more easily run your own tests. The project aims to help educate people on how browsers render elements by default, and make it easier for them to be involved in submitting improvements.

### <a name="what-is-float"></a> What is float?
With CSS float, an element can be pushed to the left or right, allowing other elements to wrap around it.

### <a name="what-are-the-various-clearing-techniques"></a> What are the various clearing techniques?
The old solution to this problem required you to add an extra element with `clear:both` to the container.
The new solution recommends adding `overflow:auto; width:100%;` to the container. overflow:hidden may also be used.

### <a name="what-is-a-css-sprite"></a> What is a CSS sprite?
An image sprite is a collection of images put into a single image. A web page with many images can take a long time to load and generates multiple server requests. Using image sprites will reduce the number of server requests and save bandwidth.

### <a name="what-is-the-difference-between-display-none-and-visibility-hidden"></a> What is the difference between display:none and visibility:hidden?
`visibility:hidden` hides an element, but it will still take up the same space as before. The element will be hidden, but still affect the layout.
`display:none` hides an element, and it will not take up any space. The element will be hidden, and the page will be displayed as if the element is not there.

### <a name="how-would-you-implement-non-standard-fonts"></a> How would you implement non-standard fonts?
By using the `@font-face` rule it is possible to include unique fonts.
###### Extra points if services like Google Fonts or TypeKit are mentioned.

### <a name="what-is-the-box-model"></a> What is the box model?
The CSS box model is essentially a box that wraps around HTML elements, and it consists of: margins, borders, padding, and the actual content.
The box model allows us to place a border around elements and space elements in relation to other elements. 

### <a name="what-is-the-problem-with-the-box-model"></a> What is the problem with the box model?
IE8 and earlier versions of IE, included padding and border in the width property.
JavaScript

### <a name="what-are-global-variables"></a> What are global variables?
Global variables are defined in the highest scope and are exposed to all JavaScript objects.

### <a name="when-would-you-use-global-variables"></a> When would you use global variables?
Global variable declaration should be avoided when possible. You should only declare globals when you want to expose a part of your application to the public.

### <a name="what-is-the-lifetime-of-variables"></a> What is the lifetime of variables?
Local variables are deleted when functions finish executing. Global variables are deleted when the page unloads. Variables can be deleted manually with the delete keyword. Garbage collection is automatic so for a resource to be destroyed it is important to remove any reference to it. 

### <a name="what-are-data-types-and-list-existing-ones-in-javascript"></a> What are data types and list existing ones in JavaScript?
A data type is a classification of the type of data a variable or object hold.  
JavaScript has the following data types: `Number`, `String`, `Boolean`, `Object`, `Null`, `Undefined`.

### <a name="what-is-the-difference-between-undefined-and-null"></a> What is the difference between undefined and null?
Undefined is a value that has not been assigned a value or that does not exist.  
Null is a value assigned to a variable and represents no value.

### <a name="what-is-a-closure"></a> What is a closure?
Closures are functions that refer to independent (free) variables.

### <a name="what-is-a-namespace"></a> What is a namespace?
A namespace is a globally nested hashtable that contains public assets.

### <a name="why-would-you-use-a-namespace"></a> Why would you use a namespace?
A namespace is used to reduce the amount of objects created on the global scope and to avoid overriding predefined objects.

### <a name="what-is-the-difference-between-==-and-==="></a> What is the difference between == and ===?
The comparison operator (==) compares values where the strict equal operator (===) compares values and types.

### <a name="what-is-event-bubbling"></a> What is event bubbling?
In bubbling the event is first captured and handled by the innermost element and then propagated to outer elements.

### <a name="what-is-event-capturing"></a> What is event capturing?
In capturing the event is first captured by the outermost element and propagated to the innermost element.

### <a name="why-would-you-use-event-bubbling-capturing"></a> Why would you use event bubbling/capturing?
This method allows setting a single callback for multiple objects and thus conserve memory. Determination logic of the target object will be done in the singular handler.

### <a name="what-is-the-difference-between-window-onclick-window-addeventlistener-click-and-window-attachevent-onclick"></a> What is the difference between window.onclick, window.addEventListener(‘click’) and window.attachEvent(‘onclick’)?
All are event observer methods.  
- `onclick` - a property of an element. If set it will trigger once.
- `attachEvent` - IE method for adding observers. Not supported as of IE11.
- `addEventListener` - Cross browser method for adding observers. Not supported prior to IE9.

### <a name="how-do-you-handle-errors"></a> How do you handle errors?
By wrapping pieces of code with `try...catch` statements.

### <a name="explain-the-following-terms-in-object-oriented-programming"></a> Explain the following terms in object-oriented programming:
Class 
> A class is an extensible template for creating objects, providing initial values for state (member variables) and implementations of behavior (member functions, methods).

Object 
> An object is a self-contained component that contains properties and methods needed to make a certain type of data useful.

Property 
> A property is a field of an object with a dedicated getter/setter routine. In JavaScript 1.8.5 Object.defineProperty was introduced to allow creation of getter/setter routines. Prior to that actual methods where needed to be defined.

Method 
> Methods are similar to functions, but they belong to classes or objects and usually expresses the verbs of the objects/class.

Constructor 
> A constructor (sometimes shortened to ctor) in a class is a special type of subroutine called to create an object.

Inheritance > Inheritance is when an object or class is based on another object or class, using the same implementation.
Encapsulation 
> Encapsulation is used to refer to one of two related but distinct notions, and sometimes to the combination thereof:
A language mechanism for restricting access to some of the object's components.  
A language construct that facilitates the bundling of data with the methods (or other functions) operating on that data.

Abstraction 
> Abstraction involves the facility to define objects that represent abstract "actors" that can perform work, report on and change their state, and "communicate" with other objects in the system.

Polymorphism 
> Polymorphism allows the expression of some sort of contract, with potentially many types implementing that contract (whether through class inheritance or not) in different ways, each according to their own purpose.

### <a name="what-type-of-inheritance-does-javascript-implement"></a> What type of inheritance does JavaScript implement?
JavaScript implements prototype inheritance. 

### <a name="what-is-the-difference-between-cookies-sessionstorage-and-localstorage"></a> What is the difference between cookies, sessionStorage and localStorage?
* cookie - stores data on the local machine.
* localStorage - an HTML5 feature that stores data with no expiration date.
* sessionStorage - an HTML5 feature that stores data for one session.

### <a name="what-is-this"></a> What is this?
this refers to the context of the current scope. Unless the scope is coming from the context of an object or was altered, this will refer to the global scope.

### <a name="what-is-the-difference-between-call-and-apply"></a> What is the difference between .call() and .apply()?
Both are methods that belong to the Function prototype and execute a function. `.call()` passes a fixed number of arguments to the function where `.apply()` passes an array of arguments with an undetermined length.

### <a name="what-does-bind-do"></a> What does .bind() do?
`.bind()` returns a clone of the function with a new context.

### <a name="what-is-the-same-origin-policy"></a> What is the same-origin policy?
The same-origin policy restricts how a document or script loaded from one origin can interact with a resource from another origin.

### <a name="what-is-the-difference-between-ajax-and-jsonp"></a> What is the difference between AJAX and JSONP?
Both are used to make calls to an external resources. Ajax calls are bound to the same domain as the script where JSONP is not.

### <a name="what-are-the-issues-with-jsonp"></a> What are the issues with JSONP?
Restricted to the HTTP GET method only.
No control over the content loaded, can introduce harmful content (code injection).

### <a name="what-solution-is-there-to-jsonp"></a> What solution is there to JSONP?
CORS (cross-origin resource sharing) in modern browsers allows to perform cross-domain requests with host identification to insure safe content. It also exposes other HTTP request methods such as POST.

### <a name="what-is-hoisting"></a> What is hoisting?
The declaration of a variable is moved to the top of the script without consideration of the line it was declared in. This means that variables that will be declared in future lines will already be accessible prior. This feature should be avoided to not cause confusion in the code. 

### <a name="would-you-extend-built-in-objects"></a> Would you extend built in objects?
It is not recommended to extend built in objects as to avoid code conflictions between 3rd party code. Sometimes built in objects are extended or overriden to provide backwards browser compatibility.

### <a name="what-is-the-difference-between-the-document-ready-and-load-events"></a> What is the difference between the document ready and load events?
The ready event occurs after the HTML document has been loaded, while the load event occurs later, when all content (e.g. images) also has been loaded.

### <a name="what-is-use-strict"></a> What is “use strict”?
Strict mode makes several changes to normal JavaScript semantics. 
Eliminates some JavaScript silent errors by changing them to throw errors.
Fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run faster than identical code that's not strict mode.
Prohibits some syntax likely to be defined in future versions of ECMAScript.
