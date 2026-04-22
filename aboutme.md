---
layout: page
title: About me
subtitle: Petri Paavola
---

<style>
	@import url("https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Source+Serif+4:wght@400;600&display=swap");

	.about-ninja {
		--ink: #102038;
		--muted: #4a5f7e;
		--line: #d9e2ef;
		--panel: #ffffff;
		--hero-a: #f5fbff;
		--hero-b: #e8f4ff;
		--accent: #0d6b9a;
		--accent-2: #ea7f2d;
		color: var(--ink);
		font-family: "Source Serif 4", Georgia, serif;
	}

	.about-hero {
		margin: 8px 0 20px;
		padding: 26px;
		border: 1px solid var(--line);
		border-radius: 14px;
		background: linear-gradient(140deg, var(--hero-a) 0%, var(--hero-b) 100%);
		box-shadow: 0 14px 28px rgba(16, 34, 56, 0.08);
	}

	.about-hero h1 {
		margin: 0 0 10px;
		font-family: "Space Grotesk", "Segoe UI", sans-serif;
		font-size: clamp(1.6rem, 2.5vw, 2.2rem);
	}

	.about-hero p {
		margin: 0;
		line-height: 1.6;
		color: #2e4463;
	}

	.about-meta {
		display: flex;
		flex-wrap: wrap;
		gap: 8px;
		margin-top: 14px;
	}

	.about-pill {
		display: inline-block;
		border: 1px solid #bdd5e8;
		border-radius: 999px;
		background: #fff;
		color: #0a567b;
		padding: 6px 10px;
		font-family: "Space Grotesk", "Segoe UI", sans-serif;
		font-size: 0.86rem;
		font-weight: 700;
		text-decoration: none;
	}

	.about-title {
		margin: 26px 0 12px;
		padding-bottom: 8px;
		border-bottom: 2px solid #e4ecf5;
		font-family: "Space Grotesk", "Segoe UI", sans-serif;
		font-size: 1.2rem;
	}

	.about-panel {
		border: 1px solid #dde6f2;
		border-radius: 14px;
		background: var(--panel);
		padding: 18px;
		box-shadow: 0 10px 22px rgba(16, 34, 56, 0.05);
	}

	.about-panel p {
		margin: 0 0 12px;
		color: var(--muted);
		line-height: 1.66;
	}

	.about-panel p:last-child {
		margin-bottom: 0;
	}

	.focus-grid {
		display: grid;
		gap: 12px;
		grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
		margin: 8px 0 14px;
	}

	.focus-card {
		padding: 14px;
		border: 1px solid #dde6f1;
		border-radius: 12px;
		background: #f9fcff;
	}

	.focus-card h3 {
		margin: 0 0 8px;
		font-family: "Space Grotesk", "Segoe UI", sans-serif;
		font-size: 0.98rem;
		color: #163457;
	}

	.focus-card p {
		margin: 0;
		font-size: 0.97rem;
		line-height: 1.6;
		color: #4f607a;
	}

	@media (max-width: 767px) {
		.about-hero,
		.about-panel {
			border-radius: 12px;
		}

		.about-hero {
			padding: 20px;
		}
	}
</style>

<div class="about-ninja">
	<section class="about-hero">
		<h1>Petri Paavola</h1>
		<p>
			CEO / Founder at <a href="https://www.yodamiitti.fi/en-us">Yodamiitti Oy</a>, Senior Modern Management Principal,
			and Microsoft MVP - Windows and Intune. I work mainly with Intune, Windows, and PowerShell.
			One specialty is creating Community Tools for Intune and Windows admins.
		</p>
		<div class="about-meta">
			<a class="about-pill" href="mailto:Petri.Paavola@yodamiitti.fi">Petri.Paavola@yodamiitti.fi</a>
			<a class="about-pill" href="https://mvp.microsoft.com/en-US/mvp/profile/cdb970c0-3c9a-e411-93f2-9cb65495d3c4">Microsoft MVP - Windows and Intune</a>
			<a class="about-pill" href="https://github.com/petripaavola">GitHub</a>
			<a class="about-pill" href="https://www.linkedin.com/in/petri-paavola">LinkedIn</a>
		</div>
	</section>

	<h2 class="about-title">Background</h2>
	<section class="about-panel">
		<p>
			Petri Paavola has been a Microsoft MVP for 15 years and has more than 25 years of experience in the IT industry.
		</p>
		<p>
			Daily focus areas are built around Intune, Windows, and PowerShell, with closely related technologies used in modern management and automation work.
		</p>
		<div class="focus-grid">
			<div class="focus-card">
				<h3>Intune</h3>
				<p>
					Device management, application deployment, configuration profiles, compliance policies, remediation, reporting,
					and ConfigMgr / co-management scenarios.
				</p>
			</div>
			<div class="focus-card">
				<h3>Windows</h3>
				<p>
					Windows Autopilot, endpoint configuration, troubleshooting, deployment workflows, and broader modern workplace operations.
				</p>
			</div>
			<div class="focus-card">
				<h3>PowerShell</h3>
				<p>
					Automation, tooling, Microsoft Graph API integrations, Entra ID related administration, data handling,
					and script-based troubleshooting.
				</p>
			</div>
		</div>
		<p>
			He also has a strong on-premises background in Active Directory, Group Policy, ConfigMgr, MDT, and task sequence-based deployment operations.
		</p>
		<p>
			The core mission: help admins do their work faster and better with practical tools that solve real production problems.
		</p>
	</section>
</div>
