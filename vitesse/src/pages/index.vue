<script setup lang="ts">
import { useUserStore } from '~/stores/user'

const user = useUserStore()
const name = ref(user.savedName)

const router = useRouter()
const go = () => {
    router.push(`/slides/theory`)
}

const { t } = useI18n()
</script>

<template>
  <div>
    <p class="text-lg">
      Оценка межрегиональной модели «экономического роста»<br>на основе
      агрегированной производственной функции Кобба-Дугласа
    </p>
    <p class="text-sm m-6">
      Лиджигоряева Иляна, Дарья Анисимова, Бузин Глеб.
    </p>
    <p>
      <em class="text-sm opacity-75">анализ чего-то</em>
    </p>

    <div class="py-4" />

    <div>
      <button
        class="m-3 text-sm btn"
        @click="go"
      >
       Поехали
      </button>
    </div>
  </div>
</template>

<route lang="yaml">
meta:
  layout: home
</route>
