---
# try also 'default' to start simple
theme: '@doctolib/slidev-theme'
# Team collaboration chaos - perfect for AI reality check
background: https://images.unsplash.com/photo-1516534775068-ba3e7458af70?q=80&w=3270&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply UnoCSS classes to the current slide
class: text-center
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
---

# AI Reality Check

Our Wins, Fails & Hard-Earned Lessons at BOSS

<!--
No-bullshit breakdown of our Q3 AI journey at BOSS
-->

---
transition: fade-out
class: text-center
---

# What We'll Cover

<div grid="~ cols-1 gap-8" class="mt-12">

<div v-click="1" class="flex items-center gap-4 text-xl">
  🚀 <span class="font-semibold text-green-400">The Game Changers</span> - Concrete wins and team deep changes
</div>

<div v-click="2" class="flex items-center gap-4 text-xl">
  ⚠️ <span class="font-semibold text-red-400">The Time Thieves</span> - What made us lose hours (and sanity)
</div>

<div v-click="3" class="flex items-center gap-4 text-xl">
  🎯 <span class="font-semibold text-blue-400">The Takeaways</span> - What we'd do differently tomorrow
</div>

</div>

---
layout: section
class: text-center
---

# 🚀 The Game Changers
## Concrete wins and team deep changes

---

# Code Way Faster to Write

<div grid="~ cols-2 gap-8" class="mt-8">
<div>

## Before AI 🐌
- Writing boilerplate took **hours** and are error-prone
- We put our ego in our code
- Starting from scratch every time

</div>
<div v-click>

## With AI 🚀
- **Most of code** written by AI first-pass
- More time and distance to be perform critical reviews on-the-fly
- Very fast refactoring and optimization

</div>
</div>

<div v-click="2" class="mt-6">
<h2 class="text-xl font-semibold mb-4">🎯 Game Changer: JIRA → PR Magic</h2>
<div class="p-4 bg-blue-900/20 border border-blue-400/30 rounded">
<strong>From ticket to working PR in 15 minutes:</strong> With well written tickets, AI reads specs, generates implementation plan, writes code, creates and run tests, and submits PR ready for review
</div>
</div>

---

# Automate Boring Tasks

<div class="mt-8">

<div grid="~ cols-2 gap-8" class="mt-6">
<div>

<div v-click="1">
<h3 class="text-lg font-semibold mb-2">🧪 Test Generation on Autopilot</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Tests generated without bias</li>
  <li>Integration tests with realistic mock data</li>
  <li>Edge cases we never thought of</li>
</ul>
</div>

<div v-click="3" class="mt-6">
<h3 class="text-lg font-semibold mb-2">📝 Documentation & Comments</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Update automatically comments alongside the code</li>
  <li>Project documentation that stay up to date</li>
</ul>
</div>

</div>
<div>

<div v-click="2">
<h3 class="text-lg font-semibold mb-2">🏗️ Boilerplate Generation</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>DTOs, interfaces, and type definitions</li>
  <li>CRUD operations and repository patterns</li>
  <li>API endpoints with proper validation</li>
  <li>Database migrations and schema updates</li>
</ul>
</div>

</div>
</div>

<div v-click="3">
<div class="p-4 bg-purple-900/20 border border-purple-400/30 rounded font-(family-name:Roboto)">
🎙️ I feel like I'm cheating, I took the ticket and it was finished in 20 minutes
</div>
</div>

</div>

---
layout: section
class: text-center
---

# ⚠️ The Time Thieves
## What made us lose hours (and sanity)

---

# Review Time Explosion

<div v-click="1">
<h2 class="text-xl font-semibold mb-4">🔍 The Code Review</h2>
<div class="p-4 bg-red-900/20 border border-red-400/30 rounded mb-6">
AI generates code fast, but volumes of code, bloated description and inconsistent patterns create review nightmares
</div>
</div>

<div v-click="2">
<h2 class="text-xl font-semibold mb-4">💥 Real Story: Error Management Chaos</h2>
<div class="grid grid-cols-2 gap-6">
<div class="p-4 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-red-400">What Happened:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>AI generated different error patterns across different files</li>
  <li>Review couldn't catch the inconsistencies</li>
</ul>
</div>
<div class="p-4 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-yellow-400">The Aftermath:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Complex evolution of a feature</li>
  <li>Error handling refactor needed</li>
  <li>Creation of an ADR and context updated</li>
</ul>
</div>
</div>
</div>

---

# JIRA Epic Generation - The Dream

<div class="mt-8">

<div v-click="1">
<div class="p-4 bg-blue-900/20 border border-blue-400/30 rounded mb-6">
From tech scoping document → Full JIRA Epic structure automatically
</div>
</div>

