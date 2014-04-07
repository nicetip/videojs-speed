videojs-speed
=============

Setup
-----

```
    <link href="/js/video-js/video-js.css" rel="stylesheet" type="text/css">
    <script src="/js/video-js/video.js"></script>
    <script>
        videojs.options.flash.swf = "/js/video-js/video-js.swf";
    </script>
    <script src="/js/video-js-plugin/video-speed.js"></script>

    <script type='text/javascript'>
        $(function(){
            var video = videojs("video", {
                controls: true,
                autoplay: true,
                preload: 'auto',
                sources: [ { type: 'video/mp4', src: 'http://domain.com/example.mp4' } ],
                plugins: {
                    speed: [
                        { text: '1배속', rate: 1, selected: true },
                        { text: '2배속', rate: 2 },
                        { text: '4배속', rate: 4 },
                        { text: '8배속', rate: 8 }
                    ]
                }
            });
        });
    </script>
```

