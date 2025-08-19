<template>
  <div class="bg-white text-gray-900 dark:bg-gray-950 dark:text-gray-100 antialiased min-h-screen">
    <!-- Nav -->
    <header class="sticky top-0 z-30 border-b border-gray-200/60 dark:border-gray-800/60 backdrop-blur bg-white/80 dark:bg-gray-950/70">
      <div class="mx-auto max-w-7xl px-4 sm:px-6">
        <div class="relative flex h-16 items-center justify-center">
          <nav class="flex items-center gap-8">
            <a href="#" class="inline-flex items-center gap-2">
              <svg class="h-7 w-7" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 2l3.09 6.26L22 9.27l-5 4.85L18.18 22 12 18.77 5.82 22 7 14.12l-5-4.85 6.91-1.01L12 2z"/></svg>
              <span class="text-lg font-semibold tracking-tight">{{ msg }}</span>
            </a>
            <ul class="hidden md:flex items-center gap-6 text-sm">
              <li><a href="#features" class="hover:text-indigo-600 dark:hover:text-indigo-400">Возможности</a></li>
              <li><a href="#demos" class="hover:text-indigo-600 dark:hover:text-indigo-400">Демки</a></li>
              <li><a href="#contact" class="hover:text-indigo-600 dark:hover:text-indigo-400">Контакты</a></li>
            </ul>
          </nav>
          <div class="absolute right-4 flex items-center gap-3">
            <button @click="toggleTheme" class="rounded-xl border border-gray-200 dark:border-gray-800 px-3 py-1.5 text-xs font-medium hover:bg-gray-50 dark:hover:bg-gray-900">
              {{ isDark ? 'Тёмная' : 'Светлая' }}
            </button>
            <a href="#contact" class="hidden sm:inline-block rounded-xl bg-indigo-600 px-3.5 py-2 text-xs font-semibold text-white hover:bg-indigo-500">Связаться</a>
          </div>
        </div>
      </div>
    </header>

    <!-- Hero -->
    <section class="relative">
      <div class="mx-auto max-w-7xl px-4 sm:px-6">
        <div class="grid items-center gap-10 py-16 sm:py-20 md:grid-cols-2">
          <div class="space-y-6">
            <p class="inline-flex items-center gap-2 rounded-full border border-indigo-200/60 dark:border-indigo-900/50 bg-indigo-50/60 dark:bg-indigo-900/20 px-3 py-1 text-xs text-indigo-700 dark:text-indigo-300">Новый релиз · v1.0</p>
            <h1 class="text-4xl font-extrabold tracking-tight sm:text-5xl">Соберите современный лендинг <span class="text-indigo-600 dark:text-indigo-400">за минуты</span></h1>
            <p class="text-base text-gray-600 dark:text-gray-300">Готовый шаблон на Tailwind CSS: центрированный навбар, hero-секция, блоки демо, контакты и аккуратный футер. Лёгкая тёмная тема в комплекте.</p>
            <div class="flex flex-wrap gap-3">
              <a href="#demos" class="inline-flex items-center justify-center rounded-xl bg-indigo-600 px-5 py-3 text-sm font-semibold text-white hover:bg-indigo-500">Смотреть демо</a>
              <a href="#features" class="inline-flex items-center justify-center rounded-xl border border-gray-300 dark:border-gray-800 px-5 py-3 text-sm font-semibold hover:bg-gray-50 dark:hover:bg-gray-900">Подробнее</a>
            </div>
          </div>
          <div class="relative">
            <div class="aspect-[16/10] w-full overflow-hidden rounded-2xl border border-gray-200 dark:border-gray-800 bg-gradient-to-br from-indigo-100 to-indigo-50 dark:from-indigo-900/30 dark:to-indigo-800/10">
              <div class="flex h-full w-full items-center justify-center">
                <span class="text-sm text-gray-500 dark:text-gray-400">Здесь может быть ваш скриншот/превью</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Features / Demos wrapper -->
    <section id="features" class="border-t border-gray-200/60 dark:border-gray-800/60">
      <div class="mx-auto max-w-7xl px-4 sm:px-6 py-16 sm:py-20">
        <div class="mx-auto max-w-2xl text-center">
          <h2 class="text-3xl font-bold tracking-tight sm:text-4xl">Почему именно этот шаблон</h2>
          <p class="mt-3 text-gray-600 dark:text-gray-300">Минимум кода — максимум практики. Адаптивность, доступность и продуманная сетка по умолчанию.</p>
        </div>

        <!-- Demos grid (two sections with image + text) -->
        <div id="demos" class="mt-12 grid gap-10 lg:gap-12">
          <!-- Demo 1 -->
          <div class="grid items-center gap-8 md:grid-cols-2">
            <div class="order-2 md:order-1">
              <h3 class="text-2xl font-semibold">Демо #1 — Панель управления</h3>
              <p class="mt-3 text-gray-600 dark:text-gray-300">Покажите, как выглядит ваш продукт: карточки, таблицы, графики. Добавьте краткое описание преимуществ и CTA.</p>
              <div class="mt-5 flex gap-3">
                <a href="#contact" class="rounded-xl bg-indigo-600 px-4 py-2 text-sm font-semibold text-white hover:bg-indigo-500">Попробовать</a>
                <a href="#" class="rounded-xl border border-gray-300 dark:border-gray-800 px-4 py-2 text-sm font-semibold hover:bg-gray-50 dark:hover:bg-gray-900">Документация</a>
              </div>
            </div>
            <div class="order-1 md:order-2">
              <div class="aspect-[16/10] overflow-hidden rounded-2xl border border-gray-200 dark:border-gray-800 bg-gray-50 dark:bg-gray-900">
                <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?q=80&w=1200&auto=format&fit=crop" alt="Demo dashboard" class="h-full w-full object-cover" />
              </div>
            </div>
          </div>

          <!-- Demo 2 -->
          <div class="grid items-center gap-8 md:grid-cols-2">
            <div>
              <div class="aspect-[16/10] overflow-hidden rounded-2xl border border-gray-200 dark:border-gray-800 bg-gray-50 dark:bg-gray-900">
                <img src="https://images.unsplash.com/photo-1555066931-4365d14bab8c?q=80&w=1200&auto=format&fit=crop" alt="Demo analytics" class="h-full w-full object-cover" />
              </div>
            </div>
            <div>
              <h3 class="text-2xl font-semibold">Демо #2 — Аналитика и отчёты</h3>
              <p class="mt-3 text-gray-600 dark:text-gray-300">Продемонстрируйте главные метрики, дайте пользователю понять ценность продукта через цифры и визуализации.</p>
              <div class="mt-5 flex gap-3">
                <a href="#contact" class="rounded-xl bg-indigo-600 px-4 py-2 text-sm font-semibold text-white hover:bg-indigo-500">Запросить доступ</a>
                <a href="#" class="rounded-xl border border-gray-300 dark:border-gray-800 px-4 py-2 text-sm font-semibold hover:bg-gray-50 dark:hover:bg-gray-900">Подробнее</a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="border-t border-gray-200/60 dark:border-gray-800/60">
      <div class="mx-auto max-w-7xl px-4 sm:px-6 py-16 sm:py-20">
        <div class="mx-auto max-w-2xl text-center">
          <h2 class="text-3xl font-bold tracking-tight sm:text-4xl">Свяжитесь с нами</h2>
          <p class="mt-3 text-gray-600 dark:text-gray-300">Оставьте заявку — ответим в ближайшее время.</p>
        </div>

        <form class="mx-auto mt-10 max-w-2xl grid grid-cols-1 gap-6" @submit.prevent>
          <div>
            <label class="mb-2 block text-sm font-medium" for="name">Имя</label>
            <input id="name" type="text" required class="w-full rounded-xl border border-gray-300 dark:border-gray-800 bg-white dark:bg-gray-950 px-4 py-2.5 outline-none focus:ring-2 focus:ring-indigo-500" placeholder="Иван" />
          </div>
          <div>
            <label class="mb-2 block text-sm font-medium" for="email">Email</label>
            <input id="email" type="email" required class="w-full rounded-xl border border-gray-300 dark:border-gray-800 bg-white dark:bg-gray-950 px-4 py-2.5 outline-none focus:ring-2 focus:ring-indigo-500" placeholder="you@example.com" />
          </div>
          <div>
            <label class="mb-2 block text-sm font-medium" for="msg">Сообщение</label>
            <textarea id="msg" rows="5" class="w-full rounded-xl border border-gray-300 dark:border-gray-800 bg-white dark:bg-gray-950 px-4 py-2.5 outline-none focus:ring-2 focus:ring-indigo-500" placeholder="Расскажите кратко о задаче"></textarea>
          </div>
          <div class="flex items-center justify-between">
            <div class="text-xs text-gray-500">Нажимая «Отправить», вы соглашаетесь с обработкой персональных данных.</div>
            <button type="submit" class="rounded-xl bg-indigo-600 px-5 py-2.5 text-sm font-semibold text-white hover:bg-indigo-500">Отправить</button>
          </div>
        </form>
      </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-gray-200/60 dark:border-gray-800/60">
      <div class="mx-auto max-w-7xl px-4 sm:px-6 py-10">
        <div class="flex flex-col items-center justify-between gap-4 sm:flex-row">
          <div class="flex items-center gap-2 text-sm text-gray-600 dark:text-gray-400">
            <svg class="h-5 w-5" viewBox="0 0 24 24" fill="currentColor" aria-hidden="true"><path d="M12 2l3.09 6.26L22 9.27l-5 4.85L18.18 22 12 18.77 5.82 22 7 14.12l-5-4.85 6.91-1.01L12 2z"/></svg>
            <span>© {{ year }} BrandName</span>
          </div>
          <div class="flex items-center gap-5 text-sm">
            <a href="#" class="hover:text-indigo-600 dark:hover:text-indigo-400">Политика</a>
            <a href="#" class="hover:text-indigo-600 dark:hover:text-indigo-400">Документация</a>
            <a href="#contact" class="hover:text-indigo-600 dark:hover:text-indigo-400">Контакты</a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { onMounted, ref } from 'vue'

const year = new Date().getFullYear()
const isDark = ref(false)

onMounted(() => {
  const savedTheme = localStorage.getItem('theme')
  const systemDark = window.matchMedia('(prefers-color-scheme: dark)').matches
  isDark.value = savedTheme ? savedTheme === 'dark' : systemDark
  document.documentElement.classList.toggle('dark', isDark.value)
})

function toggleTheme() {
  isDark.value = !isDark.value
  document.documentElement.classList.toggle('dark', isDark.value)
  localStorage.setItem('theme', isDark.value ? 'dark' : 'light')
}

defineProps({
  msg: String,
})
</script>

<style scoped>
/* Optional: smooth color transition */
:root,
:root.dark {
  transition: color 200ms linear, background-color 200ms linear;
}
</style>
