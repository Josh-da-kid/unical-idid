<script>
	import Navbar from '$lib/components/Navbar.svelte';
	import { events, news } from '$lib/news';
	import { TextInput, Button } from 'carbon-components-svelte';
	import { Add } from 'carbon-icons-svelte';

	const services = [
		{
			img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRBFtPogRcJSPmgzirUEOGeNfb7_CoFIus0qg&s',
			title: 'Identify & Biometric',
			description:
				'Leveraging state-of-the-art face verification, UNICAL IDID <br> ensures protected and intuitive access throughout the campus. <br>  Secure your sensitive information and enjoy an efficient, seamless <br>  interaction.',
			icon: 'identify-biometric',
			button: {
				text: 'Access',
				link: '/identify-biometric'
			}
		},
		{
			img: 'https://media.istockphoto.com/id/1220629405/photo/man-holding-light-bulbs-ideas-of-new-ideas-with-innovative-technology-and-creativity.jpg?s=612x612&w=0&k=20&c=QtFDsJUkcTEFmJ94YliS9UjtobZM-mBdR2Wue4sL6qc=',
			title: 'Baams',
			description:
				'Leveraging state-of-the-art face verification, UNICAL IDID <br> ensures protected and intuitive access throughout the campus. <br>  Secure your sensitive information and enjoy an efficient, seamless <br>  interaction.',
			icon: 'baams',
			button: {
				text: 'Access',
				link: '/baams'
			}
		},
		{
			img: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR9I9WoATXpTSOa2A6k2jPMKiRT1rDq5smFug&s',
			title: 'UNICAL Messenger',
			description:
				'Stay connected with ease using UNICAL Messenger, your go-to <br>  communication platform for real-time updates, group discussions, <br>  and direct messaging within the university community.',
			icon: 'unical-messenger',
			button: {
				text: 'Access',
				link: '/unical-messenger'
			}
		}
	];
</script>

<Navbar />

<section
	class="relative h-[calc(100vh-4rem)] bg-cover bg-center"
	style="background-image: url('/images.jpeg');"
>
	<!-- Dark overlay -->
	<div class="absolute inset-0 bg-black/20"></div>

	<!-- Content -->
	<div class="relative z-10 flex h-full items-center justify-center px-6">
		<div class="max-w-3xl text-center text-white space-y-6">
			<h1 class="text-4xl md:text-5xl font-bold leading-tight">
				Access Your Academic<br />
				Journey Through One Unified<br />
				Hub.
			</h1>

			<p class="text-base md:text-lg text-gray-200">
				UNICAL Hub connects students, staff, and alumni to everything they need – from course
				registration and results to accommodation, payments, and campus services. All in one place,
				accessible anytime, anywhere.
			</p>

			<div
				class="sm:flex flex-col sm:flex-row gap-3 justify-center mt-6 items-center space-y-3 sm:space-y-0"
			>
				<div class="w-full sm:w-96">
					<TextInput placeholder="Search Courses..." hideLabel class="bg-white" />
				</div>

				<Button kind="primary" class=" hover:bg-blue-700">Search</Button>
			</div>
		</div>
	</div>
</section>

<!-- slider -->
<section
	class="flex items-center justify-around py-6 px-8 bg-gray-900 text-white text-2xl space-x-6 overflow-x-auto"
