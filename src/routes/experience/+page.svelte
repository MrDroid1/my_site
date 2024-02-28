<script lang="ts">
	import { Tab, TabGroup } from "@skeletonlabs/skeleton";

  const startYear = 2016;
  const sumOfExp = new Date().getFullYear() - startYear;

  const experience = [
    {
      company: 'Балтинфоком',
      start: 'Август 2016',
      end: 'Декабрь 2017',
      grade: 'Junior',
      stack: [
        "node.js",
        "express",
        "mongodb",
        "neo4j",
        "three.js",
        "phantom.js",
        "electron.js",
        "socker.io",
      ],
      achievements: [
        "Разработал систему сборщиков информации из открытых источников"
      ],
      responsibilities: [
        "Разработка сети сборщиков информации с открытых источников с использованием",
        "Разработка клиентской части приложения для графовой визуализации данных",
      ],
    },
    {
      company: 'Fulldive',
      start: 'Декабрь 2017',
      end: 'Февраль 2019',
      grade: 'Middle',
      stack: [
        'node.js',
        'express',
        'mongodb',
        'redis',
        'neo4j',
        'docker',
        'GCP',
        'AWS'
      ],
      achievements: [
        "Разработал алгоритм хранения данных китайских пользователей в хранилищах гугла",
        "Разработал новое апи для продукта",
      ],
      responsibilities: [
        "Разработка серверной части для виртуального браузера",
        "Поддержание и оптимизация старого кода",
        "Разработка решений с использованием облачных сервисов google и amazon",
      ],
    },
    {
      company: 'OneTwoTrip',
      start: 'Февраль 2019',
      end: 'Ноябрь 2019',
      grade: 'Senior',
      stack: [
        'node.js',
        'express',
        'mongodb',
        'redis',
      ],
      achievements: [
        "Внедрил mongodb как основную базу данных для сервиса",
        "Добавил поддержку es6 по всему проекту",
        "Ускорил работу сервиса по выдачи данных в 3 раза",
      ],
      responsibilities: [
        "Разработка серверной части на Node.js",
        "Оптимизация старого кода",
        "Изменение архитектуры приложения",
        "Разработка нового функционала",
      ],
    },
    {
      company: 'Quantori',
      start: 'Ноябрь 2019',
      end: 'Июнь 2022',
      grade: 'Senior',
      stack: [
        'node.js',
        'k6',
        'Jmeter',
        'express',
        'postgresql',
        'azure',
        'temporal',
        'grafana',
        'docker',
      ],
      achievements: [
        "Создал новый продукт для тестирования физических процессов в лаборатории",
        "Разработал универсальное решение для аналитики данных нагрузочного тестирования",
        "Обучил младших специалистов работать с системой нагрузочного тестирования",
      ],
      responsibilities: [
        "Разработка серверной части ЛИМС системы",
        "Разделение монолита на микросервисы",
        "Разработка решений с использованием облачных сервисов Microsoft Azure",
      ],
    },
    {
      company: 'Леруа Мерлен',
      start: 'Июнь 2022',
      end: 'Сегодня',
      grade: 'Lead',
      stack: [
        'node.js',
        'k6',
        'nest.js',
        'postgresql',
        'mongodb',
        'jaeger',
        'grafana',
        'docker',
        'BPMN',
        'Camunda',
        'PlantUML',
      ],
      achievements: [
        "Не забыть заполнить",
        // "Разработал систему мониторинга и решения проблем мерчантов",
        // "Повысил показатель SLA с 60% до 90%",
        // "Обновил бизнес процесс, что уменьшило количество обращений в поддержку с 40 до 5 штук в день",
      ],
      responsibilities: [
        "Руководство командой",
        "Найм новых сотрудников",
        "Разработка ПО в домене исполнения мерчантских заказов",
        "Оптимизация рабочего процесса",
        "Разработка архитектуры продукта",
        "Модернизация бизнес процесса в нотации bpmn",
      ],
    },
  ].reverse();

  let tabSet: number = 2;
</script>
<div class="container w-1/2 h-full mx-auto flex justify-center items-center mt-10 text-center">
  <div class="w-full">
		<h1 class="h1">
			Мой опыт 
			<span class="bg-gradient-to-br from-lime-500 to-emerald-500 bg-clip-text text-transparent box-decoration-clone">
				работы
        {sumOfExp}
        лет
        <i class="fa-solid fa-person-running"></i>
			</span>
		</h1>
	</div>
</div>
<div class="w-64 p-6 text-3xl font-bold mx-auto flex justify-center items-center mt-10">
  <a href="/" class="btn variant-soft-surface">
    <span><i class="fa-solid fa-caret-left mr-4"></i></span>
    <span>Назад</span>
  </a>
</div>
<div class="container w-5/6 h-full mx-auto flex justify-center items-center mt-10 grid grid-cols-1 gap-4">
	{#each experience as exp}
    <div class="w-full h-full card p-6 variant-soft-surface text-center">
      <header class="card-header">
        <p class="text-6xl font-bold bg-gradient-to-br from-blue-500 to-lime-500 bg-clip-text text-transparent box-decoration-clone">
          {exp.grade}
        </p>
        <span class="mt-2 text-2xl">
          {exp.company}
        </span>
      </header>
      <section class="p-4">
        <div class="card p-6 variant-soft-surface text-xl">
          <TabGroup justify="justify-center">
            <Tab bind:group={tabSet} name="tab1" value={0}>Достижения</Tab>
            <Tab bind:group={tabSet} name="tab2" value={1}>Обязанности</Tab>
            <Tab bind:group={tabSet} name="tab3" value={2}>Стек</Tab>
            <!-- Tab Panels --->
            <svelte:fragment slot="panel">
              {#if tabSet === 0}
                <ul class="list text-left">
                  {#each exp.achievements as ach}
                    <li class="mb-2 p-2">
                      {ach}
                    </li>
                    <hr class="!border-t-1 border-1" />
                  {/each}
                </ul>
              {:else if tabSet === 1}
                <ul class="list text-left">
                  {#each exp.responsibilities as res}
                    <li class="mb-2 p-2">
                      {res}
                    </li>
                    <hr class="!border-t-1 border-1" />
                  {/each}
                </ul>
              {:else if tabSet === 2}
                {#each exp.stack as tech}
                  <span class="chip bg-gradient-to-br variant-gradient-success-warning m-2 text-xl bg-initial">{tech}</span>
                {/each}
              {/if}
            </svelte:fragment>
          </TabGroup>
        </div>
      </section>
	    <footer class="card-footer">
        <p class="mt-4">{exp.start} - {exp.end}</p>
      </footer>
    </div>
  {/each}
</div>
<div class="w-64 p-6 text-3xl font-bold mx-auto flex justify-center items-center mt-10">
  <a href="/" class="btn variant-soft-surface">
    <span><i class="fa-solid fa-caret-left mr-4"></i></span>
    <span>Назад</span>
  </a>
</div>