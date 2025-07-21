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
			title: "Sovereignty",
			description: "Your data stays yours. Our on-premise deployment ensures zero vendor data extraction while delivering autonomous operations."
		},
		{
			title: "Orchestration",
			description: "We don't just integrate—we orchestrate. Our Multi-Dimensional Digital Twins transform fragmented workflows into intelligent, coordinated systems."
		},
		{
			title: "Autonomy",
			description: "True enterprise autonomy through AI systems that operate independently while maintaining full regulatory compliance and data sovereignty."
		}
	];
</script>

<SecondaryHero
	title="Transforming healthcare through autonomous enterprise operations"
	subtitle="Sovereign AI systems that orchestrate fragmented workflows"
	imageSrc="/generated/image-a-group-of-software-engineers-collaborat.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"MIMMSoS was born from a critical realization: healthcare systems worldwide are drowning in fragmented data and disconnected workflows. With 400+ Spanish hospitals already trusting our legacy systems, we saw an opportunity to revolutionize how regulated industries operate.",
		"Our Multi-Dimensional Digital Twins don't just integrate data—they orchestrate entire enterprise operations autonomously. We've spent 20 years perfecting healthcare technology, understanding that in regulated industries, sovereignty isn't optional—it's essential.",
		"Led by Dr. Javier Herrero's 43+ years of HealthTech expertise and government network experience, we're uniquely positioned to solve enterprise AI interoperability at global scale. Every decision we make prioritizes data sovereignty and operational autonomy.",
		"We're not building another AI tool. We're creating the foundation for autonomous enterprise operations that transform fragmented chaos into intelligent, coordinated systems. Our patented sovereignty-first architecture ensures your data remains yours while delivering unprecedented operational intelligence."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Leadership team."
	subtitle="Decades of healthcare and enterprise expertise."
	stakeholders={[
		{
			name: "Dr. Javier Herrero",
			position: "Co-founder | President of Alma IT Systems S.L.",
			bio: "43+ years experience in HealthTech and government networks, uniquely positioned to solve enterprise AI interoperability for regulated industries at global scale.",
			image: "https://placehold.co/400x500/f3f4f6/f3f4f6"
		},
		{
			name: "Hugo Herrero",
			position: "Founder | Director of Tech, Innovation & Strategy",
			bio: "Leading the technical vision for Multi-Dimensional Digital Twins and autonomous enterprise operations with deep expertise in healthcare technology architecture.",
			image: "https://placehold.co/400x500/f3f4f6/f3f4f6"
		},
		{
			name: "Timo Spring",
			position: "Co-founder & Director of Sales, BD & IR",
			bio: "Former CEO & Founder of Prevess and ex-COO of Family Office managing €5-50M AUM. Proven track record in scaling operations and navigating complex enterprise sales cycles.",
			image: "https://placehold.co/400x500/f3f4f6/f3f4f6"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Proven market traction."
	subtitle="400+ Spanish hospitals already trust our systems"
	stakeholders={[
		{
			name: "Healthcare Systems",
			image: "/generated/image-a-medical-team-discussing-patient-care-i.webp"
		},
		{
			name: "Government Networks",
			image: "/generated/image-medical-professionals-collaborating-in-a.webp"
		},
		{
			name: "Regulated Industries",
			image: "/generated/image-healthcare-workers-in-a-professional-med.webp"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to transform your enterprise operations?"
	subtitle="Join the healthcare systems already leveraging autonomous AI"
	description="Discover how Multi-Dimensional Digital Twins can orchestrate your fragmented workflows into intelligent, sovereign systems while maintaining complete data sovereignty."
/>