<div v-click="2" class="space-y-4">
<div class="p-4 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-blue-400">Expected Workflow:</h3>
<ul class="list-disc list-inside space-y-2 text-sm">
  <li>📄 Start with tech scoping document</li>
  <li>✅ Generate all needed JIRA tickets (User Stories + subtasks)</li>
  <li>🔗 All task tickets linked with implementation proposal</li>
</ul>
</div>
</div>

</div>

---

# JIRA Epic Generation - Reality Check

<div class="mt-8">

<div class="grid grid-cols-2 gap-6 mb-6">
<div class="p-4 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-red-400">The Problems:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Very slow to read/write tickets via MCP</li>
  <li>AI loses information during create/update (even with explicit checks!)</li>
  <li>Tickets are inconsistent across the epic</li>
  <li>MCP cannot add links between tickets</li>
  <li>Missing mandatory fields block ticket creation</li>
</ul>
</div>
<div class="p-4 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-yellow-400">How We Mitigated:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Create local .md file cache to reduce slow MCP read/write</li>
  <li>Copy-paste from AI response (bypass MCP entirely)</li>
  <li>Create template files for US/tasks to enforce consistency</li>
  <li>Add links manually in a dedicated description section</li>
  <li>Provide an example ticket as base template with mandatory fields</li>
</ul>
</div>
</div>

<div v-click="3" class="p-4 bg-purple-900/20 border border-purple-400/30 rounded">
<strong>The Reality:</strong> Despite workarounds, JIRA ticket generation remains a manual, time-consuming process 😮‍💨
</div>

</div>

---

# Implementation in Tickets - The Dilemma

<div class="mt-4">

<div v-click="1">
<div class="p-3 bg-blue-900/20 border border-blue-400/30 rounded mb-4 text-sm">
Should we include implementation details in tickets for AI code generation?
</div>
</div>

<div v-click="2" class="grid grid-cols-2 gap-4 mb-4">
<div class="p-3 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-red-400">The Problems:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Time consuming to manage tickets with code</li>
  <li>Grooming = code review, not solution discussion</li>
  <li>Code changes break ticket synchronization</li>
</ul>
</div>
<div class="p-3 bg-gray-200 rounded">
<h3 class="font-semibold mb-2 text-yellow-400">Current Approach:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Remove implementation from tickets</li>
  <li>Developer implements when taking ticket</li>
  <li>Provide enough context for AI generation</li>
</ul>
</div>
</div>

<div v-click="3" class="p-3 bg-purple-900/20 border border-purple-400/30 rounded">
<h3 class="font-semibold mb-2 text-green-400">💡 TLDR; We need to change our process:</h3>
<ul class="list-disc list-inside space-y-1 text-sm">
  <li>Remove / Revamp grooming ritual entirely</li>
  <li>Remove subtasks (only for progress tracking)</li>
  <li>Pair or mob programming for ticket/code generation</li>
</ul>
</div>

</div>

---
layout: section
class: text-center
---

# 🎯 The Takeaways
## What are we doing differently

---

# Context First

<div class="mt-2">

<div v-click="1">
<h2 class="text-xl font-semibold mb-4">🧠 Poor Context = 90% of AI Failures</h2>
<div class="p-2 bg-red-900/20 border border-red-400/30 rounded mb-2">
<strong>Hard Truth:</strong> AI doesn't fail because it's stupid. It fails because we give it garbage context.
</div>
</div>

<div v-click="2" class="grid grid-cols-2 gap-6">
<div>
<h3 class="font-semibold mb-3 text-blue-400">The Context Investment Strategy</h3>
<div class="space-y-3 text-sm">
  <div class="p-3 bg-gray-200 rounded">
    <strong>General context</strong>
    <ul class="list-disc list-inside mt-1 space-y-1">
      <li>Main commands</li>
      <li>Principales guidelines and ADRs links</li>
      <li>Technical stack</li>
      <li>Link to other docs with context</li>
    </ul>
  </div>
</div>

<div class="space-y-3 py-3">
  <div class="p-2 bg-blue-900/20 border border-blue-400/30 rounded text-sm">
    <strong>📊 Quality Metrics:</strong> Context relevance > Context volume
  </div>
  <div class="p-2 bg-yellow-900/20 border border-yellow-400/30 rounded text-sm">
    <strong>🔄 Living Document:</strong> Update context as codebase evolves
  </div>
</div>
</div>

<div>
<h3 class="font-semibold mb-3 text-green-400">Other Documentation Links</h3>
<div class="p-3 bg-gray-200 rounded">
  <ul class="list-disc list-inside space-y-1 text-sm">
    <li>Domain-specific business logic</li>
    <li>Common pitfalls & solutions</li>
    <li>Framework / APIs docs & best practices</li>
    <li>Security guidelines</li>
  </ul>
