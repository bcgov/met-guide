---
title: FAQ
author: cotes
date: 2023-06-29 20:55:00 +0800
categories: [FAQ, getting started]
tags: [faq, getting started]
pin: true
---

<!--  This is a tab component -->

<details class="faq" onclick="toggleSymbol(this)">
<summary>
    <h3>Engagement 
        <span class="symbol">+</span>
    </h3>
</summary>


<details onclick="toggleSymbol(this)">
<summary>How do I add an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Adding)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I create an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Creation)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I edit an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Editing)](#)

</details>

</details>

<!--  This is the end of a tab component -->




<details class="faq" onclick="toggleSymbol(this)">
<summary>
    <h3>Survey
        <span class="symbol">+</span>
    </h3>
</summary>


<details onclick="toggleSymbol(this)">
<summary>How do I add an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Adding)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I create an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Creation)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I edit an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Editing)](#)

</details>

</details>

<!--  This is the end of a tab component -->



<details class="faq" onclick="toggleSymbol(this)">
<summary>
    <h3>User Management
        <span class="symbol">+</span>
    </h3>
</summary>


<details onclick="toggleSymbol(this)">
<summary>How do I add an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Adding)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I create an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Creation)](#)

</details>

<details onclick="toggleSymbol(this)">
<summary>How do I edit an engagement?<span class="symbol">+</span></summary>

You must be a Superuser to create an engagement.
To create an engagement, go to the Engagement Listing page and click the "Create an Engagement" button. This will take you to the Engagement creation page.
View all the steps on the [User Guide for Engagement(Editing)](#)

</details>

</details>

<!--  This is the end of a tab component -->

<style>
.faq-wrapper{
  margin-bottom: 10px;
}

summary {
  display: flex;
  align-items: flex-end;
  flex-direction: row;
  justify-content: space-between;
  border-bottom: 1px solid black;
  font-weight: bold;
  font-size: 1.2em;
  cursor: pointer;
}

details[open] > summary {
  border-bottom: none;
}

details > p {
    padding-top: 10px;
    padding-bottom: 10px;
}

  
.symbol {
  background-color: transparent;
  border: none;
  color: gray;
  padding: 5px 15px;
  cursor: pointer;
  font-size: 1.2em;
}

</style>

<script>
function toggleSymbol(element) {
  const symbol = element.querySelector('span.symbol');

  if (element.hasAttribute('open')) {
    symbol.innerText = '+';
  } else {
    symbol.innerText = '-';
  }
}
</script>
