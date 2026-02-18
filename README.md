# Understanding Zero Trust  

Zero Trust gets talked about a lot in security, but the core idea is actually pretty simple: **don't automatically trust anything**. Not users, not devices, not network traffic. EVERYTHING has to prove it's legitimate before it gets access.

When I started learning cybersecurity, I kept seeing Zero Trust mentioned in job descriptions, so I dug into what it really looks like in practice. Here's the version that finally clicked for me.

## "Never Trust, Always Verify" in Real Life

Zero Trust isn't a product you install. It's a mindset. Instead of assuming something is safe because it's "inside the network," Zero Trust treats every request like it's coming from the open internet.

That means:

- Users must authenticate every time they try to access something
- Devices must meet security requirements before they're allowed in
- Access is limited to exactly what someone needs and nothing extra
- Activity is monitored continuously, not just at login

It's basically the opposite of the old model where everything inside the network is safe (the castle), and only the perimeter needs protection (the moat).

## How I Practiced Zero Trust in My Own Lab

While building out my Azure and Windows environment, I started applying Zero Trust ideas without even realizing it at first. A few examples:

- **Using NSGs to restrict traffic** instead of leaving ports wide open
- **Applying least privilege** when creating users and groups
- **Requiring authentication for every service**, even inside the virtual network
- **Segmenting resources** so one compromised VM wouldn't expose everything else

It was just about being intentional with access and not assuming "internal = safe."

## Why It Matters

Zero Trust isn't just a buzzword. It's how modern organizations protect themselves when users work remotely, devices come and go, and threats can come from anywhere. Learning it early helped me understand why identity, access control, and network segmentation are such a big deal in real environments.
