<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "European Sovereignty Mission",
			description: "Build the sovereign operating system that protects Europe's critical infrastructure across healthcare, defense, government, and industrial operations with 400+ hospitals already deployed.",
			icon: IconBriefcase
		},
		{
			title: "CogniTwins® Technology",
			description: "Architect Multi-Dimensional Digital Twins and zero-trust infrastructure that transforms critical assets into intelligent, orchestrated systems for regulated industries.",
			icon: IconUsers
		},
		{
			title: "Regulated Industries Scale",
			description: "Target the €11T regulated industries market with proven track record, government network access, and strategic partnerships with Europe's leading defense OEMs and critical infrastructure operators.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior CogniTwins® AI/ML Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Sovereign Systems Integration Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Zero-Trust Architecture Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Multi-Dimensional Digital Twin Architect",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},

		// Regulated Industries
		{
			title: "Defense Systems Specialist",
			department: "Regulated Industries",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Healthcare Data Sovereignty Scientist",
			department: "Regulated Industries",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Critical Infrastructure Orchestration Engineer",
			department: "Regulated Industries",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},

		// Business Development
		{
			title: "Enterprise Sales Manager - Defense & GovTech",
			department: "Sales",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Government Relations & EU Policy Specialist",
			department: "Sales",
			location: "Madrid/Brussels",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Strategic Partnerships Manager - Critical Infrastructure",
			department: "Sales",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},

		// Operations
		{
			title: "European Compliance & Sovereignty Manager",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Zero-Trust Security Operations Specialist",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Regulated Industries Implementation Manager",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
		{
			name: "Dr. Elena Rodriguez",
			position: "CogniTwins® Systems Engineer",
			company: "Engineering Team",
			quote:
				"Building Multi-Dimensional Digital Twins that orchestrate critical workflows across healthcare, defense, and government systems is incredibly fulfilling. The technical challenges of sovereign AI are complex, but knowing our work protects Europe's critical infrastructure makes every day meaningful.",
			image: "/generated/image-a-professional-healthcare-engineer-woman.webp"
		},
		{
			name: "Carlos Martinez",
			position: "Zero-Trust Architecture Lead",
			company: "Technology Team",
			quote:
				"Architecting sovereign operating systems for regulated industries requires a unique approach. Here, I get to work on cutting-edge CogniTwins® technology while ensuring complete European data sovereignty and NATO-grade security—it's the perfect blend of innovation and responsibility.",
			image: "/generated/image-a-confident-male-architect-dressed-in-bu.webp"
		},
		{
			name: "Sofia Andersson",
			position: "Enterprise Sales Manager - Defense & GovTech",
			company: "Business Development",
			quote:
				"Having 400+ hospitals already trusting our systems and strategic partnerships with Europe's leading defense OEMs gives me incredible confidence. We're not selling a concept—we're scaling proven sovereign technology across regulated industries that need European alternatives to US platforms.",
			image: "/generated/image-a-professional-female-sales-manager-in-h.webp"
		}
	];

	const processSteps = [
		{
			step: 1,
			title: "Apply",
			description:
				"Submit your application through our careers portal with your resume and portfolio."
		},
		{
			step: 2,
			title: "Interview",
			description: "Meet with our team to discuss your experience, skills, and career aspirations."
		},
		{
			step: 3,
			title: "Welcome aboard",
			description: "Join our team and start your journey building the future with us."
		}
	];

	const values = [
		{
			icon: IconHeart,
			title: "Critical Infrastructure Mission",
			description: "Every line of code, every system design, every business decision is guided by protecting and enhancing Europe's critical infrastructure across healthcare, defense, government, and industrial operations."
		},
		{
			icon: IconUsers,
			title: "European Sovereignty & Trust",
			description: "We build sovereign systems that regulated industries can trust completely—your critical assets stay yours, under European governance and zero-trust architecture."
		},
		{
			icon: IconGlobe,
			title: "Regulated Industries Expertise",
			description: "We understand the unique challenges of healthcare, defense, government, and critical infrastructure, building CogniTwins® solutions that meet the highest sovereignty and compliance standards."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Build Europe's sovereign operating system for regulated industries"
	subtitle="Transform critical infrastructure with CogniTwins® and zero-trust architecture."
	imageSrc="/generated/image-a-healthcare-team-in-a-modern-medical-fa.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Build your career while making an impact" />

	<div class="mt-16 grid gap-4 md:grid-cols-3">
		{#each benefits as benefit}
			<Card {...benefit} />
		{/each}
	</div>
</section>

<!-- Culture Section -->
<Culture {values} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
