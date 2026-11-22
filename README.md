# VPS with cPanel: Is the License Included or Billed Extra, How Long Until You Can Log In, and Which Plan Do You Need? (Ava Hosting Plans, Prices and the Self-Managed Checklist)

A VPS with cPanel is two purchases on one invoice: the server, and the panel licence that runs on it. Hosts quote that second part in three different ways, and at the same spec level the difference between "included" and "added at checkout" can be tens of euros a month. Ava Hosting (AvaHost) lists the licence separately from the VPS, with servers from €5.00/month for 1 vCPU, 2 GB RAM and 25 GB NVMe. Below are all seven plans and their prices, how the licence is charged, what happens between payment and your first WHM login, and the work that becomes yours once the server is handed over.

> **Short answer for most readers:** VPS Basic at €10.00/month (2 vCPU, 4 GB RAM, 50 GB NVMe) is the cheapest plan here with enough memory to run cPanel and WHM without constant swapping. VPS One at €5.00 makes sense for one or two low-traffic sites. Confirm the licence figure in the cart before you pay, because it is not printed on the plan cards. 👉 [See Ava Hosting's current VPS plans and prices](https://my.ava.hosting/aff.php?aff=15562)

## All Ava Hosting VPS plans

Prices are in euros as published on the VPS plan page. Six plans are quoted monthly; VPS Nano is quoted per year.

| Plan | vCPU / RAM / NVMe | Port speed | Price (EUR) | Order |
| --- | --- | --- | --- | --- |
| VPS Nano | 1 / 512 MB / 20 GB | 100 Mbps | €11.00 per year | [Order VPS Nano](https://my.ava.hosting/aff.php?aff=15562) |
| VPS One | 1 / 2 GB / 25 GB | 1 Gbps | €5.00/month | [Order VPS One](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Basic | 2 / 4 GB / 50 GB | 1 Gbps | €10.00/month | [Order VPS Basic](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Lucky | 2 / 6 GB / 70 GB | 1 Gbps | €15.00/month | [Order VPS Lucky](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Power | 4 / 8 GB / 90 GB | 1 Gbps | €20.00/month | [Order VPS Power](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Extra | 6 / 12 GB / 120 GB | 1 Gbps | €30.00/month | [Order VPS Extra](https://my.ava.hosting/aff.php?aff=15562) |
| VPS Ultra | 8 / 16 GB / 160 GB | 1 Gbps | €40.00/month | [Order VPS Ultra](https://my.ava.hosting/aff.php?aff=15562) |

Every plan on that list carries the same baseline: unlimited traffic, free DDoS protection, weekly backups, full root access, a dedicated IPv4 address, 99.9% uptime SLA and 24/7 support, running KVM virtualisation on Intel Xeon E5 hardware with NVMe storage.

Two details on the list matter more than they look. VPS Nano is the only plan with a 100 Mbps port, and its feature list marks port 25 as closed, so outbound mail from that box is restricted. It also showed 0 available when I checked the plan page, which makes it an entry price more than a plan you can buy today. VPS One at €5.00 has 1 Gbps and no port restriction, so it is the real entry point.

The jump from VPS One to VPS Basic doubles RAM from 2 GB to 4 GB, doubles vCPU count, doubles storage and costs €5.00 more. For anything running a control panel, that is the best €5.00 in the table.

## The cPanel licence: included, itemised, or a surprise at checkout

AvaHost sells cPanel as a licensed add-on that is billed separately from the server. You add it when you order, or during a migration, and the panel arrives pre-installed on the KVM instance. The plan prices above do not include it, and the plan pages do not publish the licence amount either, so the number that decides your real monthly cost shows up at checkout.

That is one of three billing models in this market, and mixing them is the most common way people mis-cost a cPanel VPS.

**Bundled into the plan price.** Liquid Web's three cPanel VPS tiers each carry the line "Includes cPanel licensing" next to the price: $33/mo for 1 vCPU, 1 GB RAM and 30 GB storage; $45/mo for 2 vCPU, 4 GB and 80 GB; $73/mo for 4 vCPU, 8 GB and 240 GB (page dated 19 November 2024). Rad Web Hosting quotes its cPanel VPS "from as little as $52.54 USD per month (including software license)". With this model the advertised number is the whole bill, which makes comparison easy and hides how much of it is licence.

**Itemised next to the server.** Contabo prints a cPanel licence price beside every Cloud VPS tier, and the licence scales with the server: €5.50 on the 4 vCPU plan, €7.50 on the 6 vCPU, €14.00 on the 8 vCPU, €25.00 on the 12 vCPU, €37.00 on the 16 vCPU and €49.00 on the 18 vCPU. At the promotional server prices Contabo displays, the licence costs more than the server itself at every single tier. The 4 vCPU plan is €4.40/month for the first 24 months plus €5.50 for the licence, so the real outlay during the promo is €9.90/month and the licence is 56% of it.

**Priced only in the cart.** HostGator states plainly that "a cPanel license is a paid add-on, and the price depends on the tier you choose", with the current price shown in the cart before checkout. You pick a licence tier in a pop-up during the order and never see a figure on the product page.

AvaHost's model sits between the second and third: the licence is a separate line, like Contabo, but the amount is not printed on the plan card, like HostGator. The practical consequence is that a €10.00 VPS Basic and a $33.00 Liquid Web Small are not comparable numbers, because only one of them has a licence inside it. If a host will not show you the licence line before you reach payment, price the whole order in the cart and compare that.

Resellers have a fourth variable. Atlantic.Net sells licences in blocks from 5 to 500 and says the more you buy the cheaper each one gets, without publishing the discount curve. If you plan to run WHM for clients, ask what your per-account licence cost is at your expected account count, not at one account. 👉 [Start an Ava Hosting order and check the licence line](https://my.ava.hosting/aff.php?aff=15562)

## From payment to your first WHM login

Two things get measured here, and hosts blur them: how long the server takes to exist, and how long cPanel takes to install on it.

Atlantic.Net quotes provisioning a cPanel/WHM-ready VPS "in seconds" and contrasts that with 60 to 90 minutes for a self-installation (page dated 30 July 2024). Rad Web Hosting says the server is delivered instantly with its IP, but that the "cPanel installation process can be completed within 2-4 hours typically". HostGator starts setup after checkout and shows the server in the client portal's Hosting tab once ready, with no time given. So "30 seconds" means a machine with the panel image ready, and "2 to 4 hours" means cPanel itself finished installing. A vendor quoting the first number while you wait out the second is not lying, just answering a different question.

AvaHost adds cPanel at order time as a pre-installed licensed add-on rather than as something you bolt on afterwards, and its pages do not publish a provisioning time. Plan for the panel to be part of the build, and treat licence activation as the step that has to finish before WHM opens.

The first login follows the same pattern on any WHM box. Reset the root password in the client area, open the server's management page, then connect to the IP. Your browser will throw a certificate warning because the new server is using a temporary self-signed certificate; check that the IP matches the one in the portal before proceeding, and expect the warning to stay in the address bar until you install a certificate for the server hostname. Accept the terms, log in as root with the new password, and enter your cPanel Store credentials when prompted so the licence activates. Then you land in WHM.

One choice made before that login saves trouble later: the operating system. AvaHost offers AlmaLinux and Rocky Linux, CloudLinux, and Ubuntu LTS from cPanel version 110 onward. CloudLinux is the one to pick if you will host client accounts, since its CageFS and LVE limits stop one account's resource spike from taking down its neighbours. 👉 [Check the current Ava Hosting VPS offer](https://my.ava.hosting/aff.php?aff=15562)

## What "self-managed" puts on your desk

cPanel and WHM split the job in a way worth understanding before you buy. WHM is the root-level layer: it creates cPanel accounts, sets disk and bandwidth quotas, defines hosting packages, manages reseller privileges, and controls server-wide SSL, firewall and PHP handler settings. cPanel is what each end user sees, scoped to their own domains, files, databases, mail and certificates. That separation is deliberate, so a customer with a cPanel login cannot restart your server or rewrite its configuration.

On a self-managed VPS, none of the server-level work is done for you. HostGator's wording is the clearest version of the deal: you get full root access, and "you're responsible for configuring, maintaining, updating, and securing your server and software." Rad Web Hosting does not pre-configure port blocks or a firewall on its cPanel VPS and points customers to the CSF plugin for a graphical firewall interface. Atlantic.Net includes one IPv4 address per server and charges $3.65/month for each additional one.

AvaHost bundles a few of those items into the plan price: the dedicated IPv4 is included, weekly backups are included, and DDoS protection is included. CSF and ModSecurity integration are handled from inside WHM. What is not included is the part people underestimate: OS patching, PHP and MySQL version upgrades, firewall rules, spam filtering tuned to your mail volume, and a restore plan you have actually tested.

That is the honest filter for this purchase. If you can read an SSH session, are willing to keep a patching routine, and know what to do when a site hits a PHP memory limit, a €10 to €20 self-managed VPS with cPanel is excellent value. If you want someone else to own kernel updates and incident response, the Ava Hosting pages reviewed describe self-managed KVM only and do not document a managed tier, so confirm that with support before you order rather than after.

## Price anchors from other hosts

Recorded prices, not live quotes. Two of these pages carry dates that are now over two years old, so treat the numbers as reference points rather than what you would pay today.

| Provider | Entry cPanel plan | Recorded price | Page date |
| --- | --- | --- | --- |
| Liquid Web | Small: 1 vCPU, 1 GB, 30 GB, licence included | $33/mo | 19 Nov 2024 |
| Rad Web Hosting | cPanel VPS, enterprise SSD on RAID 10, licence included | from $52.54/mo | undated |
| Contabo | Cloud VPS 4: 4 vCPU, 8 GB, 100 GB, plus €5.50 licence | €4.40/mo for first 24 months + licence | undated |

Two things to take from that table. Contabo's €4.40 is a first-24-months promotional rate and the page does not show a renewal price, so it cannot be treated as a long-term monthly cost. And the two bundled hosts start where they start because a licence is inside the number, which is why their entry prices sit well above AvaHost's unlicensed €5.00. Uptime figures quoted by any of these providers, whether 99.9%, 99.999% or 100%, are self-reported and not independently verified here.

## Which plan, and what to confirm before you pay

Match the plan to the job rather than to the biggest number you can justify:

- **One or two small sites, and you can handle a terminal.** VPS One at €5.00/month. Watch memory; 2 GB runs a panel but leaves little room for mail and MySQL under load.
- **A handful of cPanel accounts for your own projects.** VPS Basic at €10.00/month is the sensible floor, with VPS Lucky at €15.00 if you want headroom for mailboxes and databases.
- **Selling hosting to clients through WHM.** VPS Power at €20.00 (4 vCPU, 8 GB, 90 GB) upward, with the CloudLinux template, since per-account isolation matters once other people's sites are on the box.
- **An agency juggling dozens of accounts.** VPS Extra or Ultra. Check whether one licence tier covers your account count before you size the server.

Two checks before you complete the order. First, the licence: it is billed separately here, and the amount is only visible in the cart, so confirm what the panel adds per month and whether it changes at higher account tiers. Second, the billing cycle and renewal: monthly is the listed basis for six plans, other periods are selectable at checkout, and VPS Nano is annual. The 30-day money-back period is your fallback if the licence total or the panel performance does not match what you expected.

👉 [Compare the Ava Hosting VPS plans and start your order](https://my.ava.hosting/aff.php?aff=15562)