>
	<div class="flex-shrink-0 flex items-center space-x-2">
		<span
			><svg xmlns="http://www.w3.org/2000/svg" width="38" height="38" viewBox="0 0 48 48"
				><g fill="none" stroke="currentColor" stroke-width="4"
					><path fill="currentColor" d="M32 28h6v11a3 3 0 1 1-6 0z" /><path
						stroke-linecap="round"
						d="M29 12h10a3 3 0 0 1 3 3v10a3 3 0 0 1-3 3H28"
					/><path stroke-linejoin="round" d="M14 14h-2a6 6 0 0 0 0 12h2" /><path
						fill="currentColor"
						d="M14.198 33a.2.2 0 0 1-.198-.198V6.198c0-.11.089-.198.198-.198H17.5C24.956 6 31 12.044 31 19.5S24.956 33 17.5 33z"
					/></g
				></svg
			></span
		>
		<span>Course Registration Now Open</span>
	</div>

	<div class="flex-shrink-0 flex items-center space-x-2">
		<span
			><svg xmlns="http://www.w3.org/2000/svg" width="38" height="38" viewBox="0 0 128 128"
				><path
					fill="#424242"
					d="M99.06 91.42S83.95 105.6 63.97 105.6S28.89 91.42 28.89 91.42s-2.81-13.49 4.45-36.78c3.83-12.28 58.33-13.53 62.6-2.79c7.26 18.23 3.12 39.57 3.12 39.57"
				/><path
					fill="#212121"
					d="m28.89 91.42l4.79 3.84s-.04-7.6 2.31-14.69c.88-2.65 4.02-3.76 6.38-2.27l18.29 11.47a6.39 6.39 0 0 0 6.7.05c8.74-5.3 31.54-19.17 32.58-20.02c0 0 0-1.71-.43-3.89L28.63 66z"
				/><path
					fill="#424242"
					d="m122.81 52.03l-56.8 33.83c-1.24.74-2.79.74-4.04 0L5.19 52.03c-1.58-.94-1.58-3.23 0-4.17l56.8-33.83c1.24-.74 2.79-.74 4.04 0l56.8 33.83c1.57.94 1.57 3.23-.02 4.17"
				/><path
					fill="#9e9e9e"
					d="M64.04 83.38c-.01 0-.03.01-.04.01c-.16 0-.32-.04-.46-.13L4.18 49.04s-.29.55 0 1.54c.3.99.76 1.31 1.01 1.46l56.8 33.83c.62.37 1.32.56 2.02.56h.04v-3.05z"
				/><path
					fill="#616161"
					d="M64 83.38c.01 0 .03.01.04.01c.16 0 .32-.04.46-.13l59.36-34.22s.29.55 0 1.54c-.3.99-.76 1.31-1.01 1.46l-56.8 33.83c-.62.37-1.32.56-2.02.56h-.04v-3.05z"
				/><path
					fill="#424242"
					d="m35.45 70.06l.32-2.81S60.28 53.92 62.7 52.52s4.96-2.96 6.09-4.21c2-2.2.56-3.58.56-3.58s-1.58 2.56-5.35 2.11c-2.16-.26-4.97-2.01-5.44-2.83s-27.67 19.9-27.67 19.9l-.19 3.33z"
				/><path
					fill="#e2a610"
					d="M69.35 44.74c-2.62 3.66-7.06 2.06-7.06 2.06s-13.91 6.67-14.43 5.66s11.49-7.19 11.49-7.19s-.67-2.46-.6-3.51c0 0-21.72 13.82-29.87 18.47c-4.27 2.44-5.18 4.74-5.17 7.98c0 1.42.02 6.03.04 8.78c0 .51-.22.99-.61 1.31a5.16 5.16 0 0 0-1.89 3.99c0 1.53.67 2.9 1.73 3.85c.57.51.45 1.61.5 2.32c.1 1.36 0 1.98-.56 3.24c-.55 1.23-1.06 2.49-1.41 3.79c-.27 1-.45 2.03-.63 3.05c-1.19 6.83-1.73 14.13-4.88 20.41a.993.993 0 0 0 .45 1.34a1.007 1.007 0 0 0 1.35-.44c1.64-3.27 2.49-6.85 3.19-10.4c-.04 3.21-.06 6.45-.17 9.95c-.02.68-.07 2.05.55 2.35c2.33 1.13 2.33-2.35 2.33-2.35s.03 3.13 3.2 3.13s3.4-3.13 3.4-3.13s.23 2.87 1.86 2.73c.66-.06 1.53-.46 1.22-3.89c-.31-3.42-1.08-15.68-1.41-19.56c-.46-5.37-2.22-8.56-2.58-10.46c-.13-.72-.14-1.47.43-1.94a5.165 5.165 0 0 0 .13-7.88a1.71 1.71 0 0 1-.58-1.42c.19-2.59.4-6.35.57-7.22c.74-3.91 2.67-4.61 4.65-5.77c1.98-1.17 30.66-14.19 32.33-15.3c3.09-2.07 2.43-3.95 2.43-3.95"
				/><path
					fill="#ffca28"
					d="M69.35 44.74c-2.47 3.49-7.6 1.93-7.6 1.93s-13.11 5.81-12.24 4.76c.86-1.05 9.84-6.16 9.84-6.16s-.67-2.46-.6-3.51c0 0-22.1 12.77-30.67 18.91c-2.21 1.59-4.95 4.19-2.72 6.78c1.03 1.19 3.02 1.44 4.29.5c.77-.56 1.37-1.38 2.05-2.03c.84-.82 1.86-1.34 2.86-1.93c1.98-1.17 30.66-14.19 32.33-15.3c3.12-2.07 2.46-3.95 2.46-3.95"
				/><path
					fill="#9e740b"
					d="M26.11 91.86c-1.32 0-2.21-.11-3.02-.3a.62.62 0 0 1-.48-.65l.26-3.82c.03-.39.4-.66.78-.55c.9.26 2.7.52 5.64-.1c.36-.08.72.17.76.54l.4 3.8c.03.31-.17.6-.47.67c-1.53.35-2.64.41-3.87.41"
				/><path
					fill="#616161"
					d="M99.06 91.42s1.77-9.24 1.06-19.07c-.12-1.66-1.14-3.09-1.93 2.72c-.45 3.33-1.43 13.3-3.1 19.53c2.55-1.84 3.97-3.18 3.97-3.18M65.73 36.79c.73.23 1.4.79 1.59 1.54c.25 1-.38 2-1.06 2.78c-1.33 1.53-3.16 2.87-5.19 2.8c-.67-.02-1.39-.24-1.8-.77c-.29-.37-.39-.85-.42-1.32c-.18-3.43 3.7-6.03 6.88-5.03"
				/></svg
			></span
		>
		<span>NUGA 2026 Hosting </span>
	</div>

	<div class="flex-shrink-0 flex items-center space-x-2">
		<span
			><svg xmlns="http://www.w3.org/2000/svg" width="38" height="38" viewBox="0 0 24 24"
				><g fill="none"
					><path
						fill="#fff"
						d="M22.044 3.87v13.39H17.26a.957.957 0 0 0-.957.957V23H2.914a.956.956 0 0 1-.957-.957V3.87a.957.957 0 0 1 .956-.957h18.174a.956.956 0 0 1 .957.957"
					/><path
						fill="#e3e3e3"
						d="M22.043 17.26L16.304 23v-4.783a.957.957 0 0 1 .957-.956z"
					/><path
						stroke="#191919"
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M4.826 1v4.304M9.609 1v4.304M14.391 1v4.304M19.174 1v4.304M9.609 7.696l-2.87 2.87L5.305 9.13m4.304 3.827l-2.87 2.87l-1.434-1.436m6.217-4.782h6.217m-6.217 4.782h6.217"
						stroke-width="1"
					/><path
						stroke="#191919"
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M22.044 3.87v13.39H17.26a.957.957 0 0 0-.957.957V23H2.914a.956.956 0 0 1-.957-.957V3.87a.957.957 0 0 1 .956-.957h18.174a.956.956 0 0 1 .957.957"
						stroke-width="1"
					/><path
						stroke="#191919"
						stroke-linecap="round"
						stroke-linejoin="round"
						d="M22.043 17.26L16.304 23v-4.783a.957.957 0 0 1 .957-.956z"
						stroke-width="1"
					/></g
				></svg
			></span
		>
		<span>Exam Timetable Released</span>
	</div>

	<div class="flex-shrink-0 flex items-center space-x-2">
		<span
			><svg xmlns="http://www.w3.org/2000/svg" width="38" height="38" viewBox="0 0 512 512"
				><path
					fill="#c2ccce"
					d="M505.999 104.494a23.07 23.07 0 0 0-19.614-19.615l-.329-.329H22.572l-.327.329A23.07 23.07 0 0 0 2.63 104.494l-.328.327v298.987l.328.329a23.07 23.07 0 0 0 19.615 19.615l.327.327h463.483l.329-.329a23.06 23.06 0 0 0 19.614-19.614l.329-.329V104.821z"
				/><path fill="#597b91" d="M2.302 149.609h504.024V236H2.302z" /><path
					fill="#fff"
					d="M442.478 294.697H69.522c-23.116 0-41.855 18.739-41.855 41.854c0 23.116 18.739 41.855 41.855 41.855h372.957c23.116 0 41.855-18.739 41.855-41.855c-.001-23.115-18.74-41.854-41.856-41.854"
				/><path
					fill="#597b91"
					d="M348.576 371.698q-1.694 0-3.326-.072c-13.51-.604-22.237-4.798-27.875-9.934c-19.207 9.371-42.187 13.168-51.84 4.363c-3.646-3.324-8.474-10.958.139-24.728c6.98-11.159 8.596-20.652 4.021-23.623c-5.534-3.594-19.407-.151-28.546 13.417c-7.215 10.713-20.291 21.218-34.977 28.101c-7.572 3.549-26.516 11.043-38.877 4.004c-6.398-3.643-15.306-13.61-3.072-39.438c1.489-3.144 1.483-4.788 1.364-5.117c-2.353-2.743-22.062-1.928-42.894 9.78c-13.271 7.458-20.56 16.171-18.57 22.195a7.501 7.501 0 0 1-14.244 4.705c-4.067-12.314 2.827-25.195 19.411-36.271c18.365-12.266 52.469-23.503 66.095-11.737c3.506 3.026 8.478 10.021 2.394 22.866c-4.848 10.233-6.078 18.263-3.062 19.979c8.7 4.959 40.956-8.093 53.991-27.447c6.122-9.09 14.594-15.913 23.857-19.215c9.37-3.34 18.591-2.759 25.3 1.596c9.678 6.284 14.898 21.184.527 44.159c-2.144 3.428-2.468 5.253-2.509 5.876c3.303 2.229 18.115.825 33.107-6.037c-2.906-8.005-2.909-17.684.06-27.01c3.132-9.841 8.966-17.644 15.605-20.872c10.473-5.092 18.629 1.841 22.433 9.324c7.173 14.11 1.809 29.42-14.717 42.004q-.484.37-.981.735c20.276 10.854 64.889-6.649 84.099-15.161a7.5 7.5 0 0 1 6.077 13.715c-29.741 13.177-54.27 19.843-72.99 19.843m-16.932-57.141c-1.332.248-5.402 3.743-8.013 11.238c-1.632 4.685-2.439 10.385-1.314 15.562q.544-.4 1.081-.811c7.26-5.556 14.942-14.089 10.318-23.186c-1.031-2.028-1.84-2.655-2.072-2.803"
				/></svg
			></span
		>
		<span>Pay Fees Online</span>
	</div>

	<div class="flex-shrink-0 flex items-center space-x-2">
		<span
			><svg xmlns="http://www.w3.org/2000/svg" width="38" height="38" viewBox="0 0 128 128"
				><path
					fill="#424242"
					d="M99.06 91.42S83.95 105.6 63.97 105.6S28.89 91.42 28.89 91.42s-2.81-13.49 4.45-36.78c3.83-12.28 58.33-13.53 62.6-2.79c7.26 18.23 3.12 39.57 3.12 39.57"
				/><path
					fill="#212121"
					d="m28.89 91.42l4.79 3.84s-.04-7.6 2.31-14.69c.88-2.65 4.02-3.76 6.38-2.27l18.29 11.47a6.39 6.39 0 0 0 6.7.05c8.74-5.3 31.54-19.17 32.58-20.02c0 0 0-1.71-.43-3.89L28.63 66z"
				/><path
					fill="#424242"
					d="m122.81 52.03l-56.8 33.83c-1.24.74-2.79.74-4.04 0L5.19 52.03c-1.58-.94-1.58-3.23 0-4.17l56.8-33.83c1.24-.74 2.79-.74 4.04 0l56.8 33.83c1.57.94 1.57 3.23-.02 4.17"
				/><path
					fill="#9e9e9e"
					d="M64.04 83.38c-.01 0-.03.01-.04.01c-.16 0-.32-.04-.46-.13L4.18 49.04s-.29.55 0 1.54c.3.99.76 1.31 1.01 1.46l56.8 33.83c.62.37 1.32.56 2.02.56h.04v-3.05z"
				/><path
					fill="#616161"
					d="M64 83.38c.01 0 .03.01.04.01c.16 0 .32-.04.46-.13l59.36-34.22s.29.55 0 1.54c-.3.99-.76 1.31-1.01 1.46l-56.8 33.83c-.62.37-1.32.56-2.02.56h-.04v-3.05z"
				/><path
					fill="#424242"
					d="m35.45 70.06l.32-2.81S60.28 53.92 62.7 52.52s4.96-2.96 6.09-4.21c2-2.2.56-3.58.56-3.58s-1.58 2.56-5.35 2.11c-2.16-.26-4.97-2.01-5.44-2.83s-27.67 19.9-27.67 19.9l-.19 3.33z"
				/><path
					fill="#e2a610"
					d="M69.35 44.74c-2.62 3.66-7.06 2.06-7.06 2.06s-13.91 6.67-14.43 5.66s11.49-7.19 11.49-7.19s-.67-2.46-.6-3.51c0 0-21.72 13.82-29.87 18.47c-4.27 2.44-5.18 4.74-5.17 7.98c0 1.42.02 6.03.04 8.78c0 .51-.22.99-.61 1.31a5.16 5.16 0 0 0-1.89 3.99c0 1.53.67 2.9 1.73 3.85c.57.51.45 1.61.5 2.32c.1 1.36 0 1.98-.56 3.24c-.55 1.23-1.06 2.49-1.41 3.79c-.27 1-.45 2.03-.63 3.05c-1.19 6.83-1.73 14.13-4.88 20.41a.993.993 0 0 0 .45 1.34a1.007 1.007 0 0 0 1.35-.44c1.64-3.27 2.49-6.85 3.19-10.4c-.04 3.21-.06 6.45-.17 9.95c-.02.68-.07 2.05.55 2.35c2.33 1.13 2.33-2.35 2.33-2.35s.03 3.13 3.2 3.13s3.4-3.13 3.4-3.13s.23 2.87 1.86 2.73c.66-.06 1.53-.46 1.22-3.89c-.31-3.42-1.08-15.68-1.41-19.56c-.46-5.37-2.22-8.56-2.58-10.46c-.13-.72-.14-1.47.43-1.94a5.165 5.165 0 0 0 .13-7.88a1.71 1.71 0 0 1-.58-1.42c.19-2.59.4-6.35.57-7.22c.74-3.91 2.67-4.61 4.65-5.77c1.98-1.17 30.66-14.19 32.33-15.3c3.09-2.07 2.43-3.95 2.43-3.95"
				/><path
					fill="#ffca28"
					d="M69.35 44.74c-2.47 3.49-7.6 1.93-7.6 1.93s-13.11 5.81-12.24 4.76c.86-1.05 9.84-6.16 9.84-6.16s-.67-2.46-.6-3.51c0 0-22.1 12.77-30.67 18.91c-2.21 1.59-4.95 4.19-2.72 6.78c1.03 1.19 3.02 1.44 4.29.5c.77-.56 1.37-1.38 2.05-2.03c.84-.82 1.86-1.34 2.86-1.93c1.98-1.17 30.66-14.19 32.33-15.3c3.12-2.07 2.46-3.95 2.46-3.95"
				/><path
					fill="#9e740b"
					d="M26.11 91.86c-1.32 0-2.21-.11-3.02-.3a.62.62 0 0 1-.48-.65l.26-3.82c.03-.39.4-.66.78-.55c.9.26 2.7.52 5.64-.1c.36-.08.72.17.76.54l.4 3.8c.03.31-.17.6-.47.67c-1.53.35-2.64.41-3.87.41"
				/><path
					fill="#616161"
					d="M99.06 91.42s1.77-9.24 1.06-19.07c-.12-1.66-1.14-3.09-1.93 2.72c-.45 3.33-1.43 13.3-3.1 19.53c2.55-1.84 3.97-3.18 3.97-3.18M65.73 36.79c.73.23 1.4.79 1.59 1.54c.25 1-.38 2-1.06 2.78c-1.33 1.53-3.16 2.87-5.19 2.8c-.67-.02-1.39-.24-1.8-.77c-.29-.37-.39-.85-.42-1.32c-.18-3.43 3.7-6.03 6.88-5.03"
				/></svg
			></span
		>
		<span>NUGA 2026 Hosting </span>
	</div>
