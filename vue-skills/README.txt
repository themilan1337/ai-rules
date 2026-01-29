# initial
/plugin marketplace add onmax/nuxt-skills

# required
/plugin install vue@nuxt-skills
/plugin install nuxt@nuxt-skills
/plugin install vueuse@nuxt-skills
/plugin install pnpm@nuxt-skills

# optional (recommended)
/plugin install motion@nuxt-skills
/plugin install nuxt-modules@nuxt-skills
/plugin install nuxt-seo@nuxt-skills
/plugin install vite@nuxt-skills

Поставить:
pnpm i npm-agentskills

и nuxt-модуль:
export default defineNuxtConfig({
  modules: ['npm-agentskills/nuxt'],
  agents: {
    targets: ['cursor', 'claude']
  }
})

Использовать модули, где уже есть skills (nuxt-better-auth).
Проверять, как меняется качество генерации.