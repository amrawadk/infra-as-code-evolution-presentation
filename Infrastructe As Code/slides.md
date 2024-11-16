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

## From Scripts to Strategy {.text-gray-400 .mb-8}
# The Past, Present, and Future of Infrastructure as Code

<div class="pt-12 flex items-center justify-center gap-4">
  <img
    class="w-24 h-24 rounded-full"
    src="https://prod-files-secure.s3.us-west-2.amazonaws.com/9abbeb10-a6cd-4555-b807-0a131d43477d/88153554-d72e-4b28-a1b8-2464516d8baf/public.avif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45GO43JXI4%2F20241115%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20241115T120051Z&X-Amz-Expires=86400&X-Amz-Signature=2da2482259084b3f6cc602b9d7f3ff463de02c53de5aa51c62c84786c9cfbf75&X-Amz-SignedHeaders=host&x-id=GetObject"
    alt="Amr Awad"
  />
  <div class="flex flex-col items-start">
    <span class="text-2xl">Amr Awad</span>
    <span class="text-gray-400">Staff Software Engineer @ Cur8 Capital</span>
  </div>
</div>

---
layout: two-cols
cols: 1-2
---

<div class="flex flex-col items-center w-full">
  <img
    class="w-48 h-48 rounded-full mb-4"
    src="https://prod-files-secure.s3.us-west-2.amazonaws.com/9abbeb10-a6cd-4555-b807-0a131d43477d/88153554-d72e-4b28-a1b8-2464516d8baf/public.avif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45GO43JXI4%2F20241115%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20241115T120051Z&X-Amz-Expires=86400&X-Amz-Signature=2da2482259084b3f6cc602b9d7f3ff463de02c53de5aa51c62c84786c9cfbf75&X-Amz-SignedHeaders=host&x-id=GetObject"
    alt="Amr Awad"
  />
  
  <h1 class="text-2xl font-bold mb-8">Amr Awad</h1>

  <div class="mt-8 flex flex-col gap-4">
    <a href="https://www.linkedin.com/in/amrawadk" target="_blank" class="text-gray-500 hover:text-blue-500">
      <carbon-logo-linkedin class="text-2xl"/>
      Linkedin
    </a>
    <a href="mailto:hello@amrawad.com" class="text-gray-500 hover:text-gray-700">
      <carbon-email class="text-2xl"/>
      hello@amrawad.com
    </a>
    <a href="https://adplist.org/mentors/amr-awad" target="_blank" class="text-gray-500 hover:text-purple-500">
      <material-symbols-light:school-rounded class="text-2xl"/>
      Adplist
    </a>
  </div>
</div>

::right::



<div class="flex flex-col gap-2">

  <h3 class="text-sm tracking-wide text-blue-400 font-semibold">Currently</h3>

  <div class="flex flex-col gap-1 mb-2">
    <div class="flex items-center gap-1">
      <carbon-development class="text-blue-500 inline"/> 
      <span>Staff Software Engineer @ Cur8 Capital</span>
    </div>
    <div class="text-sm text-gray-400">
      Building a sharia compliant investment platform
    </div>
  </div>

  <div class="flex flex-col gap-1 mb-2" v-click>
    <div class="flex items-center gap-1">
      <carbon-application class="text-orange-500 inline"/>
      <span>Founder @ Lunchflow</span>
    </div>
    <div class="text-sm text-gray-400">
      Built a SaaS app connecting UK & EU banks to Lunch Money using Open Banking.
    </div>
  </div>

  <h3 class="text-sm text-blue-400 tracking-wide font-semibold" v-click>Previously</h3>

  <div class="flex flex-col gap-1 mb-2" v-click>
    <div class="flex items-center gap-2">
      <carbon-rocket class="text-green-500 inline"/>
      <span>Founding Engineer @ Tempo (YC W15)</span>
    </div>
    <div class="flex flex-col gap-2 text-sm text-gray-400">
      <div class="flex items-center gap-2">
        <span>First full-time employee. Helped scale the company to 250+ people and raise $300M+ in funding.</span>
      </div>
    </div>
  </div>


  <div class="flex flex-col gap-1 mb-2" v-click>
  <div class="flex items-center gap-2">
    <material-symbols-light:school-rounded class="text-purple-500 inline"/>
    <span>Top Rated Freelancer @ Upwork</span>
  </div>
  <div class="text-sm text-gray-400">
    <div class="flex flex-col gap-1">
      <span>Working across multiple domains, including: machine learning, computer vision, cloud architecture and DevOps.</span>
    </div>
  </div>
  </div>

  <div class="flex flex-col gap-1" v-click>
    <div class="flex items-center gap-1">
      <carbon-car class="text-blue-500 inline"/>
      <span>Embedded Software Engineer @ Valeo</span>
    </div>
    <div class="text-sm text-gray-400">
      <div class="flex flex-col gap-1">
        <span>Developed software for autonomous driving systems and advanced driver assistance features.</span>
      </div>
    </div>
  </div>
