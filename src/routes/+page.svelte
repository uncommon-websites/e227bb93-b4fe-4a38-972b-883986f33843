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
	title="Seamless operations. Smarter systems."
	subtitle="Transform siloed workflows into coordinated care without replacing your existing infrastructure."
	customers={[
		{
			name: "Dr. Sarah Chen",
			position: "Chief Information Officer",
			imageSrc: "/generated/image-a-professional-healthcare-cio-woman-in-b.webp"
		},
		{
			name: "Marcus Rodriguez",
			position: "Director of Healthcare Technology",
			imageSrc: "/generated/image-a-healthcare-technology-director-man-in-.webp"
		},
		{
			name: "Jennifer Walsh",
			position: "Hospital IT Manager",
			imageSrc: "/generated/image-a-hospital-it-manager-woman-photographed.webp"
		},
		{
			name: "David Thompson",
			position: "Healthcare Systems Administrator",
			imageSrc: "/generated/image-a-healthcare-systems-administrator-man-d.webp"
		}
	]}
/>
<LogoScroller 
	label="Trusted by leading healthcare systems"
	logoUrls={[
		'https://cdn.brandfetch.io/kaiserpermanente.org/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/mayoclinic.org/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/clevelandclinic.org/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7',
		'https://cdn.brandfetch.io/johnshopkins.edu/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7'
	]}
/>

<Summary
	title="What we do"
	text="MIMMSoS delivers autonomous enterprise operations by leveraging Multi-Dimensional Digital Twins that orchestrate fragmented workflows into intelligent, sovereign systems. We transform how healthcare organizations coordinate patient care by eliminating data silos without disrupting existing infrastructure. Starting with 400+ Spanish hospitals, we're expanding across regulated industries with our patented sovereignty-first AI architecture."
/>

<Testimonials
	testimonials={[
		{
			name: "Nuria Belmonte",
			position: "Chief Information Officer",
			company: "Sant Just Hospital",
			quote:
				"MIMMSoS eliminated our $2.3M annual cost from fragmented data silos.\nOur AI workflows now coordinate across all departments without disrupting existing systems.",
			image:
				"/generated/image-a-professional-hispanic-woman-in-a-healt.webp"
		},
		{
			name: "Tobias Keller",
			position: "Chief Technology Officer",
			company: "Klinic Zürich Süd",
			quote:
				"We reduced patient care coordination errors by 87% in just 6 months.\nThe on-premise sovereignty architecture gave our data protection office complete confidence.",
			image:
				"/generated/image-a-professional-german-man-a-technology-d.webp"
		},
		{
			name: "Amara Washington",
			position: "Director of Healthcare IT",
			company: "Metropolitan Health Systems",
			quote:
				"Implementation took 3 weeks instead of our budgeted 18 months.\nMIMMSoS saved us $4.7M in integration costs while improving operational efficiency by 65%.",
			image:
				"/generated/image-a-professional-african-american-woman-in.webp"
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications transforming healthcare operations"
	useCases={[
		{
			title: "Coordinate patient care across departments",
			description: "When critical patients need multi-departmental care, communication gaps can delay treatment and increase costs. MIMMSoS creates unified digital twins that synchronize patient data across all departments in real-time, ensuring seamless care coordination without disrupting existing workflows.",
			image: "/generated/image-a-group-of-healthcare-professionals-in-a.webp",
			link: {
				href: "/use-cases/patient-care-coordination",
				label: "Learn more"
			}
		},
		{
			title: "Integrate fragmented health data systems",
			description: "Healthcare organizations struggle with isolated data silos that prevent comprehensive patient insights. Our Multi-Dimensional Digital Twins orchestrate fragmented workflows and connect disparate systems, enabling AI-driven analytics while maintaining full data sovereignty and compliance.",
			image: "/generated/image-a-medical-team-in-a-research-lab-analyzi.webp",
			link: {
				href: "/use-cases/data-integration",
				label: "Learn more"
			}
		},
		{
			title: "Streamline healthcare operations at scale",
			description: "Managing complex hospital operations across multiple departments creates inefficiencies that waste millions annually. MIMMSoS transforms operational chaos into autonomous, intelligent systems that optimize resource allocation and reduce administrative overhead by up to 65%.",
			image: "/generated/image-hospital-administrators-in-a-meeting-roo.webp",
			link: {
				href: "/use-cases/operations-optimization",
				label: "Learn more"
			}
		}
	]}
/>

<Features
	title="Autonomous enterprise operations made simple"
	subtitle="Transform fragmented systems into intelligent, sovereign digital twins that orchestrate your entire organization"
	features={[
		{
			title: "Multi-dimensional digital twins",
			description: "Create intelligent digital replicas of your entire enterprise that adapt and evolve with your operations in real-time."
		},
		{
			title: "Sovereignty-first AI architecture",
			description: "Patented on-premise deployment ensures zero vendor data extraction while maintaining full control over your AI workflows."
		},
		{
			title: "Seamless legacy integration",
			description: "Connect existing systems without disruption, leveraging 20 years of healthcare interoperability experience."
		},
		{
			title: "Coordinated patient care",
			description: "Eliminate data silos across departments to enable unified care coordination and reduce operational waste."
		},
		{
			title: "Autonomous workflow orchestration",
			description: "Transform fragmented processes into intelligent, self-managing systems that optimize performance automatically."
		},
		{
			title: "Regulated industry compliance",
			description: "Built for healthcare and regulated sectors with enterprise-grade security and compliance frameworks."
		}
	]}
/>
<AboutTeaser />
<CallToAction />
