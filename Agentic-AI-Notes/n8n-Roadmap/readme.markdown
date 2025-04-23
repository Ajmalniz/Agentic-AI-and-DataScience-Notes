# 12-Week n8n Learning Guide: Become an Expert (7 Hours/Week)

This guide outlines a 12-week plan to master n8n, a workflow automation tool, using free resources. Each week consists of 7 one-hour daily sessions (1 hour/day, 7 hours/week). The plan progresses from beginner to advanced topics, with hands-on exercises to build practical skills.

---

## Week 1: Introduction to n8n and Basic Setup
**Goal**: Understand n8n’s purpose, set up the environment, and create your first workflow.
- **Day 1: What is n8n? (1 hour)**
  - Read: “Index” (https://docs.n8n.io/) to understand n8n as a workflow automation platform.[](https://docs.n8n.io/courses/level-one/)
  - Watch: n8n introductory video on the homepage (n8n.io) for an overview.[](https://n8n.io/)
  - Task: Write a 100-word summary of n8n’s key features (e.g., nodes, integrations, fair-code license).
- **Day 2: Setup n8n (1 hour)**
  - Read: “Choose your n8n” (https://docs.n8n.io/getting-started/choose-your-n8n/) to decide between Cloud or self-hosted.[](https://docs.n8n.io/choose-n8n/)
  - Task: Install n8n using Docker (https://docs.n8n.io/hosting/installation/docker/) or sign up for n8n Cloud free trial. Verify access to the n8n Editor UI.
- **Day 3: Explore the Editor UI (1 hour)**
  - Read: “A very quick quickstart” (https://docs.n8n.io/getting-started/quickstart/) to navigate the UI.[](https://docs.n8n.io/try-it-out/quickstart/)
  - Task: Open n8n, explore the canvas, nodes panel, and settings. Create an empty workflow and save it.
- **Day 4: Build Your First Workflow (1 hour)**
  - Read: “A longer introduction” (https://docs.n8n.io/getting-started/introduction/) for a basic workflow tutorial.[](https://docs.n8n.io/try-it-out/tutorial-first-workflow/)
  - Task: Create a workflow using the Schedule Trigger node to fetch data from NASA’s API (follow the tutorial steps).
- **Day 5: Nodes and Data Flow (1 hour)**
  - Read: “Workflows App Automation Features” (https://docs.n8n.io/workflows/) to understand nodes and data flow.[](https://n8n.io/features/)
  - Task: Modify the NASA workflow to filter data (e.g., solar flares with class “X”).
- **Day 6: Community Resources (1 hour)**
  - Explore: n8n Community Forum (https://community.n8n.io/) and GitHub (https://github.com/n8n-io/n8n).[](https://github.com/n8n-io/n8n-docs)[](https://github.com/n8n-io/n8n)
  - Task: Join the forum, browse recent posts, and note one interesting workflow idea to try later.
- **Day 7: Review and Practice (1 hour)**
  - Task: Revisit your NASA workflow, activate it to run weekly, and test it manually. Review Week 1 notes and summarize key learnings in 200 words.

---

## Week 2: Core Concepts and Simple Workflows
**Goal**: Master n8n’s core concepts (nodes, triggers, credentials) and build simple automations.
- **Day 1: Nodes Deep Dive (1 hour)**
  - Read: “Nodes” section (https://docs.n8n.io/nodes/) to understand node types (trigger, action, etc.).
  - Task: Create a workflow with a Manual Trigger and an HTTP Request node to fetch data from a public API (e.g., OpenWeatherMap).
- **Day 2: Triggers (1 hour)**
  - Read: “Schedule Trigger node documentation” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/).[](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/)
  - Task: Build a workflow that triggers every 2 days at 10 AM and logs a message to the n8n console.
- **Day 3: Credentials (1 hour)**
  - Read: “Credentials” (https://docs.n8n.io/integrations/credentials/) to learn about authentication.
  - Task: Set up credentials for a free API (e.g., OpenWeatherMap) and use them in a workflow.
- **Day 4: Expressions (1 hour)**
  - Read: “Expressions” (https://docs.n8n.io/workflows/expressions/) to understand dynamic data handling.
  - Task: Modify the OpenWeatherMap workflow to use an expression to format the date (e.g., `$today`).
- **Day 5: Workflow Templates (1 hour)**
  - Explore: n8n Workflow Templates (https://n8n.io/workflows/).
  - Task: Import a simple template (e.g., Slack notification) and run it after configuring credentials.
- **Day 6: Debugging Workflows (1 hour)**
  - Read: “Workflows App Automation Features” on debugging (https://docs.n8n.io/workflows/).[](https://n8n.io/features/)
  - Task: Introduce an error in a workflow (e.g., wrong API key), debug it using the execution log, and fix it.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Build a workflow that triggers daily, fetches weather data, and sends a summary to a Telegram bot (use Telegram integration). Summarize Week 2 learnings.

---

## Week 3: Integrations and Data Transformation
**Goal**: Learn to integrate apps and manipulate data within workflows.
- **Day 1: App Integrations (1 hour)**
  - Read: “Best apps & software integrations” (https://n8n.io/integrations/).[](https://n8n.io/integrations/)
  - Task: Create a workflow connecting Notion and Slack (e.g., new Notion task sends a Slack message).
- **Day 2: HTTP Request Node (1 hour)**
  - Read: “HTTP Request node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/).
  - Task: Build a workflow using the HTTP Request node to fetch data from a public API (e.g., GitHub API).
- **Day 3: Data Transformation (1 hour)**
  - Read: “Level two: Introduction” on data processing (https://docs.n8n.io/courses/level-two/).[](https://docs.n8n.io/courses/level-two/)
  - Task: Create a workflow that fetches JSON data and uses the Edit Fields node to rename fields.
- **Day 4: Merging Data (1 hour)**
  - Read: “Merge node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.merge/).
  - Task: Build a workflow that merges data from two APIs (e.g., weather and news) into one output.
- **Day 5: Working with Databases (1 hour)**
  - Read: “Postgres” integration (https://docs.n8n.io/integrations/builtin/app-nodes/n8n-nodes-base.postgres/).
  - Task: Set up a local Postgres database and create a workflow to store API data in it.
- **Day 6: Community Workflow Example (1 hour)**
  - Explore: n8n Blog (https://blog.n8n.io/) for a practical example.[](https://blog.n8n.io/)
  - Task: Replicate a blog workflow (e.g., summarizing emails to Notion).[](https://medium.com/%40syrom_85473/a-practical-n8n-workflow-example-from-a-to-z-part-1-use-case-learning-journey-and-setup-1f4efcfb81b1)
- **Day 7: Review and Practice (1 hour)**
  - Task: Combine Notion, Slack, and Postgres in a workflow (e.g., new Notion task saves to Postgres and notifies Slack). Summarize Week 3 learnings.

---

## Week 4: Intermediate Workflows and Logic
**Goal**: Build workflows with complex logic and error handling.
- **Day 1: Conditional Logic (1 hour)**
  - Read: “IF node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.if/).
  - Task: Create a workflow that checks API data (e.g., weather temperature) and branches based on conditions.
- **Day 2: Loops and Iteration (1 hour)**
  - Read: “Loop Over Items node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.loopoveritems/).
  - Task: Build a workflow that iterates over a list of API items and processes each one.
- **Day 3: Error Handling (1 hour)**
  - Read: “Error Trigger node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.errortrigger/).
  - Task: Add error handling to a workflow to notify via Slack if an API call fails.
- **Day 4: Scheduling Complex Workflows (1 hour)**
  - Read: “Scheduling the workflow” (https://docs.n8n.io/workflows/scheduling/).[](https://docs.n8n.io/courses/level-one/chapter-5/chapter-5.7/)
  - Task: Create a workflow that runs every Monday at 8 AM and processes data with multiple steps.
- **Day 5: Webhooks (1 hour)**
  - Read: “Webhook node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.webhook/).
  - Task: Set up a webhook to trigger a workflow when an external event occurs (e.g., GitHub push).
- **Day 6: Community Forum Practice (1 hour)**
  - Task: Find a workflow problem on the n8n Community Forum, replicate it, and attempt to solve it.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Build a workflow with a webhook, conditional logic, and error handling (e.g., GitHub push triggers data processing and Slack notification). Summarize Week 4.

---

## Week 5: AI Workflows
**Goal**: Learn to build AI-powered workflows using n8n’s AI nodes.
- **Day 1: AI Basics in n8n (1 hour)**
  - Read: “Tutorial: Build an AI workflow in n8n” (https://docs.n8n.io/ai/tutorial/).[](https://docs.n8n.io/advanced-ai/intro-tutorial/)
  - Task: Watch the linked video and summarize AI concepts (e.g., LLMs, agents).
- **Day 2: AI Agent Node (1 hour)**
  - Read: “AI Agent node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.aiagent/).
  - Task: Create a basic AI workflow with the Chat Trigger and AI Agent node using a free model (e.g., DeepSeek).
- **Day 3: Chat Workflows (1 hour)**
  - Read: “Chat Trigger node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.chattrigger/).
  - Task: Build a chat workflow that retains context between messages.
- **Day 4: AI with External Data (1 hour)**
  - Task: Extend the AI workflow to fetch data from an API and use it in the AI prompt.
- **Day 5: AI Workflow Templates (1 hour)**
  - Explore: AI Workflow Templates (https://n8n.io/workflows/?tags=AI).
  - Task: Import and customize an AI template (e.g., document summarization).
- **Day 6: Debugging AI Workflows (1 hour)**
  - Task: Introduce an error in the AI workflow (e.g., invalid prompt), debug it, and fix it.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Build an AI workflow that fetches news data, summarizes it with an AI agent, and posts to Slack. Summarize Week 5 learnings.

---

## Week 6: Custom Code and Advanced Nodes
**Goal**: Use JavaScript/Python in workflows and explore advanced nodes.
- **Day 1: Code Node Basics (1 hour)**
  - Read: “Code node” (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/).
  - Task: Create a workflow with a Code node to manipulate JSON data (e.g., filter items).
- **Day 2: JavaScript in Code Node (1 hour)**
  - Task: Write a JavaScript function in the Code node to process API data (e.g., calculate averages).
- **Day 3: Python in Code Node (1 hour)**
  - Read: “Code node” Python section (https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.code/).
  - Task: Rewrite the JavaScript function in Python.
- **Day 4: Advanced Nodes (1 hour)**
  - Read: “Merge node” and “Switch node” (https://docs.n8n.io/integrations/builtin/core-nodes/).
  - Task: Build a workflow using Switch and Merge nodes for complex data routing.
- **Day 5: Community Code Examples (1 hour)**
  - Explore: GitHub n8n repository (https://github.com/n8n-io/n8n) for code examples.[](https://github.com/n8n-io/n8n)
  - Task: Replicate a Code node example from GitHub.
- **Day 6: Debugging Code Nodes (1 hour)**
  - Task: Introduce a syntax error in a Code node, debug it using logs, and fix it.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Build a workflow that fetches data, processes it with a Code node (JavaScript or Python), and stores it in Postgres. Summarize Week 6.

---

## Week 7: Self-Hosting and Scalability
**Goal**: Learn to self-host n8n and manage scalable deployments.
- **Day 1: Self-Hosting Basics (1 hour)**
  - Read: “n8n Hosting Documentation” (https://docs.n8n.io/hosting/).[](https://docs.n8n.io/hosting/)
  - Task: Review your Docker setup and ensure it’s optimized.
- **Day 2: Environment Variables (1 hour)**
  - Read: “Environment variables” (https://docs.n8n.io/hosting/configuration/environment-variables/).
  - Task: Configure n8n with custom environment variables (e.g., timezone).
- **Day 3: Scaling n8n (1 hour)**
  - Read: “Amazon Web Services” for Kubernetes scaling (https://docs.n8n.io/hosting/installation/aws/).[](https://docs.n8n.io/hosting/installation/server-setups/aws/)
  - Task: Simulate scaling by running multiple Docker containers locally.
- **Day 4: Security Best Practices (1 hour)**
  - Read: “Security” (https://docs.n8n.io/hosting/security/).
  - Task: Implement HTTPS for your n8n instance using a reverse proxy (e.g., Nginx).
- **Day 5: Backup and Recovery (1 hour)**
  - Task: Create a backup of your n8n workflows and test restoring them.
- **Day 6: Community Hosting Tips (1 hour)**
  - Explore: “An easy step-by-step guide on how to self-host n8n” (https://community.n8n.io/t/an-easy-step-by-step-guide-on-how-to-self-host-n8n/398).[](https://community.n8n.io/t/an-easy-step-by-step-guide-on-how-to-self-host-n8n/6505)
  - Task: Apply one tip from the community guide to your setup.
- **Day 7: Review and Practice (1 hour)**
  - Task: Deploy a workflow on your self-hosted instance and test its scalability with multiple executions. Summarize Week 7 learnings.

---

## Week 8: Real-World Projects
**Goal**: Apply skills to build practical, real-world workflows.
- **Day 1: Project Planning (1 hour)**
  - Task: Identify a manual process to automate (e.g., social media posting, email summaries).
- **Day 2: API Integration (1 hour)**
  - Task: Build a workflow integrating an API for your project (e.g., Twitter API for posting).
- **Day 3: Database Storage (1 hour)**
  - Task: Add a database component to store project data (e.g., Postgres or MongoDB).
- **Day 4: AI Enhancement (1 hour)**
  - Task: Incorporate an AI agent to enhance the project (e.g., summarize content).
- **Day 5: Scheduling and Webhooks (1 hour)**
  - Task: Add a Schedule Trigger or Webhook to automate the project workflow.
- **Day 6: Testing and Debugging (1 hour)**
  - Task: Test the project workflow, debug any issues, and optimize performance.
- **Day 7: Review and Documentation (1 hour)**
  - Task: Document your project workflow in a 300-word summary. Share it on the n8n Community Forum for feedback.

---

## Week 9: Advanced AI and Custom Nodes
**Goal**: Build advanced AI workflows and create custom nodes.
- **Day 1: Advanced AI Concepts (1 hour)**
  - Read: “Examples and concepts” (https://docs.n8n.io/ai/examples/).[](https://docs.n8n.io/advanced-ai/intro-tutorial/)
  - Task: Summarize multimodal AI capabilities in n8n.
- **Day 2: Complex AI Workflow (1 hour)**
  - Task: Build a workflow that processes images or audio with an AI agent.
- **Day 3: Custom Node Basics (1 hour)**
  - Read: “n8n-nodes-starter” (https://github.com/n8n-io/n8n-nodes-starter).[](https://github.com/n8n-io)
  - Task: Set up the environment to create a custom node.
- **Day 4: Build a Custom Node (1 hour)**
  - Task: Create a simple custom node (e.g., fetch data from a niche API).
- **Day 5: Test Custom Node (1 hour)**
  - Task: Test and debug the custom node in a workflow.
- **Day 6: Community Node Examples (1 hour)**
  - Explore: GitHub for custom nodes (https://github.com/n8n-io/).
  - Task: Install and test a community-contributed node.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Build a workflow using your custom node and an AI agent. Summarize Week 9 learnings.

---

## Week 10: Enterprise Features and Collaboration
**Goal**: Explore enterprise features and collaborative workflows.
- **Day 1: Enterprise Features (1 hour)**
  - Read: “n8n Plans and Pricing” for enterprise features (https://n8n.io/pricing/).[](https://n8n.io/pricing/)
  - Task: Summarize free vs. enterprise features (e.g., SSO, RBAC).
- **Day 2: Multi-User Workflows (1 hour)**
  - Read: “Users and permissions” (https://docs.n8n.io/users-permissions/).
  - Task: Simulate a multi-user setup locally and assign roles.
- **Day 3: Version Control (1 hour)**
  - Read: “Version control” (https://docs.n8n.io/hosting/version-control/).
  - Task: Set up Git to version control your workflows.
- **Day 4: Audit Logs (1 hour)**
  - Task: Configure audit logs for your n8n instance and review them.
- **Day 5: Collaborative Workflow (1 hour)**
  - Task: Build a workflow for a team (e.g., task assignment in Notion with Slack updates).
- **Day 6: Community Collaboration (1 hour)**
  - Task: Share a workflow on the n8n Community Forum and provide feedback on another user’s workflow.
- **Day 7: Review and Practice (1 hour)**
  - Task: Optimize the collaborative workflow and summarize Week 10 learnings.

---

## Week 11: Optimization and Performance
**Goal**: Optimize workflows and improve performance.
- **Day 1: Workflow Optimization (1 hour)**
  - Read: “Performance” (https://docs.n8n.io/hosting/performance/).
  - Task: Analyze a workflow for bottlenecks and optimize it.
- **Day 2: Caching Data (1 hour)**
  - Task: Implement caching in a workflow to reduce API calls.
- **Day 3: Parallel Processing (1 hour)**
  - Task: Modify a workflow to process items in parallel using the Split In Batches node.
- **Day 4: Monitoring Workflows (1 hour)**
  - Task: Set up monitoring for workflow executions (e.g., Slack notifications for failures).
- **Day 5: Stress Testing (1 hour)**
  - Task: Stress test a workflow with high data volumes and document performance.
- **Day 6: Community Optimization Tips (1 hour)**
  - Explore: n8n Community Forum for performance tips.
  - Task: Apply one optimization technique from the forum.
- **Day 7: Review and Mini-Project (1 hour)**
  - Task: Optimize a previous project workflow for performance and summarize Week 11 learnings.

---

## Week 12: Capstone Project and Certification
**Goal**: Build a capstone project and explore certification options.
- **Day 1: Project Planning (1 hour)**
  - Task: Design a complex workflow integrating APIs, AI, databases, and webhooks (e.g., automate a business process).
- **Day 2: Build Core Workflow (1 hour)**
  - Task: Implement the core components of the capstone project.
- **Day 3: Add AI and Custom Nodes (1 hour)**
  - Task: Incorporate an AI agent and a custom node into the project.
- **Day 4: Test and Debug (1 hour)**
  - Task: Thoroughly test and debug the project workflow.
- **Day 5: Deploy and Optimize (1 hour)**
  - Task: Deploy the workflow on your self-hosted instance and optimize performance.
- **Day 6: Documentation and Sharing (1 hour)**
  - Task: Document the project in a 500-word report and share it on the n8n Community Forum.
- **Day 7: Review and Next Steps (1 hour)**
  - Task: Review all 12 weeks, summarize key skills, and explore n8n certification options (https://n8n.io/academy/). Plan to contribute a workflow to GitHub.

---

## Additional Notes
- **Resources**: All links are from n8n’s official documentation, blog, GitHub, or community forum, ensuring they are free. Check https://docs.n8n.io/ for updates.[](https://docs.n8n.io/learning-path/)
- **Practice**: Hands-on tasks are critical. Spend extra time experimenting with workflows to reinforce learning.
- **Community**: Engage with the n8n Community Forum (https://community.n8n.io/) for support and inspiration.[](https://github.com/n8n-io/n8n)
- **Progress Tracking**: Keep a journal of your daily tasks and summaries to track progress.
- **Certification**: After Week 12, consider n8n’s free or paid certification courses at https://n8n.io/academy/ to formalize your expertise.

By following this guide, you’ll gain the skills to automate complex processes, integrate apps, and leverage AI in n8n, making you an expert in workflow automation.