</div>




---

## TODO add slide numbers

---
layout: center
---

# Agenda

<v-clicks>

- What is Infrastructure as Code (IaC)?
- The Evolution of IaC
- Next Generation of IaC tooling
- Making the Right Choice

</v-clicks>

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

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2009</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <vscode-icons-file-type-chef class="text-red-500"/> Chef
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```ruby
package 'nginx' do
  action :install
end

template '/etc/nginx/nginx.conf' do
  source 'nginx.conf.erb'
  owner 'root'
  group 'root'
  mode '0644'
  notifies :restart, 'service[nginx]'
end

service 'nginx' do
  action [:enable, :start]
  supports status: true, restart: true, reload: true
end
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <logos-ruby class="text-red-500"/>
    <span>Full Ruby DSL</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-code class="text-blue-500"/>
    <span>Procedural approach to configuration</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-development class="text-green-500"/>
    <span>Developer-friendly workflow</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Powerful Ruby programming model</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Rich ecosystem of cookbooks</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Steeper learning curve for non-developers</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2012</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <vscode-icons-file-type-ansible class="text-red-500"/> Ansible
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```yaml
- name: Configure web server
  hosts: webservers
  tasks:
    - name: Install nginx
      apt:
        name: nginx
        state: present

    - name: Start nginx
      service:
        name: nginx
        state: started
        enabled: yes
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-connect class="text-blue-500"/>
    <span>Agentless (SSH-based)</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <vscode-icons-file-type-yaml class="text-green-500"/>
    <span>YAML-based declarative syntax</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>No agent installation required</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Simple, readable YAML syntax</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Lower barrier to entry</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2010-2014</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-cloud-services class="text-blue-500"/> The Cloud Native Shift
  </h2>
</div>

::left::
<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-gray-400">
    <h3 class="font-bold text-gray-400">First Generation</h3>
    <ul class="mt-2 text-sm">
      <li>Configure individual machines</li>
      <li>Install and manage software</li>
      <li>Handle system dependencies</li>
      <li>Maintain running services</li>
    </ul>
  </div>

  <div v-click class="p-4 border rounded border-blue-400">
    <h3 class="font-bold text-blue-400">Second Generation</h3>
    <ul class="mt-2 text-sm">
      <li>Declare cloud resources</li>
      <li>Use managed services</li>
      <li>Higher-level abstractions</li>
      <li>Cloud provider handles operations</li>
    </ul>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div class="p-4 border rounded border-gray-400" v-click>
    <h3 class="font-bold flex items-center gap-2 text-gray-400">
      <carbon-cloud-app class="text-blue-500"/> Key Changes
    </h3>
    <ul class="mt-2 text-sm">
      <li>SNS instead of ZeroMQ</li>
      <li>RDS instead of PostgreSQL setup</li>
      <li>S3 instead of file systems</li>
      <li>Lambda instead of process management</li>
    </ul>
  </div>

  <div class="p-4 border rounded border-gray-400" v-click>
    <h3 class="font-bold flex items-center gap-2 text-gray-400">
      <carbon-development class="text-green-500"/> Resource-Oriented
    </h3>
    <div class="text-sm mt-2">
      <p>Infrastructure defined as a collection of managed resources rather than configuration steps</p>
    </div>
  </div>

  <div class="text-sm text-gray-400 mt-2" v-click>
    The focus shifted from "how to run services" to "which services do we need?" ...
  </div>
