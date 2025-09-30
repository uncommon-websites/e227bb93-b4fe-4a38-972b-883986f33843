<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "European Sovereignty",
			description: "Built for European governance standards with zero vendor data extraction. Complete control over your critical assets while meeting GDPR, AI Act, and NATO-grade security requirements."
		},
		{
			title: "CogniTwins® Orchestration",
			description: "Transform every critical asset—people, machines, processes, regulations, and data—into Multi-Dimensional Digital Twins that orchestrate workflows across existing systems without replacement."
		},
		{
			title: "Zero-Trust Intelligence",
			description: "Scalable enterprise intelligence with the coordination and resilience of living systems, built on zero-trust architecture that ensures security and compliance across regulated industries."
		}
	];
</script>

<SecondaryHero
	title="Building Europe's sovereign operating system for regulated industries"
	subtitle="CogniTwins® that orchestrate critical workflows with European governance and zero-trust architecture"
	imageSrc="/generated/image-a-group-of-software-engineers-collaborat.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"MIMMSoS emerged from a profound understanding: regulated industries across Europe are constrained by fragmented systems that prevent true operational intelligence. With 400+ hospitals already trusting our legacy systems and proven track record in healthcare interoperability, we recognized the opportunity to build Europe's sovereign operating system for critical industries.",
		"Our journey began almost two decades ago when Dr. Hugo Herrero was introduced to pioneering research in model-guided medicine. Over 10 years, he transformed this vision into MIMMSoS—the world's first system of systems that mirrors the complexity and resilience of the human body. Today, our CogniTwins® don't just integrate data—they orchestrate entire enterprise operations with European sovereignty at the core.",
		"Led by the combined expertise of Dr. Javier Herrero's 43+ years in HealthTech and government networks, Hugo Herrero's technical innovation, and Timo Spring's proven business scaling experience, we're uniquely positioned to deliver sovereign AI orchestration at global scale. Every architectural decision prioritizes European governance, zero-trust security, and complete data sovereignty.",
		"We're not building another AI platform. We're creating the sovereign operating system that enables enterprises to run with the intelligence, coordination, and resilience of living systems—but under European sovereignty, compliance, and control. Our patented architecture ensures your critical assets remain yours while delivering unprecedented operational orchestration across healthcare, defense, government, and critical infrastructure."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Leadership team."
	subtitle="Decades of regulated industries and sovereign AI expertise."
	stakeholders={[
		{
			name: "Dr. Javier Herrero",
			position: "Co-founder | President of Alma IT Systems S.L.",
			bio: "43+ years experience in HealthTech and government networks. Uniquely positioned to solve enterprise AI interoperability for regulated industries at global scale, with deep understanding of European compliance and sovereignty requirements.",
			image: "https://placehold.co/400x500/111827/374151"
		},
		{
			name: "Hugo Herrero",
			position: "Founder | Director of Tech, Innovation & Strategy",
			bio: "Architect of MIMMSoS and CogniTwins® technology. Transformed 20 years of model-guided medicine research into the world's first sovereign operating system for regulated industries. Leading technical vision for Multi-Dimensional Digital Twins and zero-trust architecture.",
			image: "https://placehold.co/400x500/111827/374151"
		},
		{
			name: "Timo Spring",
			position: "Co-founder & Director of Sales, BD & IR",
			bio: "Former CEO & Founder of Prevess and ex-COO of Family Office managing €5-50M AUM. Built Europe's BLUEPRINT protocol and launched personalized nutrition APIs. Proven track record in scaling operations across regulated industries and navigating complex enterprise sales cycles.",
			image: "https://placehold.co/400x500/111827/374151"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Proven market traction."
	subtitle="Trusted across regulated industries with 400+ hospitals and strategic partnerships"
	stakeholders={[
		{
			name: "Healthcare Systems",
			image: "/generated/image-a-medical-team-discussing-patient-care-i.webp"
		},
		{
			name: "Defense & Government",
			image: "/generated/image-medical-professionals-collaborating-in-a.webp"
		},
		{
			name: "Critical Infrastructure",
			image: "/generated/image-healthcare-workers-in-a-professional-med.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to achieve sovereign operational intelligence?"
	subtitle="Join the regulated industries already leveraging CogniTwins®"
	description="Discover how MIMMSoS transforms critical assets into Multi-Dimensional Digital Twins that orchestrate workflows across existing systems with European governance, zero-trust architecture, and complete data sovereignty."
/>
