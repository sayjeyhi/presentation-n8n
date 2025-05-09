
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
<img src="https://cdn.n8n.io/app/uploads/2023/07/n8n-social-preview.png" class="h-60 rounded shadow" />
</div>
</div>

---

# How N8N Works

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

### Workflow Triggers
- Button clicks
- Chat messages
- Form submissions
- Webhooks
- Scheduled events

### Data Flow
- Input → Process → Output
- Transform data between steps
- Built-in `$fromAI` function
- Variables for dynamic data

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/workflows/editor-overview.png" class="h-60 rounded shadow" />
</div>
</div>

---

# Core Features

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

### Data Operations
- Filter nodes
- Switch routing
- Merge multiple streams

### Common Integrations
- Google Sheets
- Calendar apps
- CRM systems
- Email services
- Chat platforms

</v-clicks>

</div>
<div>
<div v-click class="mt-2 rounded-lg bg-gray-100 dark:bg-gray-800 p-4">
<pre class="text-sm"><code>// Example using $fromAI
const enhancedText = $fromAI.enhance(
  inputText,
  'Make more professional'
);</code></pre>
</div>
</div>
</div>

---

# Why Use N8N?

<div class="grid grid-cols-[3fr,2fr] gap-4">
<div>

<v-clicks>

- ✅ Visual workflow builder

- ✅ Open-source and extensible

- ✅ Built-in conditional logic and loops

- ✅ Code nodes for custom logic

- ✅ Active community and plugins

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/workflows/editor-overview.png" class="h-60 rounded shadow" />
</div>
</div>

---

# Core Concepts

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

- **Workflows** – Automation pipelines

- **Nodes** – Blocks that perform a task

- **Triggers** – Start a workflow (Webhook, Cron, etc.)

- **Expressions** – Use variables and data references

- **Execution Modes** – Manual, Triggered, Test

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/workflows/workflow-detail.png" class="h-60 rounded shadow" />
</div>
</div>

---
layout: two-cols
---

# Real-Life Use Cases

<v-clicks>

### Lead Collection Automation
- Trigger: Webhook
- Nodes: Airtable → Slack → Email

### Twitter Auto-Poster
- Trigger: Google Sheets update
- Nodes: HTTP Request → Twitter

### Error Monitoring
- Trigger: API failure response
- Nodes: Log to Notion → Email alert

</v-clicks>

::right::

<div class="pl-4 pt-12">
<img v-click src="https://docs.n8n.io/img/workflows/example-workflow.png" class="h-70 rounded shadow" />
</div>

---

# Example Workflow: "New Lead to CRM"

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

### Trigger: Webhook

### Steps:
1. Extract form data
2. Validate input
3. Add to Google Sheets
4. Add to CRM (e.g., HubSpot)
5. Send internal Slack alert

**Bonus**: Conditional node to skip if lead is duplicate

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/workflows/editor-ui.png" class="h-60 rounded shadow" />
</div>
</div>

---

# Key Node Types

<div class="overflow-auto">
<table class="border-collapse table-auto w-full text-sm">
  <thead>
    <tr>
      <th class="border-b dark:border-slate-600 font-medium p-4 pl-8 pt-0 pb-3 text-slate-400 dark:text-slate-200 text-left">Type</th>
      <th class="border-b dark:border-slate-600 font-medium p-4 pt-0 pb-3 text-slate-400 dark:text-slate-200 text-left">Examples</th>
    </tr>
  </thead>
  <tbody>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">Trigger</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">Webhook, Cron, Poll</td>
    </tr>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">Data</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">Set, Merge, IF</td>
    </tr>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">API</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">HTTP Request, OAuth2</td>
    </tr>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">Integration</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">Google Sheets, Trello</td>
    </tr>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">Logic</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">Switch, Wait, Loop</td>
    </tr>
    <tr v-click>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 pl-8 text-slate-500 dark:text-slate-400">Code</td>
      <td class="border-b border-slate-100 dark:border-slate-700 p-4 text-slate-500 dark:text-slate-400">JavaScript (Function)</td>
    </tr>
  </tbody>
</table>
</div>

---

# Hands-On: Tools You'll Use

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

- 🧰 N8N Desktop App or self-hosted via Docker

- 🌐 n8n.cloud (cloud-hosted option)

- 📁 Postman or browser to test webhooks

- 🛠️ Integrations: Slack, Google Sheets, GitHub, etc.

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/getting-started/desktop-app.png" class="h-60 rounded shadow" />
</div>
</div>

---

# Advanced Features

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

- 🔄 Looping (SplitInBatches node)

- 🔀 Conditional branching

- 🔐 Environment variables & credentials

- 🧠 Custom function code (JavaScript)

- 📦 Community nodes & npm modules

</v-clicks>

</div>
<div>
<div v-click class="mt-2 rounded-lg bg-gray-100 dark:bg-gray-800 p-4">
<pre class="text-sm"><code>// Example JavaScript code in Function node
return items.map(item => {
  // Transform the data
  item.json.fullName = item.json.firstName + ' ' + item.json.lastName;
  item.json.processed = true;
  return item;
});</code></pre>
</div>
</div>
</div>

---

# Tips & Best Practices

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

- Use naming conventions in nodes

- Test node-by-node using manual executions

- Store sensitive data in credentials or environment variables

- Use the Set node for data shaping

- Log errors with custom error-handling workflows

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/workflows/best-practices/naming-convention.png" class="h-60 rounded shadow" />
</div>
</div>

---
layout: two-cols
---

# Workshop Activity

<v-clicks>

### Challenge: Build a workflow to monitor a website's status

### Goal: If the site goes down, send an email alert

### Nodes used:
- Cron (Trigger every 5 min)
- HTTP Request (to check site)
- IF (check status code)
- Email (notify)

</v-clicks>

::right::

<div class="pl-4 pt-12">
<div v-click class="rounded-lg bg-gray-100 dark:bg-gray-800 p-4">
<div class="text-sm">
<p class="font-bold">Workshop Steps:</p>
<ol class="list-decimal pl-5">
  <li>Create new workflow</li>
  <li>Add Cron node (5 min interval)</li>
  <li>Add HTTP Request node</li>
  <li>Add IF node to check status</li>
  <li>Add Email node for alerts</li>
  <li>Test and activate</li>
</ol>
</div>
</div>
</div>

---

# Resources

<div class="grid grid-cols-2 gap-4">
<div>

<v-clicks>

- 🌐 [https://n8n.io](https://n8n.io)

- 📚 Docs: [https://docs.n8n.io](https://docs.n8n.io)

- 🧑‍💻 GitHub: [https://github.com/n8n-io/n8n](https://github.com/n8n-io/n8n)

- 💬 Community: [https://community.n8n.io](https://community.n8n.io)

- 🧱 Example workflows: [https://n8n.io/workflows](https://n8n.io/workflows)

</v-clicks>

</div>
<div>
<img v-click src="https://docs.n8n.io/img/getting-started/community.png" class="h-60 rounded shadow" />
</div>
</div>

---
layout: center
class: text-center
---

# Q&A + Wrap Up

What will you automate next?

Let's build it together.

Thank you! 🙏

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer" hover="bg-white bg-opacity-10">
    <a href="https://n8n.io" target="_blank">Visit n8n.io to get started</a>
  </span>
</div>
