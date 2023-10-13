# A simple scroll position synchronizer

# Introduction
Let us say that you have a simple static page that you want to view together with your friends, and take people to a particular scroll position in real time.

You add the following a few lines to the page and then viewing the page becomes collaborative.

~~~~~~~~ HTML
<script src="https://unpkg.com/@croquet/croquet"></script>
<script src="https://unpkg.com/page-synchronizer@1.0.13"></script>
<script type="text/javascript">
if (window.location.search !== "") {
    SimplePageView.start({
        apiKey: "<your apiKey from https://croquet.io/keys>",
    })
}
</script>
~~~~~~~~

Please obtain a Croquet apiKey from [Croquet Developer Portal](https://croquet.io/keys) and use a key in above snippets.

# A demonstration
You can try it on a [page](https://tinlizzie.org/ohshima?q=test123). You can create a new session by providing different `?q=` value, or you can remove the `if` test in the snippet and get everybody into the same session.
