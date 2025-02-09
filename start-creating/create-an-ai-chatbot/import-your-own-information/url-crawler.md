# URL Crawler

<figure><img src="../../../.gitbook/assets/image (320).png" alt="If you click the &#x22;Import&#x22; button of the &#x22;Select Your Own Information&#x22; page in the AI Chatbot creation process, you can access the URL Crawler by clicking its tab. You can then insert a root URL for crawling."><figcaption><p>If you click the "Import" button of the "Select Your Own Information" page in the AI Chatbot creation process, you can access the URL Crawler by clicking its tab. You can then insert a root URL for crawling.</p></figcaption></figure>

Thanks to the **URL Crawler**, you can now simply insert just one root URL (or main URL) and Captivate Chat will use a web crawler to gather all URLs located inside that website - no need to manually find them yourself.&#x20;

{% hint style="info" %}
**Use Direct Input if you have a specific set of URLs to ingest**

If you want your AI Chatbot to ingest and learn from all available URLs within a website, the URL Crawler is a convenient tool to use!&#x20;

**However,** you should use **Import >** **Direct Input** if you only have **a specific set of URLs** you want your AI Chatbot to ingest.
{% endhint %}

***

## Using the URL Crawler

<figure><img src="../../../.gitbook/assets/image (322).png" alt="To use the URL Crawler feature, insert the root URL or main URL you want to use as a source for the crawl. Captivate Chat will deploy a web crawler to look for all URLs nested under this source."><figcaption><p>To use the URL Crawler feature, insert the root URL or main URL you want to use as a source for the crawl. Captivate Chat will deploy a web crawler to look for all URLs nested under this source.</p></figcaption></figure>

To use the URL Crawler feature, simply place a **root URL** in the box provided and click the ![Clicking the "Submit" button under "Import Your Own Information" > Import > URL Crawler will prompt Captivate Chat to deploy a web crawler to find all pages found under that URL. ](<../../../.gitbook/assets/image (323).png>) button.

<figure><img src="../../../.gitbook/assets/image (324).png" alt="After clicking &#x22;Submit&#x22; under &#x22;Import Your Own Information&#x22; > Import > URL Crawler, Captivate Chat will list all URLs nested under your root URL. It will appear under the &#x22;Start deep crawl&#x22; pop-up window. You can then select the ones you want your AI Chatbot to ingest and click &#x22;Import Selected&#x22; to proceed."><figcaption><p>After clicking "Submit" under "Import Your Own Information" > Import > URL Crawler, Captivate Chat will list all URLs nested under your root URL. It will appear under the "Start deep crawl" pop-up window. You can then select the ones you want your AI Chatbot to ingest and click "Import Selected" to proceed.</p></figcaption></figure>

**Start deep crawl** will appear after listing your root URL. It will list all the URLs available under that main link.&#x20;

You can scroll down to choose which URLs you want your AI Chatbot to ingest, but you can also just click the checkbox beside the "URL" column name to select all the URLs listed in the crawl.&#x20;

***

## Wildcard Character

<figure><img src="../../../.gitbook/assets/image (2) (1).png" alt="Using a wildcard character or an asterisk (*) at the end of the last front slash of a root URL inside the URL Crawler will make the Captivate Chat web crawler look for all relevant URLs within that website layer."><figcaption><p>Using a wildcard character or an asterisk (*) at the end of the last front slash of a root URL inside the URL Crawler will make the Captivate Chat web crawler look for all relevant URLs within that website layer.</p></figcaption></figure>

If you want to make more precise searches with our URL Crawler, you can use what's called a **wildcard character or an asterisk (\*)** at the end of your root URL.

What this does is to command the Captivate Chat web crawler to only retrieve URLs of that specific website layer.  The Captivate Chat URL Crawler can retrieve from up to two (2) layers within a website. If we're using the above example:

### 1 Wildcard Character: `url.com/abc/*`

<figure><img src="../../../.gitbook/assets/image (3) (1).png" alt="Using only one wildcard character or asterisk (*) in the Captivate Chat URL Crawler will only retrieve URLs of one layer beneath the  specified root URL."><figcaption><p>Using only one wildcard character or asterisk (*) in the Captivate Chat URL Crawler will only retrieve URLs of one layer beneath the specified root URL.</p></figcaption></figure>

If you only use **1 Wildcard Character or asterisk (\*)** in the format `url.com/abc/*` in the URL Crawler, then you should be able to retrieve all URLs one layer below your root URL.

As a more technical example, if your website has this kind of arrangement:

`/abc/def/123`&#x20;

`/abc/def/123/456`&#x20;

`/abc/ghi/123/456`&#x20;

`/abc/jkl/`

Then, inputting `/abc/*` in the URL Crawler will only retrieve:

`/abc/def/`

`/abc/ghi/`

`/abc/jkl/`

As we only crawled one layer downward.

{% hint style="info" %}
This is useful for retrieving all pages within a single website section, such as the specific subcategories within a category of products.&#x20;

For instance, a URL Crawler can give you all brands (subcategories) of laptop (laptop) in an electronics store.&#x20;
{% endhint %}

***

### 2 Wildcard Characters: `url.com/abc/**`

<figure><img src="../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption><p>Using only two wildcard characters or asterisks (**) in the Captivate Chat URL Crawler will only retrieve URLs of one layer beneath the specified root URL.</p></figcaption></figure>

If you use **2 Wildcard Characters or asterisks (\*\*)** in the format `url.com/abc/**` in the URL Crawler, then you should be able to retrieve all the URLs under your root URL.

As a more technical example, if your website has this kind of arrangement:

`/abc/def/123`&#x20;

`/abc/def/123/456`&#x20;

`/abc/ghi/123/456`&#x20;

`/abc/jkl/`

Then, inputting `/abc/def/**` in the URL Crawler will only retrieve:

`/abc/def/123`&#x20;

`/abc/def/123/456`

As we allowed the URL Crawler to look for all pages under `/abc/def/`, including lower layers.

{% hint style="info" %}
This is useful for retrieving specific sub-types of a subcategory within a category of products.&#x20;

For instance, a URL Crawler will give you all models (sub-type) or even models of a specific year (deeper sub-type) of a brand (subcategory) of a laptop (category) in an electronics store.
{% endhint %}

***

After choosing the URLs you want to ingest, click ![Click "Import Selected" after choosing the files and URLs you want to import so your AI Chatbot can start ingesting the files. This button is available under "Import Your Own Information"](<../../../.gitbook/assets/image (325).png>) to proceed.
