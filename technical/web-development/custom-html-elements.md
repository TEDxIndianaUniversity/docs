# 🧠 Custom HTML Elements

## Overview

Got some HTML, CSS, and JS experience? Need a better component than the ones provided? Easy! We can do that with a custom element. Just like any [web component](https://developer.mozilla.org/en-US/docs/Web/Web\_Components), you can build components to use in Wix Studio. Once you've coded the JS, the elements are available in the Wix Studio Editor! Here's some details:

{% embed url="https://dev.wix.com/docs/develop-websites/articles/wix-editor-elements/custom-elements/about-custom-elements" %}

## About Web Components

Web components have had decent support across web browsers [for the last few years](https://developer.mozilla.org/en-US/docs/Web/API/Web\_components#browser\_compatibility). While I'm not a fan of over-JSing things, this is a great way to add custom behaviour to a Wix site. In case you aren't familiar with web components, I recommend researching about them [on MDN](https://developer.mozilla.org/en-US/docs/Web/API/Web\_components) and [Wix Developer Docs](https://dev.wix.com/docs/develop-websites/articles/wix-editor-elements/custom-elements/about-custom-elements#examples). Here's a simple example to get you started:

<pre class="language-javascript" data-line-numbers><code class="lang-javascript">// Create a subclass of HTMLElement
class HelloWorld extends HTMLElement {

  // connectedCallback() is called whenever rendering is attempted
  connectedCallback() {
    // Define the innerHTML; add attribute handing; etc.
    this.innerHTML = '&#x3C;br>Hello World!';
  }
  
  // Here you can implement another <a data-footnote-ref href="#user-content-fn-1">lifecycle callback</a>
  
}

// Register the class as a web component
customElements.define('hello-world', HelloWorld);
</code></pre>



[^1]: [https://developer.mozilla.org/en-US/docs/Web/API/Web\_components/Using\_custom\_elements#Using\_the\_lifecycle\_callbacks](https://developer.mozilla.org/en-US/docs/Web/API/Web\_components/Using\_custom\_elements#Using\_the\_lifecycle\_callbacks)

