# Ex Machina Parlor Cyber Ranges

A responsive, static GitHub Pages site introducing EMP cyber ranges, the tools we use, and the systems and protocols we test. Dedicated conference attendee guides cover Robotics & Cyber-Physical, EMP Active Directory, EMP Range Days, and Hack My Bot. Each guide directs attendees to the EMP range crew for access, scope, exercises, and assistance.

The robotics guide summarizes the supplied `robotics-cyber-range-main (1).zip` example and has five linked lab-zone sections: factory/OT, smart IoT, delivery-drone telemetry, Damn Vulnerable Drone, and virtual Wi-Fi. Optional/cloud-profile tooling and simulation boundaries are identified explicitly. The archive is reference material only; none of its deployment commands are executed or published as event access instructions. No public repository URL was supplied for this archive, so the guide does not invent one.

## Publish on GitHub Pages

1. Push these files to the `main` branch of this repository.
2. In GitHub, open **Settings → Pages → Build and deployment**, and select **GitHub Actions** as the source.
3. Run the **Deploy GitHub Pages** workflow, or push to `main` to trigger it.

Expected project URL: https://exmachinaparlor.github.io/Ex-Machina-Parlor-Cyber-Range-/

## Preview and edit

Run `python scripts/build.py`, then `python -m http.server 8000` from this directory. Open http://localhost:8000.

Edit the `RANGES` catalog in `scripts/build.py` and homepage/attendee content in `scripts/attendee_content.py`, then regenerate the HTML. Update `assets/style.css` for design changes. Commit generated HTML alongside its source so the site can also be served without a build. All internal paths support GitHub Pages project subdirectories.

The site uses no JavaScript or package dependencies. Google Fonts are optional; local font fallbacks are provided. The publishing workflow uploads only the homepage, range pages, and public assets.

## EMP 2026 branding

The supplied EMP Range 2026 logo sets the site palette: deep teal `#00151b`, green `#42bc6e`, and bright green `#50ec66`. Optimized assets in `assets/` include a 960px WebP homepage emblem, a 160px WebP header mark, and a PNG favicon. The original artwork is preserved in the supplied source file; web copies are resized and compressed without changing the design. Shared branding is applied to every generated page.
