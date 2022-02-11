<script>

    const fallback_onerror = (e) => {
        console.error('Some fallback')
    }

</script>

<h1>Testing on:error</h1>

<video autoplay muted loop>
    <source src="some_video.webm"
        type='video/some_unsupported_mime; codecs="some_unsupported_codec"'
        on:error={fallback_onerror}>
</video>


<!-- Workaround -->

<!-- <video autoplay muted loop>
    <source src="some_video.webm"
        type='video/some_unsupported_mime; codecs="some_unsupported_codec"'
        onerror="console.error('Some fallback - workaround')">
</video> -->
