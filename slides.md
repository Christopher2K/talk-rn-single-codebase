```yaml
theme: apple-basic
layout: intro
transition: slide-left
```

# From React-Native to React-\*

Introduction to a strategy to `write Once, deploy Everywhere`

<div class="absolute bottom-0 bottom-5">
  <p>
    Christopher N. Katoyi Kaba
  </p>
  <p class="font-200">
    Senior Frontend Engineer @ Maple, Toronto, ON
  </p>
</div>

---

```yaml
layout: custom-image-right
image: mockup-1.png
transition: slide-up
```

# Concentration

Cross-platform pomodoro<span class="font-900 color-red-900">\*</span> timer

<ul class="w-full text-left">
  <li>Available on iOS, Android, MacOS, Linux</li>
  <li>Initially built for mobile, using Expo</li>
  <li>Used by 4000 people across 3 continents!</li>
</ul>

<div class="absolute bottom-0 bottom-5">
  <p class="font-200">
    <span class="color-red-900 font-900">*</span> : A pomodoro timer orchestrates 25-minute work sessions with 5-minute breaks.  </p>
</div>

---

```yaml
layout: custom-two-cols
clicks: 3
```

::header::

# Two code-share strategies

👎 Strategy one: one app, same entry point, `n`<span class="font-900 color-red-900">\*</span> builds process

::footer::

<p class="font-200">
  <span class="color-red-900 font-900">*</span> : `n` being the number of platforms supported
</p>

::left::

<OneAppStrategy />

::right::

<span v-click="1">

## What I like

<div class="mb-5">

- 🚀 Faster time to market.
- 💅 Perfect when apps have to look the exact same.

</div>

</span>

<span v-click="2">

## What I want to avoid

<div>

- 🫨 Code is harder to read.
- 🚨 Introducing new libs is more error prone.
- 😵‍💫 Platform specifics semantics or specifics are harder to implement.

</div>

</span>

---
