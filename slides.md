---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## N8N Master Class Workshop
  Presentation slides for learning N8N workflow automation.
drawings:
  persist: false
css: unocss
---

# Automate everything (n8n)

Automate Everything with Open Source Workflows

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="avtar mt-36 rounded-full flex w-full align-center justify-center ">
  <img class="w-18 h-18 rounded-full grayscale" src="https://avatars.githubusercontent.com/u/6254009?v=4" />

  <a class="text-left ml-4 mt-2" href="https://github.com/sayjeyhi">
    <strong class="text-xl">Jafar Rezaei</strong> <br/>
    <span class="text-gray-400 text-sm">May 2025</span>
  </a>
</div>

---
layout: center
class: text-center
---

<span class="text-3xl">Almost everything we do follows a flow</span>

---
layout: center
class: text-center
---

<span class="text-3xl mb-3">It doesn't mean that</span>

<img src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExdTgwODltajBxam8ycm9ydHR5amFsM3FnbWhtaXJkb3B4Mmwyb3ZwNiZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/5QRnThZOV6csvKXdmB/giphy.gif" />

---
layout: center
class: text-center
---

```mermaid {theme: 'dark' , scale: 1.4 }
graph LR
A(Trigger) -->|Output| B(Process)
B --> |Output| C[Action 1]

B --> |Output| D[Action 2]
```

--- 

# Tools to handle automation

<br/>
<br/>

<div class="grid grid-cols-2 gap-x-4">
<div>

- n8n
- airflow
- node-red
- tray.io
- make.com
- zapier
- parbola
- ...

</div>
<div>
<img class="w-64" src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExZjVhMTFiZzNld2lhZGlpOTd2NzBuMnoxNDVtN2RkODBiNmg3bnp1byZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/12QMzVeF4QsqTC/giphy.gif" />
</div>
</div>

---


## 🔧 Open-Source Tools Comparison

| Tool         | Visual Interface | Coding Required | Flexibility   | Best For                             |
|--------------|------------------|------------------|---------------|---------------------------------------|
| **n8n**         | ✅ Yes            | ⚠️ Optional         | ✅ High        | General automation, APIs, custom logic |
| Node-RED     | ✅ Yes            | ⚠️ Minimal          | ⚠️ Medium      | IoT, home automation                  |
| Apache Airflow | ❌ No             | ✅ Required         | ✅ Very High   | Data engineering, scheduling          |
| Huginn       | ❌ Minimal        | ✅ Required         | ⚠️ Medium      | Personal data agents                  |
| Activepieces | ✅ Yes            | ❌ Low              | ⚠️ Moderate    | Simpler UI, early-stage tool          |

---

## 🌐 Cloud-Based Tools Comparison

| Tool        | Visual UI | Self-Hosted | App Integrations | Custom Logic      | Pricing Model              |
|-------------|-----------|-------------|------------------|-------------------|-----------------------------|
| **n8n**        | ✅ Yes     | ✅ Yes        | ⚠️ Growing         | ✅ JavaScript/functions | Free & paid (open source)   |
| Zapier      | ✅ Yes     | ❌ No         | ✅ Massive         | ❌ Minimal            | Paid tiers, usage-based     |
| Make (Integromat) | ✅ Yes | ❌ No         | ✅ Wide            | ⚠️ Limited scripting  | Usage-based plans           |
| Pipedream   | ✅ Yes     | ❌ No         | ✅ Good            | ✅ Node.js focused     | Generous free tier          |

---

## ✅ Summary: Where n8n Stands

### Strengths
- ✅ Open source and self-hostable
- ✅ Powerful for both developers and no-coders
- ✅ Supports custom logic and scripting
- ✅ No forced step limits (unlike Zapier)

### Weaknesses
- ⚠️ UI less polished than Zapier/Make
- ⚠️ Smaller integration library (but growing)
- ⚠️ Slightly steeper learning curve than no-code tools
- ⚠️ Needs setup for production use

---

# We Chose n8n

## n8n vs Alternatives: How It Compares

n8n sits **in the middle ground** between developer-heavy tools and no-code platforms. It blends visual workflows with the power to code when needed.

n8n is the **best balance** for teams who want the **freedom of code with visual simplicity**, without the limitations of commercial SaaS tools.

---

# What is N8N?

<div class="grid grid-cols-2 gap-x-4">
<div>

- N8N stands for "Node-Node"

- Open-source workflow automation tool

- Alternative to Zapier, Make.com

- Supports over 300 integrations and growing

- Can be self-hosted or cloud-based

</div>

<div>
<img src="/n8n.png" class="h-60 rounded shadow" />
</div>
</div>

---


# How N8N Works?


<br/>

<div class="grid grid-cols-2 gap-4">
<div>


## Workflow Triggers

<br/>

- Button clicks
- Chat messages
- Form submissions
- Webhooks
- Scheduled events


</div>
<div>


## Data Flow

<br/>

- Input → Process → Output
- Transform data between steps
- Built-in `$fromAI` function
- Variables for dynamic data


</div>
</div>

---

<img src="/sample-n8n.png">

---

# Core Features


<br/>

<div class="grid grid-cols-2 gap-4">
<div>


## Data Operations

<br/>


- Filter nodes
- Switch routing
- Merge multiple streams
- Iterate over items
- ...


</div>
<div>


## Common Integrations

<br/>

- Google Sheets
- Calendar apps
- CRM systems
- Email services
- Chat platforms
- ...


</div>
</div>

---
layout: center
class: text-center
---

<img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExY20xOXZhN3lleDhlNXVsbDljanltdHF6dnF0MG1heXY5a2NwbDk2bCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3ohs5QIWnQN3Vb3QqI/giphy.gif" />
<span class="text-3xl text-yellow">Let's jump into it...</span>

---

<div class="flex align-center flex-col items-center mt-12">
<img class="w-32 mb-12" src="https://em-content.zobj.net/source/microsoft-teams/363/cowboy-hat-face_1f920.png" />

# Thank You!

<span class="text-xs -mt-4">

Slides: <a href="https://n8n.catshoulder.dev" class="text-blue-400">n8n.catshoulder.dev</a>

</span>

[GitHub](https://github.com/sayjeyhi) · [My Website](https://sayjeyhi.com)

</div>
