<script>
	import { Accordion, AccordionItem } from "@skeletonlabs/skeleton";
	import BackButton from "../../components/BackButton.svelte";
	import MainGreeting from "../../components/MainGreeting.svelte";

  const questions = [
    {
      question: 'Рассматриваете предложения по работе?',
      answer: 'Нет'
    },
    {
      question: 'Как на счет фронтовых вакансий?',
      answer: 'Графический интерфейс для слабаков, посоны на терминалах'
    },
    {
      question: 'Какой Ваш самый любимый динозавр?',
      answer: 'Тиранозавр!'
    },
    {
      question: 'Что для Вас идеальная команда?',
      answer: 'Вот чтобы такой смотришь и думаешь "Вот щас точно в дрова будем"'
    },
    {
      question: 'Может Java?',
      answer: 'Не дай Бог'
    },
    {
      question: 'А как на счет GO?',
      answer: 'Не хотелось бы уходить от JS\'а, но против ничего не имею'
    },
    {
      question: 'А может по харду Rust?',
      answer: 'А вот это можно, если уж страдать то до конца!'
    },
    {
      question: 'Сколько потоков в JS?',
      answer: 'У нас в JS только 1 праведный поток, остальные небогоугодные'
    },
    {
      question: 'Какие у Вас сильные стороны?',
      answer: 'Я знаю 3 версии анекдота про нюансы'
    },
    {
      question: 'Какой самый великолепный язык программирования?',
      answer: 'Русский топ'
    },
    {
      question: 'Что Вы можете создать?',
      answer: 'Все, я могу все, было бы время'
    },
    {
      question: 'Как работает event loop?',
      answer: 'С кайфом'
    },
  ];
</script>
<MainGreeting>
  <h1 class="h1">
    Частые задаваемые 
    <span class="bg-gradient-to-br from-green-500 to-emerald-500 bg-clip-text text-transparent box-decoration-clone">
      вопросы
      <i class="fa-solid fa-fire-extinguisher"></i>
    </span>
  </h1>
</MainGreeting>
<BackButton />
<div class="container text-xl w-5/6 h-full mx-auto flex justify-center items-center mt-10">
	<Accordion autocollapse>
    {#each questions as { question, answer } }
      <AccordionItem class="rounded-lg variant-soft-surface">
        <svelte:fragment slot="lead">
          <i class="fa-solid fa-circle-info"></i>
        </svelte:fragment>
        <svelte:fragment slot="summary">{question}</svelte:fragment>
        <svelte:fragment slot="content">{answer}</svelte:fragment>
      </AccordionItem>
    {/each}
  </Accordion>
</div>
<BackButton />