# Word Cloud Demo

First, I grabbed Bootstrap's [starter template](https://getbootstrap.com/docs/4.3/getting-started/introduction/).
Next, I grabbed the `wordcloud2.js` file from [here](https://github.com/timdream/wordcloud2.js/blob/gh-pages/src/wordcloud2.js).

Back in `index.html`, I added the following lines:

```html

<!-- A place to render the word cloud -->
<canvas id="content-main"></canvas>

<!-- Load the wordcloud2 script -->
<script src='./wordcloud2.js'></script>

<!-- A function call-->
<script>
    // A list to render (weeb theme)
    var phraseFrequenciesList =
        [['nippon', 72], ['desu', 24], ['neko', 36], ['inu', 36], ['kawaii', 14], ['sakura', 16]];

    WordCloud(document.getElementById('content-main'), { list: phraseFrequenciesList });
</script>

```

Refreshing the page a few times, you can see that the `WordCloud` function doesn't produce the same result every time.