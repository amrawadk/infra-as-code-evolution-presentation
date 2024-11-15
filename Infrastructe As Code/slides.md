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

## TODO add an intro slide

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
</div>

::left::
<div class="mt-2 p-4 h-[80vh]">

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

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
    <carbon:terminal class="text-blue-500"/>
    <span>Configuration Management</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
    <carbon:document class="text-purple-500"/>
    <span>Utilizes shell commands</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
    <carbon:build-image class="text-orange-500"/>
    <span>Focuses on build processes</span>
  </div>
</div>
</div>


<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Simple syntax</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Runs on any Unix system.</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>No state tracking</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded"  v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Single machine</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">1993</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-code class="text-blue-500"/> CFEngine
  </h2>
</div>

::left::
<div class="mt-2 p-4 h-[80vh]">

```ts
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
<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-gears class="text-blue-500"/>
    <span>Built by Mark Burgess while pursuing a postdoctorate in theoritical physics</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-checkmark class="text-blue-500"/>
    <span>Enables managing multiple Unix workstations</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <material-symbols-light-handshake class="text-blue-500"/>
    <span>Introduced a declarative DSL to manage complexity</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Multiple machines with a lightweight agent</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Steep learning curve due to complex syntax</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Limited adoption</span>
    </div>
  </div>
</div>

</div>


---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2000-2006</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-growth class="text-blue-500"/> The Scale Problem
  </h2>
</div>

::left::
<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-gray-400">
    <h3 class="font-bold text-gray-400">Traditional Approach</h3>
    <ul class="mt-2 text-sm">
      <li>Buy physical servers</li>
      <li>Set up in data centers</li>
      <li>Long procurement cycles</li>
      <li>High upfront costs</li>
    </ul>
  </div>

  <div v-click class="p-4 border rounded border-gray-400">
    <h3 class="font-bold text-gray-400">Growing Demands</h3>
    <ul class="mt-2 text-sm">
      <li>Internet boom</li>
      <li>Web-scale applications</li>
      <li>Need for rapid scaling</li>
    </ul>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div class="p-4 border rounded border-gray-400" v-click>
    <h3 class="font-bold flex items-center gap-2 text-gray-400">
      <carbon-cloud class="text-blue-500"/> Enter AWS EC2 (2006)
    </h3>
    <ul class="mt-2 text-sm">
      <li>Virtual machines on demand</li>
      <li>Pay-as-you-go model</li>
      <li>Minutes vs. months to deploy</li>
      <li>Democratized scaling</li>
    </ul>
  </div>

  <div class="text-sm text-gray-400 mt-4" v-click>
    Infrastructure scaling became everyone's challenge, not just large enterprises ...
  </div>
</div>

</div>



---
layout: two-cols-header
---


<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2005</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <logos-puppet-icon class="text-blue-500"/> Puppet
  </h2>
</div>


::left::

<div class="mt-2 p-4 h-[80vh]">

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

</div>


::right::


<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-gears class="text-blue-500"/>
    <span>Declarative DSL</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <material-symbols-light-handshake class="text-blue-500"/>
    <span>State Management</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Idempotent Operations</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Configuration Drift Detection</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Much simpler than CF Engine</span>
    </div>
  </div>
</div>

</div>

