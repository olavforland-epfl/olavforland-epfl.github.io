---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
classes: 
    - wide
permalink: /
# title: "A (NOT SO) RANDOM WALK DOWN WALLSTREET"
# excerpt: An investigation into whether media coverage affects the stock price of Apple Inc.

# header:
#     overlay_image: /assets/images/cover_photo.jpg
#     caption: "Photo Credit: [**The Economic Times**](https://economictimes.indiatimes.com/markets/stocks/news/irrational-exuberance-are-we-near-the-shiller-mark-that-can-trigger-pain/articleshow/85265082.cms?from=mdr)"

---

<section id="header">
    <h1>A (NOT SO) RANDOM WALK DOWN WALLSTREET</h1>
    <p>An investigation into whether media coverage affects the stock price of Apple Inc.</p>
</section>

<section id="introduction">
    <h1>Companies and Media Attention</h1>
    <h2> Stock prices vary significantly from day to day</h2>
    <p>
        Some of these fluctuations are a direct result of physical events affecting the company. However, media attention and its wordings significantly affect people’s choice to buy or sell a stock, thus affecting the stock price as well. just imagine... come with examples. 
    </p>
    <h2> We want to go beyond the anecdotal </h2>
    <p>
        Quotebank provides us with tools to investigate media's effect on stock prices on a large scale. Quotebank is a corpus containing nearly 200 million quoations from the english media over the period 2008 - 2020, attributed to their most likely speaker. We have extracted quotes regarding Apple Inc. from the period 2015 - 2020, and aim to quantify the medias impact on Apple's stock price. 
    </p>
</section>


<section id="exploration">
    <h1>Who even talks about Apple?</h1>
    <h2>Everybody!</h2>
    <p>
        Since Steve Jobs' infamous presentation of the first iPhone in 2007, the popularity of Apple products has skyrocketed. Now, everybody has an iPhone. Although this is good news for Apple, we are more interested in who speeks the <b>most</b> about Apple.
    </p>
    <div class="graph_text">
        <img src="./assets/graphs/most_frequent_speakers_animation.gif">
        <blockquote>
            <h3>Those who most often mention Apple, are people working at Apple</h3>
            <p>
                People like Tim Cook (CEO), Steve Jobs (Founder) and Eddy Hue (Senior Vice President) are those who most frequently are mentioned in the media talking about Apple
            </p>
        </blockquote>
    </div>
</section>

<section id="sentiment">
    <h2>All publicity is good publicity - at least for Apple</h2>
    <p>
        To determine the contents of quotations about Apple, Python comes stacked with useful libraries. NLTK assigns a value between -1 and 1 to each quote, where -1 is absolute negative and 1 is absolute positive. By aggregating over all quotes for each month we can determine the overall attitude towards Apple. This reveils an overwhelming 
        <span style="color:#800020">positive attidude</span> towards Apple.   
    </p>
    <div class="graph_text">
        <img src="./assets/graphs/monthly_sentiment.png">
        <blockquote>
            <h3>The attidude towards Apple is overwhelmingly positive</h3>
            <p>
                Very few months land close to zero. Interestingly, the ones which do all appear in 2016. This is the year of the infamous <a href="https://en.wikipedia.org/wiki/Batterygate">Batterygate</a> scandal, where it was reveiled that Apple deliberately slowed down the processors in older iPhone models.
            </p>
        </blockquote>
    </div>
</section>

<section id="events">
    <h2>How Apple events draw massive media attention</h2>
    <p>
        Apple events are something special. Although Apple doesn't reveil the event date until right before it happens, there is always a certain expactation building in the weeks prior to each event. It's a peculiar phenomenon, espacially considering that the products and release date are known (or more precise: "rumored") weeks, and sometimes even months, in advance.<br><br>The figure illustrates how Apple's media attention builds up towards it's product events, only to fall back towards the baseline again. A normal product launch for Apple causes a 
        <span style="color: #800020">100% increase in attention.</span>
    </p>
    <img src="./assets/graphs/attention_dist.png">
</section>



<!-- For making pretty quotes -->
    <!-- <blockquote>
        <h3>An <span style="color: #800020">iPod</span>, a <span style="color: #800020">phone</span>, an <span style="color: #800020">internet mobile communicator</span>... </h3> ~Steve Jobs, prior to reveiling it being one device 
    </blockquote> -->
 