</div>
</div>
</div>

</div>

---

# Documentation as living part of the code

<div class="mt-2">

<div v-click="1">
<h2 class="text-xl font-semibold mb-2">🎯 Structure Your Docs for AI Success</h2>
<div class="p-2 bg-blue-900/20 border border-blue-400/30 rounded">
<strong>Goal:</strong> Make documentation that AI can easily parse, understand, and leverage
</div>
</div>

<div v-click="2" class="grid grid-cols-2 gap-6">
<div>
<h3 class="font-semibold mb-3 text-green-400">Format & Structure</h3>
<div class="space-y-3 text-sm">
  <div class="p-2 bg-orange-900/20 border border-green-400/30 rounded">
    <strong>📋 Co-located Documentation :</strong> All docs live alongside in a dedicated directory (/docs, /docs/adr/, ...)
  </div>
  <div class="p-2 bg-green-900/20 border border-green-400/30 rounded">
    <strong>📋 Searchable Format:</strong> Markdown with clear headings and examples, Mermaid for the schemas
  </div>
  <div class="p-2 bg-blue-900/20 border border-blue-400/30 rounded">
    <strong>🚀 Auto-Discovery:</strong> AI finds relevant docs through file structure
  </div>
  <div class="p-2 bg-purple-900/20 border border-purple-400/30 rounded">
    <strong>🔄 CI/CD Integration:</strong> Docs updated and validated regularly
  </div>
</div>
</div>

<div>
<h3 class="font-semibold mb-3 text-purple-400">Context Linking</h3>
<div class="space-y-3 text-sm">
  <div class="p-3 bg-gray-200 rounded">
    <strong>✅ Context Pointers Examples:</strong>
    <ul class="list-disc list-inside mt-1 space-y-1">
      <li>"See /docs/patterns/error-handling.md for standards"</li>
      <li>"Check /docs/adr/012-authentication.md for auth patterns"</li>
      <li>"Follow /docs/api/validation.md for input validation"</li>
    </ul>
  </div>
</div>
</div>
</div>

</div>

---

# Knowledge Sharing

<div class="mt-6">

<div v-click="1">
<h2 class="text-xl font-semibold mb-4">🚀 AI Evolves Fast - Stay Connected</h2>
<div class="p-2 bg-blue-900/20 border border-blue-400/30 rounded mb-2">
<strong>Reality:</strong> AI landscape changes weekly, especially at Doctolib. Yesterday's best practices are today's anti-patterns.
</div>
</div>

<div class="grid grid-cols-2 gap-6">
<div v-click="2">
<h3 class="font-semibold mb-3 text-green-400">Stay in the Loop</h3>
<div class="space-y-3 text-sm">
  <div class="p-3 bg-gray-200 rounded">
    <strong>🗣️ Join Community Channels</strong>
    <ul class="list-disc list-inside mt-1 space-y-1">
      <li><strong>#build-with-ai</strong> - Latest tools & techniques</li>
    </ul>
  </div>
  <div class="p-3 bg-gray-200 rounded">
    <strong>📚 Learn from Others' XP</strong>
    <ul class="list-disc list-inside mt-1 space-y-1">
      <li>Failed experiments teach more than wins</li>
      <li>Pair-sharing inside your team / domain</li>
    </ul>
  </div>
</div>
</div>

<div v-click="3">
<h3 class="font-semibold mb-3 text-purple-400">Share Your Journey</h3>
<div class="space-y-3 text-sm">
  <div class="p-2 bg-green-900/20 border border-green-400/30 rounded">
    <strong>🏠 Internal Sharing:</strong> Team demos, BP Pulse, Tech time
  </div>
  <div class="p-2 bg-yellow-900/20 border border-yellow-400/30 rounded">
    <strong>💡 Document Everything:</strong> Wins, fails, and "meh" experiments
  </div>
  <div class="p-2 bg-purple-900/20 border border-purple-400/30 rounded">
    <strong>🔄 Create Feedback Loops:</strong> Regular AI tool evaluations
  </div>
</div>
</div>
</div>

</div>

---
layout: cover
class: text-center
background: https://images.unsplash.com/photo-1665789318391-6057c533005e?q=80&w=2064&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
---

# Questions?

<div class="mt-6 text-sm opacity-50">
Thanks for listening to our AI reality check 🤖
</div>

<img src="/QrCode.png" alt="QR Code" class="absolute bottom-4 right-4 w-32 h-32 bg-white p-2 rounded" />
