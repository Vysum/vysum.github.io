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
    <div id="${id}" class="card text-center bg-black">
        <div class="card-header">
            <h3>
                <i class="fas fa-code" style="color: ${lang.color}"></i>
                <span> ${lang.name}</span>
            </h3>
        </div>
        <div class="card-body">
            <p>${lang.summary}</p>
            <a href="${lang.link}" target="_blank">Read More</a>
        </div>
    </div>
    `);
})
</script>