</div>

</div>

// ... existing code ...

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2011</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 mt-2">
    <logos-aws/> CloudFormation
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```yaml
Resources:
  WebServerInstance:
    Type: AWS::EC2::Instance
    Properties:
      ImageId: ami-0c55b159cbfafe1f0
      InstanceType: t2.micro
      SecurityGroups:
        - !Ref WebServerSecurityGroup
      UserData: 
        Fn::Base64: !Sub |
          #!/bin/bash
          yum update -y
          yum install -y httpd

  WebServerSecurityGroup:
    Type: AWS::EC2::SecurityGroup
    Properties:
      GroupDescription: Enable HTTP access
      SecurityGroupIngress:
        - IpProtocol: tcp
          FromPort: 80
          ToPort: 80
          CidrIp: 0.0.0.0/0
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud class="text-orange-500"/>
    <span>Native AWS Integration</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-template class="text-blue-500"/>
    <span>JSON/YAML Templates</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-flow class="text-green-500"/>
    <span>Built-in State Management</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Deep AWS Integration</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Automatic Rollbacks</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>AWS-only</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Complex Template Syntax</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2014</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 mt-2">
    <logos-terraform-icon class="text-purple-500"/> Terraform
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```hcl
provider "aws" {
  region = "us-west-2"
}

resource "aws_instance" "web" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"

  tags = {
    Name = "WebServer"
  }
}

resource "aws_security_group" "allow_http" {
  name        = "allow_http"
  description = "Allow HTTP inbound traffic"

  ingress {
    from_port   = 80
    to_port     = 80
    protocol    = "tcp"
    cidr_blocks = ["0.0.0.0/0"]
  }
}
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud-satellite class="text-purple-500"/>
    <span>Multi-Cloud Support</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-code class="text-blue-500"/>
    <span>HCL Configuration Language</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <vscode-icons-file-type-graphql class="text-green-500"/>
    <span>Resource Graph & Planning</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Provider-agnostic</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Clear State Management</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Rich Provider Ecosystem</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>State File Management</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2014-2018</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-warning class="text-yellow-500"/> Declarative Cloud Challenges
  </h2>
</div>

::left::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-yellow-400">
    <h3 class="font-bold flex items-center gap-2 text-yellow-400">
      <carbon-code class="text-yellow-500"/> Custom DSL Limitations
    </h3>
    <ul class="mt-2 text-sm">
      <li>No general-purpose programming facilities</li>
      <li>Limited code reuse capabilities</li>
      <li>Difficult to implement complex logic</li>
      <li>Poor developer experience</li>
    </ul>
  </div>

  <div v-click class="p-4 border rounded border-orange-400">
    <h3 class="font-bold flex items-center gap-2 text-orange-400">
      <carbon-document class="text-orange-500"/> Verbose Configuration
    </h3>
    <ul class="mt-2 text-sm">
      <li>Full resource configuration required</li>
      <li>Complex 'glue' configurations (IAM, networking)</li>
      <li>Limited abstraction capabilities</li>
      <li>Repetitive boilerplate code</li>
    </ul>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">

  <div class="p-4 border rounded border-gray-400" v-click>
    <h3 class="font-bold flex items-center gap-2 text-gray-400">
      <carbon-development class="text-green-500"/> What Was Needed
    </h3>
    <ul class="mt-2 text-sm">
      <li>Programming language constructs</li>
      <li>Better abstraction capabilities</li>
      <li>Reusable components</li>
      <li>Modern development workflows</li>
    </ul>
  </div>

  <div class="text-sm text-gray-400 mt-2" v-click>
    These limitations led to the rise of the next generation of infrastructure as code tooling ...
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2018-Present</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-code class="text-blue-500"/> Infrastructure as Software
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-blue-400">
    <h3 class="font-bold text-blue-400">Key Characteristics</h3>
    <ul class="mt-2 text-sm">
      <li>General-purpose programming languages</li>
      <li>Object-oriented abstractions</li>
      <li>Package management</li>
      <li>Modern IDE support</li>
    </ul>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">
  <div v-click class="p-4 border rounded border-green-400">
    <h3 class="font-bold text-green-400">Benefits</h3>
    <ul class="mt-2 text-sm">
      <li>Shareable components</li>
      <li>Type safety</li>
      <li>Unit testing</li>
      <li>Code reuse</li>
    </ul>
  </div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2019</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <logos-aws class="text-orange-500"/> AWS CDK
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
import * as cdk from 'aws-cdk-lib';
import * as lambda from 'aws-cdk-lib/aws-lambda';
import * as apigateway from 'aws-cdk-lib/aws-apigateway';

