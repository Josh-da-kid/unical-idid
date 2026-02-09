<script>
	import Slider from '$lib/components/Slider.svelte';
	import { Button } from 'carbon-components-svelte';
</script>

<section class="my-12 p-3">
	<h1 class="text-3xl lg:text-5xl font-bold text-center text-blue-600">
		University Administration Offices
	</h1>
	<p class="text-gray-500 text-xl lg:text-3xl font-semibold text-center mt-4">
		Access and manage the core administrative functions of the University of calabar <br /> through the
		dedicated offices below.
	</p>
</section>

<!-- university administration offices -->
<section class="max-w-7xl mx-auto px-6 lg:px-8">
	<!-- Office of the dvc -->
	<div class="flex flex-col text-start mx-auto justify-center space-x-4 mb-8 gap-3">
		<div class="flex items-center space-x-4 mb-4">
			<!-- svg -->
			<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 448 512"
				><path
					fill="currentColor"
					d="M304 128a80 80 0 1 0-160 0a80 80 0 1 0 160 0m-208 0a128 128 0 1 1 256 0a128 128 0 1 1-256 0M49.3 464h349.5c-8.9-63.3-63.3-112-129-112h-91.4c-65.7 0-120.1 48.7-129 112zM0 482.3C0 383.8 79.8 304 178.3 304h91.4c98.5 0 178.3 79.8 178.3 178.3c0 16.4-13.3 29.7-29.7 29.7H29.7C13.3 512 0 498.7 0 482.3"
				/></svg
			>
			<div class="text-start">
				<h2 class="font-semibold text-xl lg:text-3xl">Office Of The DVC</h2>
				<p class="text-gray-600 lg:text-lg">Manages academic programs and curriculum development</p>
			</div>
		</div>
		<p class="text-lg sm:text-xl">
			The Office of the Deputy Vice-Chancellor oversees academic planning, research, and development
			activities across the university.
		</p>
		<div class="text-xl flex flex-col space-y-2 my-2">
			<li>Academic Policy Development</li>
			<li>Research Coordination</li>
			<li>Strategic Planning</li>
			<li>Quality Assurance</li>
			<li>Staff Development Programs</li>
		</div>
		<Button class="w-fit">Contact Office</Button>
	</div>

	<!-- the senate -->
	<div class="flex flex-col text-start mx-auto justify-center space-x-4 mb-8 gap-3">
		<div class="flex items-center space-x-4 mb-4">
			<!-- svg -->
			<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 24 24"
				><g
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					><path
						d="M2.6 10.4a2.12 2.12 0 1 0 3.02 2.98L12 7l6.4 6.4a2.12 2.12 0 1 0 2.979-3.021L13.7 2.7a2.4 2.4 0 0 0-3.404.004Z"
					/><path d="M20 14v6a2 2 0 0 1-2 2H6a2 2 0 0 1-2-2v-6" /><path
						d="M14 22v-6a2 2 0 0 0-4 0v6"
					/></g
				></svg
			>
			<div class="text-start">
				<h2 class="font-semibold text-xl lg:text-3xl">The Senate</h2>
				<p class="text-gray-600 lg:text-lg">Ensuring quality and standards of education</p>
			</div>
		</div>
		<p class="text-lg sm:text-xl">
			The Senate is the highest academic body responsible for regulating academic programs and
			standards throughout the university.
		</p>
		<div class="text-xl flex flex-col space-y-2 my-2">
			<li>Academic Program Approval</li>
			<li>Curriculum Development</li>
			<li>Examination Regulations</li>
			<li>Degree Conferment</li>
			<li>Academic Calender Management</li>
		</div>
		<Button class="w-fit">Contact Office</Button>
	</div>

	<!-- Uni Registry -->
	<div class="flex flex-col text-start mx-auto justify-center space-x-4 mb-8 gap-3">
		<div class="flex items-center space-x-4 mb-4">
			<!-- svg -->
			<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 36 36"
				><path
					fill="currentColor"
					d="M28 2H8a2 2 0 0 0-2 2v28a2 2 0 0 0 2 2h20a2 2 0 0 0 2-2V4a2 2 0 0 0-2-2M13 26h-2v-2h2Zm0-4h-2v-2h2Zm0-4h-2v-2h2Zm0-4h-2v-2h2Zm0-4h-2V8h2Zm12 16H15v-2h10Zm0-4H15v-2h10Zm0-4H15v-2h10Zm0-4H15v-2h10Zm0-4H15V8h10Z"
					class="clr-i-solid clr-i-solid-path-1"
				/><path fill="none" d="M0 0h36v36H0z" /></svg
			>
			<div class="text-start">
				<h2 class="font-semibold text-xl lg:text-3xl">University Registry</h2>
				<p class="text-gray-600 lg:text-lg">Maintains academic records and student information</p>
			</div>
		</div>
		<p class="text-lg sm:text-xl">
			The Registry manages student records, admissions, examinations, and serves as the central
			administrative hub for academic operations.
		</p>
		<div class="text-xl flex flex-col space-y-2 my-2">
			<li>Student Records Management</li>
			<li>Admissions Processing</li>
			<li>Transcripts & Certificates</li>
			<li>Course Registration</li>
			<li>Graduation Processing</li>
		</div>
		<Button class="w-fit">Contact Office</Button>
	</div>

	<!-- Uni Bursary -->
	<div class="flex flex-col text-start mx-auto justify-center space-x-4 mb-8 gap-3">
		<div class="flex items-center space-x-4 mb-4">
			<!-- svg -->
			<svg xmlns="http://www.w3.org/2000/svg" width="48" height="48" viewBox="0 0 24 24"
				><path
					fill="none"
					stroke="currentColor"
					stroke-linecap="round"
					stroke-linejoin="round"
					stroke-width="2"
					d="M6.5 15H6m12-6h-.5M3 6.5c7 2 11-2 18 0v11c-7-2-11 2-18 0zm8.47 3.106l.098-.02a2.451 2.451 0 0 1 .961 4.808l-.097.02a2.452 2.452 0 0 1-.961-4.808Z"
				/></svg
			>
			<div class="text-start">
				<h2 class="font-semibold text-xl lg:text-3xl">University Bursary</h2>
				<p class="text-gray-600 lg:text-lg">Manages student financial aid and scholarships</p>
			</div>
		</div>
		<p class="text-lg sm:text-xl">
			The Bursary manages all financial transactions, fee collection, budgeting, and financial
			reporting for the university.
		</p>
		<div class="text-xl flex flex-col space-y-2 my-2">
			<li>Tuition Fee Management</li>
			<li>Financial Aid & Scholarships</li>
			<li>Budgeting Planning</li>
			<li>Payment Processing</li>
			<li>Financial Reporting</li>
		</div>
		<Button class="w-fit">Contact Office</Button>
	</div>
</section>

<!-- slider  -->
<Slider/>

