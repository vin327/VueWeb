<template>
<div class="techrider-header">
    <div class="techrider-name">
        <p class="techrider-name-text">Top “Manhattan” party</p>
    </div>
    <div class="techrider-text-heading">
        <p>ТЕХРАЙДЕР</p>
    </div>
    </div>
    <div class="techrider-conteiner">
        <div class="techrider-list">
        <div class="techrider-list-content">
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindow">
                <template v-if="OpenWindow">
                <div @click="OpenWindow =! OpenWindow" class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">Loudspeakers</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 260.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div @click="OpenWindow =! OpenWindow" class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">Loudspeakers</p>
                    <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 260.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindowTwo">
                <template v-if="OpenWindowTwo">
                <div  @click="OpenWindowTwo =! OpenWindowTwo"  class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">Amplifier</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 313.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">Amplifier</p>
                    <button @click="OpenWindowTwo = !OpenWindowTwo">
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 316.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindowThree">
                <template v-if="OpenWindowThree">
                <div class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div  @click="OpenWindowThree = !OpenWindowThree"  class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">FOH</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 380.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">FOH</p>
                    <button @click="OpenWindowThree = !OpenWindowThree">
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 380.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindowFour">
                <template v-if="OpenWindowFour">
                <div class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div  @click="OpenWindowFour = !OpenWindowFour"  class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">Backline</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 320.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">Backline</p>
                    <button @click="OpenWindowFour = !OpenWindowFour">
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 320.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindowFive">
                <template v-if="OpenWindowFive">
                <div class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div  @click="OpenWindowFive = !OpenWindowFive"  class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">Microphone set</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 240.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">Microphone set</p>
                    <button @click="OpenWindowFive = !OpenWindowFive">
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 240.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
            <Transition name="bounce">
            <!-- Используем один блок, который будет переключаться по ключу -->
            <div :key="OpenWindowSix">
                <template v-if="OpenWindowSix">
                <div class="techrider-list-order-open">
                    <!-- Контент для OpenWindow === true -->
                    <div  @click="OpenWindowSix = !OpenWindowSix"  class="techrider-list-order-open-content">
                    <!-- Заголовок и кнопка -->
                    <div class="techrider-list-order-title" style="margin: 0px 0 20px 0">
                        <p class="techrider-list-order-text">DJ equipment</p>
                        <button>
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 271.1px;" src="../assets/images/techrider-list-arrow.svg" alt="">
                        </button>
                    </div>
                    <!-- Остальной контент -->
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <p class="techrider-list-order-open-text">· Acoustic system BELL Top 600W x 2</p>
                    <!-- ... -->
                    </div>
                </div>
                </template>
                <template v-else>
                <div class="techrider-list-order">
                    <div class="techrider-list-order-title">
                    <p class="techrider-list-order-text">DJ equipment</p>
                    <button @click="OpenWindowSix = !OpenWindowSix">
                        <img style="width: 20.78px; height: 11.96px; margin: 0 0 0 271.1px; transform:rotate(180)" src="../assets/images/techrider-list-arrow.svg" alt="">
                    </button>
                    </div>
                </div>
                </template>
            </div>
            </Transition>
        </div>
        </div>
        <div style="float:left" class="soundEngineers">
        <div class="soundEngineers-header-text">
            <p>Звукорежиссеры клуба МАНХЭТТЕН</p>
        </div>
        <div class="soundEngineers-poster">
            <div class="soundEngineers-poster-order">
            <img src="../assets/images/soundEngineers-poster-1.jpeg" alt="">
            <p style="margin: 30px 0 0 0" class="soundEngineers-name">Изотов Константин</p>
            </div>
            <div class="soundEngineers-poster-order">
            <img src="../assets/images/soundEngineers-poster-2.jpeg" alt="">
            <p style="margin: 30px 0 0 0" class="soundEngineers-name">Давид Хозиев</p>
            </div>
        </div>
        <div class="soundEngineers-contact-main">
            <div class="soundEngineers-contact-conteiner">
            <div class="soundEngineers-btn-contact">
                <img src="../assets/images/icons-btn-vk.svg" alt="">
            </div>
            <div class="soundEngineers-btn-contact">
                <img src="../assets/images/icons-btn-tg.svg" alt="">
            </div>
            </div>
            <div class="soundEngineers-contact-conteiner">
            <div class="soundEngineers-btn-contact">
                <img src="../assets/images/icons-btn-vk.svg" alt="">
            </div>
            <div class="soundEngineers-btn-contact">
                <img src="../assets/images/icons-btn-tg.svg" alt="">
            </div>
            </div>
        </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      OpenWindow: false,
      OpenWindowTwo: false,
      OpenWindowThree: false,
      OpenWindowFour: false,
      OpenWindowFive: false,
      OpenWindowSix: false,
    }
  },
  computed: {

  },
  methods: {

  },
  watch: {

  }
}
</script>