export class ApiStack extends cdk.Stack {
  constructor(scope: cdk.App, id: string, props?: cdk.StackProps) {
    super(scope, id, props);

    // Create Lambda function
    const handler = new lambda.Function(this, 'Handler', {
      runtime: lambda.Runtime.NODEJS_18_X,
      code: lambda.Code.fromAsset('lambda'),
      handler: 'handler.main',
    });

    // Create API Gateway
    const api = new apigateway.RestApi(this, 'Api');
    api.root.addMethod('GET', 
      new apigateway.LambdaIntegration(handler));
  }
}
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <logos-typescript-icon class="text-blue-500"/>
    <span>TypeScript-first Development</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-package class="text-green-500"/>
    <a href="https://constructs.dev" target="_blank">
      <span>Constructs Ecosystem</span>
    </a>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud class="text-orange-500"/>
    <span>CloudFormation Under the Hood</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Full Programming Language Power</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Type Safety & IDE Support</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>AWS-only</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>All Cloudformation issues</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2018</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <vscode-icons-file-type-pulumi class="text-purple-500"/> Pulumi
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

const bucket = new aws.s3.Bucket("my-bucket");

const lambdaRole = new aws.iam.Role("lambdaRole", {
    assumeRolePolicy: aws.iam.assumeRolePolicyForPrincipal({
        Service: "lambda.amazonaws.com"
    }),
});

const lambda = new aws.lambda.Function("myLambda", {
    code: new pulumi.asset.AssetArchive({
        ".": new pulumi.asset.FileArchive("./app"),
    }),
    role: lambdaRole.arn,
    handler: "index.handler",
    runtime: "nodejs18.x",
});
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud-satellite class="text-purple-500"/>
    <span>Multi-Cloud Native</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-code class="text-blue-500"/>
    <span>Multiple Language Support</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Provider-agnostic</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Language Choice Flexibility</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Learning Curve</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">2020</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <vscode-icons-file-type-sst class="text-orange-500"/> SST (Serverless Stack)
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
import { StackContext, Api, Auth } from "@serverless-stack/resources";

