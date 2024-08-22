# Special Response

* It is stored in the context variable $special\_response.
* Returns special types of response such as cards and files that are not available yet in Watson Assistant.&#x20;
* Can be used together with other types of responses such as text, buttons.&#x20;
* When $special\_response is used, all types of responses in Watson Assistant are ignored. All types of responses like texts and buttons must be added to the context variable $special\_response.
* $special\_response context variable is an array containing different types of responses.&#x20;
* Enables developers to return any types of Response to different channels. Even though the system automatically converts known specific response type formats

**Types of special responses**

1. **Card** - shows up a set of cards in the response.

![](https://lh6.googleusercontent.com/Fhk7cT3nqHMi1EvGyknPmG57KILouBpdY\_jjan1vDMrks6N67eXjMdIYC8-qfbZDfOVSeSeBLuwfLq7pTDExnyAzi5s0o7h8Mh\_BTY6EAQ4xqbK8wr1Vixjzj0s7LaX4QJgKI6M)

2\. **Pause** - pauses in between messages with the specified time in milliseconds (ms).

![](https://lh4.googleusercontent.com/fS6bhTNyAgAPk\_N0D3Gi1NN2sLwI6XiU1m2yPnS9N8iCQjeigtcMG\_WUkI-l4kU\_fHJrccflQJfN\_Z0LzJOHbe\_Ka0W2Lh5Dz3kXMyo0kSyP3xv4h1clFvAHm8eJCVgSsOZ1dIE)

3\. **Button** - shows a single message (title) and a set of options as choices.

![](https://lh4.googleusercontent.com/IZQ6p1BNa5J0ruXdwTqB04IxlUt7K-SNK2mXbnLw0l8Blm9cVFm8qx60Mgx166WauMcWZhg7qanB7bq\_hAM56\_i85Av2QURPTU5IMt5kwEtH4w0R73zXtyqWYAJHx756fr5KHQc)

4\. **Text** - shows a single message.

![](https://lh4.googleusercontent.com/FmHxofdEGv1HScRHDUifwryPuumGhDL9CJLNO8GVHKyo-zH5s2pHkeHwZQPA\_S4vtrtBpXEv6elK-Zn09FlepP0RGc7L0hP4pVdpIUt3vK7i6el5kscFg33rW6BVjgt\_kxGA-zo)

5\. **File** - attach a file as part of the response.

![](https://lh6.googleusercontent.com/yYy2L2mnzkYG6Jnb1741uOARq4-4pMuj55rvKUWHOdZQ\_Xb9V1GZumpoBQk-1Jx2XR1gFzMugYzTbDClhucTkKvTJ94V-99mG5nKPHyb0K96QrZ2JWPYpllG\_mGVXJ6Q83H-LAM)