</section>

<!-- IDID BY NUMBER -->
<section class="justify-center text-center space-y-4 px-6 py-12 bg-gray-100 mx-auto">
	<div class="">
		<h2 class="font-semibold text-4xl">UNICAL IDID BY NUMBER</h2>
		<p class="text-lg">Explore our comprehensive academic and research infrastructure</p>
	</div>

	<section class="grid sm:grid-cols-2 lg:grid-cols-4">
		<div class="p-4 flex flex-col items-center space-y-4 text-start mx-auto shadow-xl w-fit">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRDHtumyPFPD5JHePUORdC4Te5lj_mG_jSsDQ&s"
				alt=""
				class="w-72 h-72"
			/>

			<!-- /// -->
			<div class="w-full space-y-3">
				<div class="text-3xl font-semibold flex items-center justify-between mx-auto">
					<h3>Faculties</h3>
					<span class="font-bold"
						><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
							><path
								fill="currentColor"
								d="M18 7.05a1 1 0 0 0-1-1L9 6a1 1 0 0 0 0 2h5.56l-8.27 8.29a1 1 0 0 0 0 1.42a1 1 0 0 0 1.42 0L16 9.42V15a1 1 0 0 0 1 1a1 1 0 0 0 1-1Z"
							/></svg
						></span
					>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Faculties</h3>
					<span class="font-bold text-2xl">234</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Departments</h3>
					<span class="font-bold text-2xl">45</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Students</h3>
					<span class="font-bold text-2xl">945,344</span>
				</div>
			</div>

			<!-- image block -->
			<div class="flex items-center gap-3 w-full pt-3">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ68xCJyjzwUC0J89fXPOkmIvW09vTZjHRkVg&s"
					alt=""
					class="w-11 h-11 rounded-full"
				/>
				<div class="text-sm">
					<p class="font-semibold text-sm">University of Calabar VC</p>
					<p class="text-gray-500 text-sm">
						Professor <span class="underline">Offiong Efanga Offiong</span>
					</p>
				</div>
			</div>
		</div>

		<div class="p-4 flex flex-col items-center space-y-4 text-start mx-auto shadow-xl w-fit">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR1LKmFG6CM0OQ2yx92vsyx5NLiG3tUJLERIw&s"
				alt=""
				class="w-72 h-72"
			/>

			<!-- /// -->
			<div class="w-full space-y-3">
				<div class="text-3xl font-semibold flex items-center justify-between mx-auto">
					<h3>Departments</h3>
					<span class="font-bold"
						><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
							><path
								fill="currentColor"
								d="M18 7.05a1 1 0 0 0-1-1L9 6a1 1 0 0 0 0 2h5.56l-8.27 8.29a1 1 0 0 0 0 1.42a1 1 0 0 0 1.42 0L16 9.42V15a1 1 0 0 0 1 1a1 1 0 0 0 1-1Z"
							/></svg
						></span
					>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Faculties</h3>
					<span class="font-bold text-2xl">234</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Departments</h3>
					<span class="font-bold text-2xl">45</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Students</h3>
					<span class="font-bold text-2xl">945,344</span>
				</div>
			</div>

			<!-- image block -->
			<div class="flex items-center gap-3 w-full pt-3">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ68xCJyjzwUC0J89fXPOkmIvW09vTZjHRkVg&s"
					alt=""
					class="w-11 h-11 rounded-full"
				/>
				<div class="text-sm">
					<p class="font-semibold text-sm">Head of Departments</p>
					<p class="text-gray-500 text-sm">
						Professor <span class="underline">Offiong Efanga Offiong</span>
					</p>
				</div>
			</div>
		</div>

		<div class="p-4 flex flex-col items-center space-y-4 text-start mx-auto shadow-xl w-fit">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSVylJrbsgRnU9X-X0YdJGB9Alf9wpegkdWtw&s"
				alt=""
				class="w-72 h-72"
			/>

			<!-- /// -->
			<div class="w-full space-y-3">
				<div class="text-3xl font-semibold flex items-center justify-between mx-auto">
					<h3>Staffs</h3>
					<span class="font-bold"
						><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
							><path
								fill="currentColor"
								d="M18 7.05a1 1 0 0 0-1-1L9 6a1 1 0 0 0 0 2h5.56l-8.27 8.29a1 1 0 0 0 0 1.42a1 1 0 0 0 1.42 0L16 9.42V15a1 1 0 0 0 1 1a1 1 0 0 0 1-1Z"
							/></svg
						></span
					>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Faculties</h3>
					<span class="font-bold text-2xl">234</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Departments</h3>
					<span class="font-bold text-2xl">45</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Students</h3>
					<span class="font-bold text-2xl">945,344</span>
				</div>
			</div>

			<!-- image block -->
			<div class="flex items-center gap-3 w-full pt-3">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ68xCJyjzwUC0J89fXPOkmIvW09vTZjHRkVg&s"
					alt=""
					class="w-11 h-11 rounded-full"
				/>
				<div class="text-sm">
					<p class="font-semibold text-sm">Head of Staff Affairs</p>
					<p class="text-gray-500 text-sm">
						Professor <span class="underline">Offiong Efanga Offiong</span>
					</p>
				</div>
			</div>
		</div>

		<div class="p-4 flex flex-col items-center space-y-4 text-start mx-auto shadow-xl w-fit">
			<img
				src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyMO2fuyjikP09AWCdLqN5BMn0JJokSNlTuA&s"
				alt=""
				class="w-72 h-72"
			/>

			<!-- /// -->
			<div class="w-full space-y-3">
				<div class="text-3xl font-semibold flex items-center justify-between mx-auto">
					<h3>Students</h3>
					<span class="font-bold"
						><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
							><path
								fill="currentColor"
								d="M18 7.05a1 1 0 0 0-1-1L9 6a1 1 0 0 0 0 2h5.56l-8.27 8.29a1 1 0 0 0 0 1.42a1 1 0 0 0 1.42 0L16 9.42V15a1 1 0 0 0 1 1a1 1 0 0 0 1-1Z"
							/></svg
						></span
					>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Faculties</h3>
					<span class="font-bold text-2xl">234</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Departments</h3>
					<span class="font-bold text-2xl">45</span>
				</div>
				<div class="flex items-center justify-between mx-auto">
					<h3 class="text-gray-500 text-lg">Number of Students</h3>
					<span class="font-bold text-2xl">945,344</span>
				</div>
			</div>

			<!-- image block -->
			<div class="flex items-center gap-3 w-full pt-3">
				<img
					src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ68xCJyjzwUC0J89fXPOkmIvW09vTZjHRkVg&s"
					alt=""
					class="w-11 h-11 rounded-full"
				/>
				<div class="text-sm">
					<p class="font-semibold text-sm">Head of Student Affairs</p>
					<p class="text-gray-500 text-sm">
						Professor <span class="underline">Offiong Efanga Offiong</span>
					</p>
				</div>
			</div>
		</div>
	</section>