export function MyStack({ stack }: StackContext) {
  const auth = new Auth(stack, "auth", {
    login: ["email"],
  });

  const api = new Api(stack, "api", {
    authorizer: "iam",
    routes: {
      "GET  /notes": "functions/list.main",
      "POST /notes": "functions/create.main",
    },
  });

  auth.attachPermissionsToUser(api);

  return {
    api: api.url,
    auth: auth.auth.userPoolId,
  };
}
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-application class="text-blue-500"/>
    <span>Higher-level Abstractions</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-development class="text-green-500"/>
    <span>Live Lambda Development</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud class="text-orange-500"/>
    <span>Initially built on AWS CDK, but recently <a href="https://www.pulumi.com/blog/from-cdk-pulumi-evolution-of-sst/" target="_blank">
      migrated to Pulumi.
    </a></span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Higher-Level Abstractions</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Developer Experience Focus</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">Present Day</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-road class="text-blue-500"/> The Road Ahead
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-orange-400">
    <h3 class="font-bold flex items-center gap-2 text-orange-400">
      <carbon-warning class="text-orange-500"/> Current Limitations
    </h3>
    <ul class="mt-2 text-sm">
      <li>Service-level abstractions only</li>
      <li>Deep cloud service knowledge required</li>
      <li>Infrastructure isolated from application code</li>
      <li>Complex deployment coordination</li>
    </ul>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-blue-400">
    <h3 class="font-bold flex items-center gap-2 text-blue-400">
      <carbon-idea class="text-blue-500"/> What We Need
    </h3>
    <ul class="mt-2 text-sm">
      <li>Business-level abstractions</li>
      <li>Closer integration with application code</li>
      <li>Intent-based infrastructure</li>
      <li>Unified deployment workflows</li>
    </ul>
  </div>

  <div class="text-sm text-gray-400 mt-4" v-click>
    Moving towards infrastructure that adapts to your application's needs...
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">Next Generation</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-code class="text-purple-500"/> New Programming Languages
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```ts
bring cloud;

let api = new cloud.Api();
let bucket = new cloud.Bucket();

api.get("/files", inflight (req) => {
  let files = bucket.list();
  return {
    status: 200,
    body: files
  };
});

api.post("/files", inflight (req) => {
  let key = req.body.key;
  let data = req.body.data;
  bucket.put(key, data);
  return {
    status: 201
  };
});
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 my-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud class="text-green-500"/>
    <span>Cloud-native by design</span>
  </div>
</div>


### Examples {class="text-gray-400" v-click}

<div class="flex flex-col gap-2 mt-4">

  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <logos-winglang-icon class="text-blue-500"/>
    <span>Wing Language</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <material-symbols-light-dark-mode-rounded class="text-purple-500"/>
    <span>Darklang</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Purpose-built for cloud</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Enhanced development experience</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>New language learning curve</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Limited ecosystem</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">Next Generation</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-api class="text-blue-500"/> SDK-Based Approach
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
import { api, storage } from '@nitric/sdk'

// Create a bucket
const files = storage('files').bucket()

// Create an API
api('public').get('/files', async (ctx) => {
  const fileList = await files.list()
  return ctx.ok(fileList)
})

api('public').post('/files', async (ctx) => {
  const { key, data } = ctx.req.body
  await files.file(key).write(data)
  return ctx.created()
})
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 my-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-api-1 class="text-green-500"/>
    <span>Abstracted Cloud APIs</span>
  </div>
</div>


### Examples {class="text-gray-400" v-click}

<div class="flex flex-col gap-2 mt-4">

  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <bx-cloud-lightning class="text-blue-500"/>
    <span>Ampt</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-arrow-right class="text-purple-500"/>
    <span>Nitric</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Use existing languages</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Familiar development model</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Vendor lock-in to SDK</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Limited community ecosystem</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">Next Generation</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-code-reference class="text-green-500"/> SDK + Annotations
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
// Encore example
import { api, Cache } from 'encore'

// Define cache with annotation
@cache({ ttl: '24h' })
class FileCache {
  async list(): Promise<File[]> {
    // ... implementation
  }
}

// Define API endpoint
@api.get('/files')
async function getFiles() {
  const files = await cache.list()
  return { files }
}
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-development class="text-green-500"/>
    <span>Rich Development Experience</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-cloud class="text-orange-500"/>
    <span>Infrastructure Generation</span>
  </div>
</div>
</div>

<div class="px-4">

### Examples {class="text-gray-400" v-click}

<div class="flex gap-6 my-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <div class="text-blue-500 font-bold text-lg">e</div>
    <span>Encore</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-rocket />
    <span>Shuttle</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <logos-aws />
    <span>AWS Chalice</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Framework-style development</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Strong developer tooling</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Double learning curve</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Framework lock-in</span>
    </div>
  </div>
</div>

</div>

---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <span class="text-gray-400 text-sm tracking-wide">Next Generation</span>
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-intent-request-scale-out class="text-orange-500"/> Pure Annotations
  </h2>
</div>

::left::

<div class="mt-2 p-4 h-[80vh]">

```typescript
import { S3 } from 'aws-sdk'
import express from 'express'

