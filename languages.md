---
layout: general
title: Language Rosetta
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
        <div class="card-header">
            <h4>
                <i class="fas fa-circle fa-sm" style="color: ${lang.color}"></i>
                <span> ${lang.name}</span>
            </h4>
        </div>
        <div class="card-body">
            <p>${lang.summary}</p>
            <a href="${lang.link}" target="_blank">Read More</a>
        </div>
    </div>
    <br>
    `);
})
</script>