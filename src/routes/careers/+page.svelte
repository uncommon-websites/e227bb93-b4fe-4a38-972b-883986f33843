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
			title: "Mission-Driven Impact",
			description: "Work on technology that directly improves patient care and healthcare operations across 400+ hospitals and growing.",
			icon: IconBriefcase
		},
		{
			title: "Cutting-Edge Technology",
			description: "Build Multi-Dimensional Digital Twins and sovereignty-first AI architecture that's reshaping regulated industries.",
			icon: IconUsers
		},
		{
			title: "Global Scale Opportunity",
			description: "Join a team targeting the $11T regulated industries market with proven healthcare track record and government network access.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior AI/ML Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Healthcare Systems Integration Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Digital Twin Architecture Engineer",
			department: "Engineering",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},

		// Healthcare
		{
			title: "Healthcare Data Scientist",
			department: "Healthcare",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Clinical Workflow Specialist",
			department: "Healthcare",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},

		// Business Development
		{
			title: "Enterprise Sales Manager - Healthcare",
			department: "Sales",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Government Relations Specialist",
			department: "Sales",
			location: "Madrid",
			type: "Full-time",
			url: "#"
		},

		// Operations
		{
			title: "Healthcare Compliance Manager",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Data Sovereignty Specialist",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Enterprise Implementation Manager",
			department: "Operations",
			location: "Remote/Madrid",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
		{
			name: "Dr. Elena Rodriguez",
			position: "Healthcare Systems Engineer",
			company: "Engineering Team",
			quote:
				"Working on Multi-Dimensional Digital Twins that directly impact patient care across hundreds of hospitals is incredibly fulfilling. The technical challenges are complex, but knowing our work saves lives makes every day meaningful.",
			image: "/generated/image-a-professional-healthcare-engineer-woman.webp"
		},
		{
			name: "Carlos Martinez",
			position: "AI Architecture Lead",
			company: "Technology Team",
			quote:
				"Building sovereignty-first AI for regulated industries requires a unique approach. Here, I get to work on cutting-edge technology while ensuring complete data sovereignty—it's the perfect blend of innovation and responsibility.",
			image: "/generated/image-a-confident-male-architect-dressed-in-bu.webp"
		},
		{
			name: "Sofia Andersson",
			position: "Enterprise Sales Manager",
			company: "Business Development",
			quote:
				"Having 400+ hospitals already trusting our systems gives me incredible confidence when speaking with new prospects. We're not selling a concept—we're scaling proven technology that transforms healthcare operations.",
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
			title: "Patient-First Mission",
			description: "Every line of code, every system design, every business decision is guided by improving patient care and healthcare outcomes."
		},
		{
			icon: IconUsers,
			title: "Sovereignty & Trust",
			description: "We build systems that healthcare organizations can trust completely—your data stays yours, always."
		},
		{
			icon: IconGlobe,
			title: "Regulated Industries Expertise",
			description: "We understand the unique challenges of healthcare, government, and regulated industries, building solutions that meet the highest compliance standards."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Build the future of autonomous healthcare operations"
	subtitle="Transform regulated industries with sovereign AI systems."
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