// @klotho::persist {
//   id = "files"
//   type = "object-store"
// }
const files = new S3()

// @klotho::expose {
//   id = "public-api"
//   type = "http"
// }
app.get('/files', async (req, res) => {
  const fileList = await files.listObjects().promise()
  res.json(fileList)
})
```

</div>

::right::

<div class="mt-2 p-4 mb-4">

<div class="flex flex-col gap-2 mt-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-intent-request-scale-out class="text-blue-500"/>
    <span>Architecture from Code</span>
  </div>
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-code class="text-orange-500"/>
    <span>Native SDK Usage</span>
  </div>
</div>
</div>

<div class="px-4">

### Examples {class="text-gray-400" v-click}

<div class="flex flex-col gap-2 my-4">
  <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
    <carbon-intent-request-scale-out class="text-blue-500"/>
    <span>Klotho</span>
  </div>
</div>
</div>

<div class="px-4">

### Trade-offs {class="text-gray-400" v-click}

<div class="grid grid-cols-1 gap-4 mt-4">
  <div class="flex flex-col gap-2">
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Use native cloud SDKs</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Minimal learning curve</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:checkmark-filled class="text-green-500"/>
      <span>Architecture-level abstractions</span>
    </div>
    <div class="flex items-center gap-2 hover:bg-gray-50 rounded" v-click>
      <carbon:close-filled class="text-red-500"/>
      <span>Limited infrastructure control</span>
    </div>
  </div>
</div>

</div>

---
layout: center
---

# Let's recap

---
layout: center
---

# Evolution of Infrastructure as Code

<v-clicks>

- **2005-2010: Configuration Management** {.text-orange-500}
  - <carbon-bare-metal-server class="text-orange-500 inline mb-1"/> CFEngine, Puppet, Chef, Ansible
  - <carbon-settings class="text-orange-400 inline mb-1"/> Focus on server configuration and management

- **2011-2017: Declarative Cloud** {.text-blue-500}
  - <carbon-cloud class="text-blue-500 inline mb-1"/> CloudFormation, Terraform, ARM Templates
  - <carbon-document class="text-blue-400 inline mb-1"/> Cloud resource definitions in YAML, JSON, HCL

- **2018-2022: Infrastructure as Software** {.text-purple-500}
  - <carbon-code class="text-purple-500 inline mb-1"/> AWS CDK, Pulumi, SST
  - <carbon-application class="text-purple-400 inline mb-1"/> Programming languages for infrastructure

- **2023+: Infrastructure from Code** {.text-green-500}
  - <carbon-code-reference class="text-green-500 inline mb-1"/> Wing, Nitric, Encore, Klotho
  - <carbon-intent-request-scale-out class="text-green-400 inline mb-1"/> Infrastructure derived from application code

</v-clicks>

---
layout: center
---

# Key Trends in Infrastructure as Code

<br>

<v-clicks>

- **Higher Abstractions** {.text-green-500}
  - <carbon-arrow-up class="text-green-500 inline mb-1"/> From server configs to business logic
  - <carbon-chart-relationship class="text-green-400 inline mb-1"/> Increasing levels of abstraction

- **Better Developer Experience** {.text-blue-500}
  - <carbon-development class="text-blue-500 inline mb-1"/> Modern development workflows
  - <carbon-tools class="text-blue-400 inline mb-1"/> Rich tooling and IDE support

- **Closer to Application Code** {.text-purple-500}
  - <carbon-integration class="text-purple-500 inline mb-1"/> Unified development experience
  - <carbon-code-reference class="text-purple-400 inline mb-1"/> Infrastructure derived from intent

</v-clicks>
---
layout: two-cols-header
---

<div class="flex flex-col items-start">
  <h2 class="text-3xl font-bold flex items-center gap-2 my-2">
    <carbon-decision-tree class="text-blue-500"/> When to Choose What?
  </h2>
  <span class="text-gray-400 text-sm tracking-wide">Lessons learned the hard way</span>
</div>

::left::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-green-400">
    <h3 class="font-bold flex items-center gap-2 text-green-400">
      <carbon-group class="text-green-500"/> Small Teams
    </h3>
    <div class="mt-2">
      <div class="flex items-center gap-2 mb-2" v-click>
        <material-symbols-light:shield-question-rounded/>
        <span class="font-semibold">Is infrastructure a core differentiator?</span>
      </div>
      <div class="ml-6" v-click>
        <div class="text-sm mb-2">If no, consider managed platforms, such as:</div>
        <ul class="text-sm list-disc ml-4">
          <li>Digital Ocean App Platform</li>
          <li>Vercel</li>
          <li>Netlify</li>
        </ul>
      </div>
    </div>
  </div>
  <div v-click class="p-4 border rounded border-blue-400">
    <h3 class="font-bold flex items-center gap-2 text-blue-400">
      <carbon-currency class="text-blue-500"/> Growing Teams
    </h3>
    <div class="mt-2">
      <div class="text-sm mb-2">When costs increase:</div>
      <ul class="text-sm list-disc ml-4">
        <li>Choose tools in your app's language, like CDK or Pulumi</li>
        <li>Focus on developer productivity</li>
      </ul>
    </div>
  </div>
</div>

</div>

::right::

<div class="mt-2 p-4">

<div class="flex flex-col gap-4">
  <div v-click class="p-4 border rounded border-purple-400">
    <h3 class="font-bold flex items-center gap-2 text-purple-400">
      <carbon-enterprise class="text-purple-500"/> Enterprise
    </h3>
    <div class="mt-2">
      <div class="text-sm mb-2">Key considerations:</div>
      <ul class="text-sm list-disc ml-4">
        <li>Developer tooling & standards</li>
        <li>Licensing & compliance</li>
        <li>Team training & support</li>
        <li>Multi-cloud strategy</li>
      </ul>
    </div>
  </div>

  <div class="text-sm text-gray-400" v-click>
  Remember: The best tool is often the one that lets your team ship value fastest ...
</div>
</div>
</div>


---
layout: center
---

# Questions? 😀

---
layout: center
---

# Resources

<v-clicks>

- **Historical Evolution** {.text-orange-500}
  - <carbon-document class="text-orange-500 inline mb-1"/> ["A Brief DevOps History: The Roots of Infrastructure as Code"](https://thenewstack.io/a-brief-devops-history-the-roots-of-infrastructure-as-code/)
  - <carbon-time class="text-orange-400 inline mb-1"/> Comprehensive timeline from Make (1976) to modern tools

- **Technical Deep Dive** {.text-blue-500}
  - <carbon-book class="text-blue-500 inline mb-1"/> ["History and Future of Infrastructure as Code"](https://www.endoflineblog.com/history-and-future-of-infrastructure-as-code)
  - <carbon-growth class="text-blue-400 inline mb-1"/> Detailed analysis of IaC generations and their characteristics

- **Next Generation Approaches** {.text-purple-500}
  - <carbon-rocket class="text-purple-500 inline mb-1"/> ["State of Infrastructure from Code 2023"](https://klo.dev/state-of-infrastructure-from-code-2023/)
  - <carbon-development class="text-purple-400 inline mb-1"/> Comprehensive overview of modern IaC approaches

- **Cloud Evolution** {.text-green-500}
  - <carbon-cloud class="text-green-500 inline mb-1"/> ["10 Years of Cloud Infrastructure as Code"](https://medium.com/nordhero/10-years-of-cloud-infrastructure-as-code-history-and-trends-d307f8c4ce31)
  - <carbon-analytics class="text-green-400 inline mb-1"/> Focus on serverless and modern cloud patterns

</v-clicks>
