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
transition: fade
```

::header::

# Two code-share strategies

👎 Strategy one: one app, same entrypoint, `n`<span class="font-900 color-red-900">\*</span> builds process

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
- 😵‍💫 Platform specifics are harder to implement.

</div>

</span>

---

```yaml
layout: custom-two-cols
```

::header::

# Two code-share strategies

🚀 Strategy two: `n`<span class="font-900 color-red-900">\*</span> apps, `n` entrypoints, as much as **packages** as you need

::footer::

<p class="font-200">
  <span class="color-red-900 font-900">*</span> : `n` being the number of platforms supported
</p>

::left::

<NAppsStrategy />

::right::

<span v-click="1">

## What I like

<div class="mb-5">

- 👍 Easy to work on platform specifics
- ♻️ Builds are easier to manage
- 🫂 One app does not impact another
- 🪜 Changes are incremental

</div>

</span>

<span v-click="2">

## Where's the catch

<div>

- 🐢 Requires more planning than strategy 1.
- 📦 CI/CD is hard to figure out.

</div>

</span>

---

```yaml
layout: custom-two-cols
transition: fade
```

::header::

# What does strategy 2 looks like?

Inside Concentration, our case study

::left::

## Apps

- All applications are under `apps`.
- Each application is independant from others

## Libraries

- Libraries are shreable assets
  - Assets (images, fonts)
  - Configuration files (prettier, eslint)
  - UI components
  - Domain logic

::right::

<img src="/concentration-folders.png" class="h-[400px] w-auto" />
