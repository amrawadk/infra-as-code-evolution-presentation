---
theme: default
background: https://source.unsplash.com/collection/94734566/1920x1080
class: text-center
highlighter: shiki
lineNumbers: false
info: |
  ## From Scripts to Strategy
  The Past, Present, and Future of Infrastructure as Code
drawings:
  persist: false
transition: slide-left
title: From Scripts to Strategy
mdc: true
---

# From Scripts to Strategy
## The Past, Present, and Future of Infrastructure as Code

<div class="pt-12">
  <span class="text-xl text-opacity-80">
    Presented by [Your Name]
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <a href="https://github.com/yourusername" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---
layout: section
---

# What is Infrastructure as Code?

---
layout: two-cols
---

# Your Application

<div class="flex flex-col gap-2">
  <div class="flex items-center gap-2">
    <carbon:application class="text-blue-500 text-2xl"/>
    <span>Your core business logic</span>
  </div>
  <div class="text-sm text-gray-400 mt-2">
    The code your team writes daily
  </div>
</div>

::right::

# Everything Else

<div class="flex flex-col gap-4 mt-2">
  <div class="flex items-center gap-2">
    <carbon:cloud class="text-green-500"/>
    <span>Compute Resources</span>
  </div>
  <div class="flex items-center gap-2">
    <carbon:datastore class="text-green-500"/>
    <span>Storage Solutions</span>
  </div>
  <div class="flex items-center gap-2">
    <carbon:network-2 class="text-green-500"/>
    <span>Networking</span>
  </div>
  <div class="flex items-center gap-2">
    <carbon:notification class="text-green-500"/>
    <span>Monitoring & Alerting</span>
  </div>
</div>

---
layout: quote
---

# "Infrastructure as Code is treating your infrastructure with the same respect as your application code."

---
layout: default
---

# The "as Code" Part

<v-clicks>

- **Version Controlled**: Track changes, rollback when needed
- **Reproducible**: Same code = Same infrastructure
- **Testable**: Validate before applying
- **Collaborative**: Review infrastructure changes like code
- **Automated**: No manual clicking in consoles

</v-clicks>

---
layout: two-cols
---

# IaC in Practice

```hcl
# AWS Infrastructure Example
resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"

  tags = {
    Name = "WebServer"
    Environment = "Production"
  }
}

resource "aws_s3_bucket" "logs" {
  bucket = "my-app-logs"
}
```

::right::

<div class="flex flex-col gap-4">
<v-clicks>

- Define infrastructure in code files
- Declarative approach
- Version controlled with Git
- Reproducible across environments
- Automated deployment pipelines

</v-clicks>
</div>

---
layout: center
class: text-center
---

# Infrastructure as Code Benefits

<div class="grid grid-cols-2 gap-4 mt-8">
<div v-click class="p-4 border rounded">
  <carbon:security class="text-3xl text-blue-500 mb-2"/>
  <h3>Consistency</h3>
  <p class="text-sm">Eliminate configuration drift</p>
</div>

<div v-click class="p-4 border rounded">
  <carbon:time class="text-3xl text-green-500 mb-2"/>
  <h3>Speed</h3>
  <p class="text-sm">Rapid infrastructure deployment</p>
</div>

<div v-click class="p-4 border rounded">
  <carbon:document class="text-3xl text-purple-500 mb-2"/>
  <h3>Scale</h3>
  <p class="text-sm">Manage complex infrastructure</p>
</div>

<div v-click class="p-4 border rounded">
  <carbon:collaborate class="text-3xl text-orange-500 mb-2"/>
  <h3>Collaboration</h3>
  <p class="text-sm">Team-wide infrastructure visibility</p>
</div>
</div>
