# NGFW Engineer Practice Exam

An offline-capable practice app for the Palo Alto Networks Certified Next-Generation Firewall (NGFW) Engineer exam, built like the ISSAP, ENSLD, and AZ-900 apps.

- **240 original scenario questions**, weighted to the exam datasheet blueprint:

  | Domain | Weight | Bank | Per full exam |
  |---|---|---|---|
  | 1. PAN-OS Networking Configuration | 40% | 96 | 30 |
  | 2. PAN-OS Device Setting Configuration | 40% | 96 | 30 |
  | 3. Integration and Automation | 20% | 48 | 15 |

- **Full practice exam**: 75 questions, 90-minute timer, flag and review, scored at the end. Palo Alto doesn't publish a pass mark, so aim for 75%+ here.
- **5-question test**: timed (5 min), scored at the end.
- **Quick practice / domain drills / missed questions**: 5, 10, 20, 50, or all at a time, unseen questions first, explanation after each answer.
- Exam or study mode for the full exam and 5-question test.
- Progress is saved in the browser, with backup and restore as copy-paste text.
- Installable as a home-screen app (PWA) and works offline after the first load.

Coverage follows the datasheet task list: interfaces, zones, HA, routing and the Advanced Routing Engine, GlobalProtect, IPSec (including quantum-resistant IKEv2) and GRE; authentication, VSYS, logging and Strata Logging Service, software updates, certificates and decryption, User-ID and the Cloud Identity Engine, and the PAN-OS web proxy; PA/VM/CN-Series, Cloud NGFW, AI Runtime Security, XML and REST APIs, Terraform and Ansible, Panorama, and ACC/reports.

Questions use scenario stems, CLI and API snippets, multi-select items, and close distractors. Every question has an explanation covering why the other answers are wrong.

## Files

- `index.html`: the app
- `bank/d1a.js` to `bank/d3.js`: the question bank (`{id, d, q, o, a, e}`; `a` is the index of the correct option, and options are shuffled at display time)
- `sw.js`, `manifest.webmanifest`, `icon-*.png`: offline support and app install

Host it with GitHub Pages (Settings → Pages → deploy from branch) or open `index.html` from any static web server.

Questions are original study material, not exam dumps.