</section>

<!-- IDID serivices -->
<section class="justify-center text-center space-y-4 px-6 py-12">
	<h1 class="text-4xl font-semibold">IDID Services</h1>
	<p class="text-lg lg:text-xl">
		Your gateway to seamless digital identity and access management at UNICAL
	</p>

	{#each services as service}
		<div
			class="lg:flex items-center space-x-4 p-6 text-start justify-center mx-auto gap-12 bg-gray-100/50 rounded-md"
		>
			<img src={service.img} alt={service.title} class="w-[500px] h-[250px] object-cover" />

			<div class="flex flex-col space-y-4 py-4 lg:py-0">
				<h2 class="text-2xl lg:text-4xl font-semibold">{service.title}</h2>
				<p class="text-lg lg:text-xl">{@html service.description}</p>
				<button class="bg-blue-600 p-3 px-6 text-white w-fit"
					><a href={service.button.link}>{service.button.text}</a></button
				>
			</div>
		</div>
	{/each}
</section>

<!-- news & notices -->
<section class="justify-center text-center space-y-4 px-6 py-12 bg-gray-100/50 mx-auto">
	<h1 class="text-4xl font-semibold">University News & Notices</h1>
	<p class="text-lg lg:text-xl">Stay informed with the latest news and events from UNICAL</p>

	<section class="grid lg:grid-cols-2 gap-12 justify-center mx-auto pt-8 w-full">
		<div class="col-span-full flex justify-between items-center w-full">
			<h2 class="text-2xl md:text-4xl font-semibold text-blue-600">Campus Updates</h2>
			<a
				href="#"
				class="hidden sm:flex text-gray-600 font-semibold text-lg md:text-2xl cursor-pointer underline"
				>See all News</a
			>
		</div>
		{#each news as news}
			<div class="md:flex text-start gap-6 items-center shadow-md">
				<img src={news.img} alt={news.heading} class="w-[300px] h-[320px] object-cover" />
				<div class="flex flex-col space-y-4 p-3">
					<h3 class="font-semibold text-lg lg:text-2xl">{news.heading}</h3>
					<p class="text-md">{news.description}</p>
					<a href={news.link} class="text-gray-600 font-semibold underline text-xl">Read more</a>
				</div>
			</div>
		{/each}

		<a
			href="#"
			class="sm:hidden text-gray-600 font-semibold text-lg md:text-2xl cursor-pointer underline"
			>See all News</a
		>
	</section>
</section>

<!-- UNICAL 4.0 -->
<section
	class="relative py-12 my-12 bg-cover bg-center"
	style="background-image: url('https://media.gettyimages.com/id/1066324992/photo/graduation-day.jpg?s=612x612&w=gi&k=20&c=r4OR-dcAzA8hrFo3ANSvipFcG6iCBnpo6jsZPgsayfo=');"
>
	<!-- Dark overlay -->
	<div class="absolute inset-0 bg-gray-200/60"></div>

	<!-- Content -->
	<div class="relative z-10 flex h-full items-center justify-center px-6 w-full">
		<div class="max-w-5xl text-center text-black space-y-6">
			<h1 class="text-4xl md:text-5xl font-bold leading-tight">UNICAL 4.0</h1>

			<p class="text-base md:text-2xl text-black w-full">
				Celebrating <strong>50 years of academic excellence</strong>, UNICAL stands as a beacon of
				<br />
				knowledge, innovation, and cultural heritage. Over the past five decades, we have <br />
				nurtured leaders, advanced research, and fostered a global community committed <br /> to
				making a difference. Join us as we honor our past, celebrate our present, and <br /> shape the
				future together.
			</p>
		</div>
	</div>
</section>

<!-- featured events -->
<section class="justify-center text-center space-y-4 px-6 py-12 bg-gray-100/50 mx-auto my-12">
	<section class="grid lg:grid-cols-2 gap-12 justify-center mx-auto pt-8 w-full">
		<div class="col-span-full flex justify-between items-center w-full">
			<h2 class="text-xl sm:text-2xl md:text-4xl font-bold">Featured events</h2>
			<a
				href="#"
				class="hidden sm:flex text-gray-600 font-bold text-lg md:text-2xl cursor-pointer underline"
				>See all Events</a
			>
		</div>
		{#each events as event}
			<div class="sm:flex text-start gap-6 items-center shadow-md">
				<img src={event.img} alt={event.date} class="sm:w-[300px] h-[320px] object-cover" />
				<div class="flex flex-col space-y-4 p-3">
					<h3 class="font-semibold text-lg lg:text-2xl">{@html event.date}</h3>
					<p class="text-md">{@html event.description}</p>
					<a href={event.link.url} class="font-bold underline text-xl">{event.link.title}</a>
				</div>
			</div>
		{/each}

		<a
			href="#"
			class="pt-8 sm:hidden text-gray-600 font-bold text-lg md:text-2xl cursor-pointer underline"
			>See all Events</a
		>
	</section>
</section>

<!-- digital technology courses -->
<section class="py-12 max-w-7xl justify-center items-center mx-auto px-4">
	<div class="sm:flex text-start gap-6 items-center shadow-lg">
		<img
			src="https://i0.wp.com/opportunitycell.com/wp-content/uploads/2020/11/2020.132_BAM_CA_10-free-short-courses-to-upskill_940x485.jpg?fit=940%2C485&ssl=1"
			alt="digital-technology-courses-image"
			class="w-[400px] lg:w-[500px] h-[320px] object-cover"
		/>
		<div class="flex flex-col space-y-4 p-3">
			<h3 class="font-bold text-lg lg:text-4xl">Digital Technology Courses</h3>
			<p class="text-lg">
				Take Advantage of our digital technology course, and gain new skills <br /> this summer.
			</p>
			<p class="text-lg">Free whatsapp courses</p>
			<Button icon={Add} class="w-fit">Learn More</Button>
		</div>
	</div>
</section>
