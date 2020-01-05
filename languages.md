---
layout: general
title: Git Languages
description: The guide to most known code languages!
icon: book-open
---
<div id="languages" class="container"></div>

<script src="/assets/js/languages.core.js"></script>
<script type="text/javascript">
languages.forEach(function(lang, i) {
    let id = lang.name.toLowerCase().replace(' ', '-');
    $('#languages').append(`
    <div id="${id}" class="card text-center bg-dark">
        <div class="card-header" style="background-color: ${lang.color}">
        </div>
        <div class="card-body">
            <h4>${lang.name}</h4>
            <p>${lang.summary}</p>
            <a href="${lang.link}" target="_blank">Read More</a>
        </div>
    </div>
    <br>
    `);
})
</script>