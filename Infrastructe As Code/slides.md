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
    Presented by Amr Awad
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

## TODO review the 2 following slides for describing IaC

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

---
layout: center
---

# The Evolution of Infrastructure as Code

<div class="fixed top-4 w-full flex justify-center">
  <div class="timeline-header flex items-center gap-8">
    <!-- Timeline items will be added dynamically -->
  </div>
</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">1976</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <vscode-icons-file-type-makefile/> Make
  </h2>
  <span class="text-gray-400 text-lg font-light">First Steps in Automation: Configuration Management</span>
</div>

::left::
<div class="mt-2 p-4">

```makefile
install:
    mkdir -p ~/myapp
    cp config.json ~/myapp/
    chmod +x ~/myapp/start.sh

configure:
    echo "PORT=3000" > ~/myapp/.env
    echo "DEBUG=true" >> ~/myapp/.env
    ./start.sh
```

</div>

::right::
<div class="mt-2 p-4 mb-4" v-click>

### Key Features {class="text-gray-400"}
<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <carbon:terminal class="text-blue-500"/>
    <span>Shell commands automation</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <carbon:document class="text-purple-500"/>
    <span>File-based operations</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <carbon:build-image class="text-orange-500"/>
    <span>Build process focus</span>
  </div>
</div>
</div>


<div class="px-4" v-click>

### Trade-offs {class="text-gray-400"}

<div class="grid grid-cols-2 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Simple syntax</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Universal tool</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Language agnostic</span>
    </div>
  </div>
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>No state tracking</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>Error-prone</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>Single machine</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---
---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">1993</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-code class="text-blue-500"/> CFEngine
  </h2>
  <span class="text-gray-400 text-lg font-light">First True Infrastructure Tool</span>
</div>

::left::
<div class="mt-2 p-4">

```
bundle agent example {
  files:
    "/etc/nginx/nginx.conf"
      perms => mog("644", "root", "root"),
      create => "true",
      edit_line => nginx_config;
      
  processes:
    "nginx"
      restart_class => "restart_nginx";
}
```

</div>

::right::
<div class="mt-2 p-4 mb-4" v-click>

### Key Features {class="text-gray-400"}
<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <material-symbols-light-handshake class="text-blue-500"/>
    <span>Promise Theory based</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <carbon-gears class="text-blue-500"/>
    <span>Self-healing systems</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
    <carbon-checkmark class="text-blue-500"/>
    <span>Continuous verification</span>
  </div>
</div>
</div>

<div class="px-4" v-click>

### Trade-offs {class="text-gray-400"}

<div class="grid grid-cols-2 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Lightweight agent</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Fast execution</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:checkmark-filled class="text-green-500"/>
      <span>True automation</span>
    </div>
  </div>
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>Steep learning curve</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>Complex syntax</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded">
      <carbon:close-filled class="text-red-500"/>
      <span>Limited adoption</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

# 2005: Configuration Management
## Puppet: Declarative Infrastructure

::left::

```ruby
package { 'nginx':
  ensure => installed
}

service { 'nginx':
  ensure  => running,
  enable  => true,
  require => Package['nginx']
}
```

::right::

<div class="mt-12">

### Key Features
- Declarative DSL
- Resource dependencies
- State management

<div v-click class="mt-8">

### Trade-offs
<div class="pros-cons-grid">
  <div class="pros">
    <div class="pros-header">✅ Pros</div>
    <ul>
      <li>Declarative approach</li>
      <li>Idempotent operations</li>
      <li>Configuration drift detection</li>
    </ul>
  </div>
  <div class="cons">
    <div class="cons-header">❌ Cons</div>
    <ul>
      <li>Required agents</li>
      <li>Complex Ruby DSL</li>
      <li>Host-level only</li>
    </ul>
  </div>
</div>

</div>
</div> 