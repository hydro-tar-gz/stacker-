# 🧰 Stacker Suite  
### *“Your server setup shouldn’t feel like dark magic.”*

Stacker Suite is an ambitious little toolbox that aims to take all the annoying, repetitive, error-prone parts of deploying a website on a Linux server…  
and blows it up to piexes

No more sacrificing goats to appease Nginx.  
No more “why does Node version 16 break everything?”  
No more forgetting to renew your certs and waking up to 37 angry emails.

---

## ⁉️ What the heck **is** Stacker Suite?

Imagine three programs had a baby:

- **archinstall** → for guided wizard setup  
- **oh-my-zsh** → for plugins / packs / customizable goodness  
- **nvm** → but built for *production*, not just “works on my laptop” vibes

Now give that baby caffeine, a Linux server, and root access.

Stacker Suite’s goal is to make deploying web projects feel effortless, predictable, and maybe even… fun?

---

## ✨ Features We’re Cooking (a.k.a. The Wishlist)

- 🧠 **Smart OS & project detection**  
  It sniffs out your Linux distro, figures out what kind of project you’re running, and points out problems before they explode.

- 🧙 **Guided installation wizard**  
  Like archinstall, but for setting up Node, PM2/systemd, Nginx/Caddy, certs, folders, etc.

- 📦 **Config-as-code with `stacker.yml`**  
  “Describe what you want, then let Stacker do the heavy lifting.”

- 🔧 **Production-safe Node version manager**  
  Like nvm, but without breaking your systemd services or ghosting your binary paths.

- 🔥 **Automatic Nginx/Caddy config generation**  
  Reverse proxies, HTTPS redirects, headers… all handled.

- 🔒 **Let’s Encrypt / Certbot integration**  
  TLS certificates, auto-renewed, with status reports.

- ⚙️ **Process management**  
  PM2 or systemd — whichever your app needs.

- 💉 **Stacker Doctor**  
  A full diagnostic command that checks DNS, TLS, firewall, Nginx, Node versions, PM2, disk space, and vibes.

- 📈 **Web dashboard**  
  A shiny browser UI where you can see:
  - sites  
  - domains  
  - cert expiry  
  - server health  
  - updates  
  - logs  
  - your life choices  

- 🎛️ **Update agent**  
  Watches versions, packages, certs, and lets you safely update things (with zero “surprise Node upgrades” madness).

- 🔗 **GitHub integration**  
  PR checks, auth, approvals, and automated “stacker plan” reports.

- 🧩 **Plugin/Packs system**  
  Want Postgres? Redis? Next.js SSR? Add a pack and go wild.

---

## 🧪 Example Commands

```text
stacker init          # Generate stacker.yml (wizard mode optional)
stacker detect        # Sniffs your project + OS
stacker plan          # Dry-run + linter + "what will change?"
stacker apply         # Make it real

stacker add domain    # Add domain config
stacker add db        # Add a database entry
stacker add env       # Add environment variables

stacker update check  # Show available updates
stacker update apply  # Apply safe updates only

stacker auth github   # Connect GitHub for PR checks
stacker web           # Open the dashboard
stacker doctor        # Diagnose Everything™



## why does this exist?

I hate setting up servers.
