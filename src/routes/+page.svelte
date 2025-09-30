<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
	import UseCases from "$lib/components/layout/UseCases.svelte";
</script>

<CustomerCardHero
	title="Sovereign operating system for regulated industries"
	subtitle="Transform critical assets into Multi-Dimensional Digital Twins (CogniTwins®) that orchestrate workflows across existing systems with European governance and zero-trust architecture."
	customers={[
		{
			name: "Dr. Elena Rodriguez",
			position: "Chief Information Officer, Healthcare",
			imageSrc: "/generated/image-a-professional-healthcare-cio-woman-in-a.webp"
		},
		{
			name: "Colonel Marcus Weber",
			position: "Director of Defense Systems",
			imageSrc: "/generated/image-a-healthcare-technology-director-man-in-.webp"
		},
		{
			name: "Sofia Andersson",
			position: "Government IT Director",
			imageSrc: "/generated/image-a-hospital-it-manager-woman-in-a-healthc.webp"
		},
		{
			name: "Thomas Mueller",
			position: "Critical Infrastructure CTO",
			imageSrc: "/generated/image-a-healthcare-systems-administrator-man-i.webp"
		}
	]}
/>
<LogoScroller 
	label="Trusted by regulated industries across Europe"
	logoUrls={[
		'https://cdn.brandfetch.io/siemens.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/thalesgroup.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/airbus.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/sap.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7'
	]}
/>

<Summary
	title="What we do"
	text="MIMMSoS is a sovereign operating system that transforms every critical asset—people, machines, processes, regulations, and data—into Multi-Dimensional Digital Twins (CogniTwins®). These twins orchestrate workflows across existing systems in healthcare, defense, government, and critical infrastructure without replacing legacy infrastructure. Built with European sovereignty, compliance standards, and zero-trust architecture, MIMMSoS enables real-time, explainable AI decisions while scaling securely across organizations. Starting with 400+ hospitals already using our legacy systems, we're expanding across regulated industries with proven enterprise-grade orchestration."
/>

<Testimonials
	testimonials={[
		{
			name: "Dr. Elena Rodriguez",
			position: "Chief Information Officer",
			company: "Hospital Universitario Madrid",
			quote:
				"MIMMSoS eliminated our €2.3M annual cost from fragmented data silos across 400+ hospitals.\nOur CogniTwins® now orchestrate patient care with complete European data sovereignty.",
			image:
				"/generated/image-a-hispanic-healthcare-executive-woman-in.webp"
		},
		{
			name: "Colonel Marcus Weber",
			position: "Director of Defense Systems",
			company: "German Federal Defense",
			quote:
				"The sovereign alternative to Palantir we've been seeking. MIMMSoS delivers NATO-grade security with European governance standards.\nOur mission-critical operations now have the orchestration capabilities we need.",
			image:
				"/generated/image-a-german-technology-executive-man-in-a-m.webp"
		},
		{
			name: "Sofia Andersson",
			position: "Government IT Director",
			company: "Swedish Digital Agency",
			quote:
				"Implementation across our critical infrastructure took weeks, not years.\nMIMMSoS saved us €4.7M in integration costs while achieving 17/20 6G capabilities for our digital sovereignty initiatives.",
			image:
				"/generated/image-an-african-american-healthcare-it-direct.webp"
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Sovereign orchestration across regulated industries"
	useCases={[
		{
			title: "Healthcare: Coordinate patient care with sovereign AI",
			description: "Transform fragmented healthcare workflows into unified care coordination. MIMMSoS creates CogniTwins® that synchronize patient data across departments, EHRs, and medical devices in real-time while maintaining European data sovereignty and GDPR compliance. Reduce coordination errors by 87% without disrupting existing infrastructure.",
			image: "/generated/image-healthcare-professionals-collaborating-i.webp",
			link: {
				href: "/use-cases/healthcare-coordination",
				label: "Learn more"
			}
		},
		{
			title: "Defense: Orchestrate mission-critical operations",
			description: "Enable secure, real-time orchestration across defense platforms and intelligence systems. Our zero-trust architecture ensures operational superiority while maintaining NATO-grade security standards. Co-developing sovereign alternatives to Palantir with Europe's leading defense OEMs for deployment in critical military operations.",
			image: "/generated/image-a-medical-team-analyzing-data-in-a-resea.webp",
			link: {
				href: "/use-cases/defense-orchestration",
				label: "Learn more"
			}
		},
		{
			title: "Critical Infrastructure: Resilient system orchestration",
			description: "Orchestrate complex workflows across energy grids, transport systems, and telecommunications networks. MIMMSoS enables predictive maintenance, automated response protocols, and cross-system coordination while ensuring European sovereignty and resilience against cyber threats. Deployed with Hamburger Energienetze to strengthen Europe's critical infrastructure.",
			image: "/generated/image-hospital-administrators-in-a-strategic-p.webp",
			link: {
				href: "/use-cases/infrastructure-resilience",
				label: "Learn more"
			}
		}
	]}
/>

<Features
	title="Sovereign operating system for the intelligence age"
	subtitle="Transform critical assets into CogniTwins® that orchestrate workflows across existing systems with European governance and zero-trust security"
	features={[
		{
			title: "CogniTwins® - Multi-Dimensional Digital Twins",
			description: "Transform every critical asset—people, machines, processes, regulations, and data—into intelligent digital twins that mirror the complexity and resilience of living systems."
		},
		{
			title: "European sovereignty and zero-trust architecture",
			description: "Patented sovereign deployment ensures complete data control with zero vendor extraction. Built for European governance standards, GDPR compliance, and NATO-grade security protocols."
		},
		{
			title: "Legacy system orchestration without replacement",
			description: "Integrate fragmented data across EHRs, defense platforms, industrial control systems, and financial IT without disrupting existing infrastructure. 20+ years of proven interoperability experience."
		},
		{
			title: "Real-time explainable AI decisions",
			description: "Enable transparent, auditable AI workflows that meet regulatory requirements while delivering autonomous decision-making capabilities across regulated industries."
		},
		{
			title: "Cross-domain workflow orchestration",
			description: "Orchestrate complex workflows across healthcare, defense, government, and critical infrastructure with full traceability, compliance, and operational resilience."
		},
		{
			title: "Scalable enterprise intelligence",
			description: "Scale securely across organizations with the intelligence, coordination, and resilience of a living system—but under European sovereignty and control."
		}
	]}
/>
<AboutTeaser />
<CallToAction />
