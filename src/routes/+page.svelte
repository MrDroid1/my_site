<script>
	import MainGreeting from '../components/MainGreeting.svelte';
</script>
<MainGreeting>
	<div class="space-y-3">
		<h1 class="h1 text-center">
			Привет
		</h1>
		<h1 class="h1">
			Я
			<span class="bg-gradient-to-br from-red-500 to-yellow-500 bg-clip-text text-transparent box-decoration-clone">
				Андрей!
			</span>
		</h1>
	</div>
</MainGreeting>
<div class="container h-full mx-auto flex justify-center items-center mt-10">
	<div class="card w-5/6 p-6 text-2xl variant-soft-surface">
		Всем говорю, что я
		<span class="font-bold bg-gradient-to-br from-purple-500 to-blue-500 bg-clip-text text-transparent box-decoration-clone">
			lead software engineer.
		</span>
		МСМК по созвонам.
	</div>
</div>
<div class="container h-full mx-auto flex justify-center items-center mt-2">
	<div class="card w-5/6 p-6 text-2xl variant-soft-surface">
		<span class="font-bold bg-gradient-to-br from-red-500 to-amber-500 bg-clip-text text-transparent box-decoration-clone">
			Не хочу
		</span>
		во
		<span class="font-bold bg-gradient-to-br from-red-500 to-amber-500 bg-clip-text text-transparent box-decoration-clone">
			frontend.
		</span>
		Кто-то любит делать красиво и умеет верстать, но не я. Проигрываю в шрифты и цвета.
	</div>
</div>
<div class="container h-full mx-auto flex justify-center items-center mt-2">
	<div class="card w-5/6 p-6 text-2xl variant-soft-surface">
		Аки рыба в воде и пиво в кружке обитаю на
		<span class="font-bold bg-gradient-to-br from-fuchsia-500 to-rose-500 bg-clip-text text-transparent box-decoration-clone">
			backend
		</span>'е.
		Мой код
		<span class="font-bold bg-gradient-to-br from-fuchsia-500 to-rose-500 bg-clip-text text-transparent box-decoration-clone">
			решает проблемы,
		</span>
		работает
		<span class="font-bold bg-gradient-to-br from-fuchsia-500 to-rose-500 bg-clip-text text-transparent box-decoration-clone">
			быстро
		</span>
		и
		<span class="font-bold bg-gradient-to-br from-fuchsia-500 to-rose-500 bg-clip-text text-transparent box-decoration-clone">
			жрет мало памяти.
		</span>
	</div>
</div>
<div class="container h-full mx-auto flex justify-center items-center mt-2">
	<div class="card w-5/6 p-6 text-2xl variant-soft-surface">
		Основной стек - 
		<span class="font-bold bg-gradient-to-br from-green-500 to-yellow-500 bg-clip-text text-transparent box-decoration-clone">
			TypeScript, Node.js, MongoDB, Zoom, Пиво
		</span>
	</div>
</div>
<div class="container h-full mx-auto flex justify-center my-2 text-2xl text-center">
	<div class="w-5/6">
		<div class="grid grid-cols-3 gap-2 justify-items-stretch">
			<div class="card p-4 variant-soft-surface col-span-3 xl:col-span-1 md:col-span-1">
				<div>Много обо мне</div>
				<button type="button" class="btn variant-soft-surface mt-4">
					<a href="/about">Перейти</a>
				</button>
			</div>
			<div class="card p-4 variant-soft-surface col-span-3 xl:col-span-1 md:col-span-1">
				<div>Опыт работы</div>
				<button type="button" class="btn variant-soft-surface mt-4">
					<a href="/experience">Перейти</a>
				</button>
			</div>
			<div class="card p-4 variant-soft-surface col-span-3 xl:col-span-1 md:col-span-1">
				<div>FAQ</div>
				<button type="button" class="btn variant-soft-surface mt-4 self-end">
					<a href="/faq">Перейти</a>
				</button>
			</div>
		</div>
	</div>
</div>
