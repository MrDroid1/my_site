<script>

	import { ProgressRadial } from "@skeletonlabs/skeleton";
  import BackButton from '../../components/BackButton.svelte';
	import MainGreeting from "../../components/MainGreeting.svelte";

</script>
<MainGreeting>
  <h1 class="h1">
    Много обо 
    <span class="bg-gradient-to-br from-red-500 to-yellow-500 bg-clip-text text-transparent box-decoration-clone">
      мне
      <i class="fa-solid fa-hat-wizard"></i>
    </span>
  </h1>
</MainGreeting>
<BackButton />
<div class="container text-center w-5/6 mx-auto mt-10 grid grid-cols-6 gap-4">
	<div class="w-full h-full card p-6 variant-soft-surface col-span-6 xl:col-span-2 lg:col-span-6 sm:col-span-6">
		<p class="text-5xl font-bold">
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
				Punk's Not Dead
			</span>
    </p>
    <p class="mt-4">Но это не точно</p>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:col-span-1 lg:col-span-3 sm:col-span-6">
    Мастер меча и осушения пивных банок
	</div>
  <div class="w-full h-full card p-6 text-3xl variant-soft-surface col-span-6 xl:col-span-1 lg:col-span-3 sm:col-span-6">
		<p>
      Люблю
      <span class="font-bold bg-gradient-to-br from-green-500 to-yellow-500 bg-clip-text text-transparent box-decoration-clone">
        динозавров
      </span>
    </p>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:col-span-2 lg:col-span-6 sm:col-span-6">
		<p>Всю сознательную жизнь просидел за компом обучаясь разработке.</p>
    <p>По сей день не вставал и не хочу</p>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:row-span-2 xl:col-span-1 lg:col-span-2 sm:col-span-6">
    Уверенность
		<ProgressRadial class="mx-auto mt-6" stroke={120} meter="stroke-success-500" value="{100}" strokeLinecap="round">
      {146}%
    </ProgressRadial>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:row-span-2 xl:col-span-1 lg:col-span-2 sm:col-span-6">
		Резист к ядам
		<ProgressRadial class="mx-auto mt-6" stroke={120} meter="stroke-warning-500" track="stroke-warning-500/30" value="{54}" strokeLinecap="round">
      {54}%
    </ProgressRadial>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:col-span-2 xl:row-span-4 lg:row-span-1 lg:col-span-2 sm:col-span-6">
		<div>
      <img class="rounded-lg" src="https://avatars.dzeninfra.ru/get-zen_doc/1706869/pub_5fbe079c9e832457055a6f45_5fbe0925d81aaf181b43ec9a/scale_1200" alt="Собака">
    </div>
	</div>
  <div class="w-full h-full card p-6 text-6xl variant-soft-surface col-span-6 xl:col-span-2 xl:row-span-1 lg:col-span-6 sm:col-span-6">
    <div class="grid grid-cols-4 gap-4">
      <div>
        <i class="fa-brands fa-js bg-gradient-to-br from-amber-500 to-red-500 bg-clip-text text-transparent box-decoration-clone"></i>
      </div>
      <div>
        <i class="fa-brands fa-node"></i>
      </div>
      <div>
        <i class="fa-brands fa-git"></i>
      </div>
      <div>
        <i class="fa-solid fa-bug-slash"></i>
      </div>
      <div>
        <i class="fa-brands fa-docker"></i>
      </div>
      <div>
        <i class="fa-brands fa-linux"></i>
      </div>
      <div>
        <i class="fa-solid fa-frog bg-gradient-to-br from-lime-500 to-green-500 bg-clip-text text-transparent box-decoration-clone"></i>
      </div>
      <div>
        <i class="fa-solid fa-terminal"></i>
      </div>
    </div>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:col-span-2 xl:row-span-5 lg:col-span-6 sm:col-span-6">
		<p>
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        Разрабатываю ПО.
      </span>
      Думаю о том как правильно
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разрабатывать ПО.
      </span>
      Читаю о
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разработке ПО.
      </span>
      Пишу о том как
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разрабатывать ПО.
      </span>
      Обучаю других нюансам
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разработки ПО.
      </span>
      Руковожу людьми, чтобы
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разрабатывать ПО.
      </span>
      Решаю проблемы
      <span class="bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
        разработкой ПО.
      </span>
    </p>
	</div>
  <div class="w-full h-full card p-6 text-6xl variant-soft-surface col-span-6 xl:col-span-2 xl:row-span-2 lg:col-span-2 sm:col-span-6">
    <div class="grid grid-cols-3 gap-4">
      <div>
        <a href="https://github.com/MrDroid1">
          <i class="fa-brands fa-github"></i>
        </a>
      </div>
      <div>
        <a href="https://t.me/AndrewKirillov">
          <i class="fa-brands fa-telegram bg-gradient-to-br from-blue-500 to-teal-500 bg-clip-text text-transparent box-decoration-clone"></i>
        </a>
      </div>
      <div>
        <a href="https://www.linkedin.com/in/andrew-kirillov-js/">
          <i class="fa-brands fa-linkedin"></i></a>
      </div>
    </div>
	</div>
  <div class="w-full h-full card p-6 text-2xl variant-soft-surface col-span-6 xl:col-span-3 xl:row-span-2 lg:col-span-4 sm:col-span-6">
		Люблю
    <span class="font-bold bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 bg-clip-text text-transparent box-decoration-clone">
      спорт, бары
    </span>
    и разложиться на концертах
	</div>
  <div class="w-full h-full card p-6 text-4xl variant-soft-surface col-span-6 xl:col-span-1 xl:row-span-2 lg:col-span-6 sm:col-span-6">
    <span class="font-bold bg-gradient-to-br from-purple-500 to-blue-500 bg-clip-text text-transparent box-decoration-clone">
      Козерог
    </span>
	</div>
</div>
<BackButton />
