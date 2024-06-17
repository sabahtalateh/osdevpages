<head>
    <title>Markmap</title>
    <style>
        .markmap {
            position: relative;
        }
        .markmap>svg {
            width: 100%;
            height: 300px;
        }
    </style>
    <script src="https://cdn.jsdelivr.net/npm/markmap-autoloader@latest"></script>
</head>

<body>
    {% capture inc %}{% include_relative inc.md %}{% endcapture %}
    {{ inc | markdownify }}
    <div class="markmap">
        <script type="text/template">
          {% capture inc %}{% include_relative inc.md %}{% endcapture %}
          {{ inc | markdownify }}
        </script>
    </div>
</body>