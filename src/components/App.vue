<template>
  <div id="app">
  <div class="modal" v-if = "isShowModal">
    <button type="button" class="exit_icon" @click = "closeModal">
    </button>

    <div class="show">
        <img src="../assets/hood.jpg" alt="черное худи колеса"
        class="image" width="330" height="330">
        <div class="photos">
            <button type="button" class="galleryButtons">
                <img src="../assets/Woman.jpg" alt="девушка в белом худи"
                width="50px" height="50px">
            </button>
            <button type="button" class="galleryButtons">
                <img class="active-preview" src="../assets/miniHood.jpg"
                alt="черное худи колеса" width="50px"
                    height="50px">
            </button>
            <button type="button" class="galleryButtons">
                <img src="../assets/Man.jpg" alt="парень в черном худи"
                width="50px" height="50px">
            </button>
        </div>
    </div>
  <div class="content">
      <h4>
          Футболка "Эволюционируй или сдохни"
      </h4>
      <div class="money">
          <div class="purchase">
              <div class="cost">
                  100 баллов
              </div>
              <button class="button_js" type="button">
                  Заказать
              </button>
          </div>

          <div class="balance">
              <div class="leftBalance">
                  <div class="balance-text">Твой баланс:</div>
                  <div class="numb">
                      3 945 баллов
                  </div>
              </div>
              <div class="shop_icon">
              </div>
          </div>
      </div>
      <div class="buy">
          <div class="color">
              <span class="colorSize">Цвета:</span>
              <div class="radiocolor">
                  <label class="colorLabel checked">
                      <span class="colorInputWrapper">
                          <input class="radio" type="radio" id="color-1"
                          name="color" value="blue" checked />
                          <span class="sizeLabelBox blue"></span>
                      </span>
                      <span class="sizeLabelSpan">Синий</span>
                  </label>

                  <label class="colorLabel">
                      <span class="colorInputWrapper">
                          <input class="radio" type="radio" id="color-2"
                          name="color" value="beige" />
                          <span class="sizeLabelBox  beige"></span>
                      </span>
                      <span class="sizeLabelSpan">Бежевый</span>
                  </label>

                  <label class="colorLabel">
                      <span class="colorInputWrapper">
                          <input class="radio" type="radio" id="color-3"
                          name="color" value="grey" />
                          <span class="sizeLabelBox  grey"></span>
                      </span>
                      <span class="sizeLabelSpan">Серый</span>
                  </label>
              </div>
          </div>

          <div class="size">
              <span class="colorSize">Размер:</span>
              <div class="sizeWrapper">
                  <label class="sizeLabel  checked">
                      <span class="sizeInputWrapper">
                          <input class="radio" label="S" type="radio" id="s-size"
                          name="size" value="S" checked />

                      </span>
                      <span class="sizeLabelSpan">S</span>
                  </label>

                  <label class="sizeLabel">
                      <span class="sizeInputWrapper">
                          <input class="radio" label="M" type="radio" id="m-size"
                          name="size" value="M" />

                      </span>
                      <span class="sizeLabelSpan">M</span>
                  </label>

                  <label class="sizeLabel">
                      <span class="sizeInputWrapper">
                          <input class="radio" label="L" type="radio" id="l-size"
                          name="size" value="L" />

                      </span>
                      <span class="sizeLabelSpan">L</span>
                  </label>
              </div>
          </div>
          <div class="details">
              <div>
                  Детали:
                  <div class="words">
                      Брендированная толстовка от Qazaq Republic. Материал: Хлопок 80%, Вискоза 20%
                  </div>
              </div>
              <div class="material">
              Как выбрать размер:
                  <div class="howChooseText">
                  Написать дяде Рику для уточнения.</div>
              </div>
          </div>
      </div>
  </div>
</div>

    <div class="overlay" v-bind:class = "{overlayOn: isShowModal}" @click = "closeModal"></div>
    <div class="wrapper">
          <div class="main">
              <div class="main_bar">
                  <div class="kolesa_logo">
                      <a>
                      <img src="../assets/logo.svg"
                      alt="kolesa_logo"
                      width="215px"
                      height="35px">
                      </a>
                  </div>
                  <ul class="menu_list">
                      <li><a>Оргсхема</a></li>
                      <li><a>Kolesa <span class="massive">Team</span></a></li>
                      <li class="chosen"><a>Kolesa Shop</a></li>
                      <li><a>Картина компании</a></li>
                      <li><a>Новости</a></li>
                      <li><a>Education</a></li>
                      <li><a>Guidelines</a></li>
                      <li><a>Библиотека</a></li>
                      <li><a>FAQ</a></li>
                  </ul>
              </div>
              <div class="main_content">
                  <div class="search_account">
                      <form class="search">
                          <button class="search_button"
                          type="button"><label
                          for="search"></label></button>
                          <input id="search"
                          type="text"
                          placeholder="Поиск">
                      </form>
                      <a>
                          <div class="account">
                              <img src="../assets/acc.jpg"
                              alt="аватар профиля"
                              width="44px"
                              height="44px">
                              <div class="account_name">
                                  <h4>Мортиджан</h4>
                                  <span>300 баллов</span>
                              </div>
                          </div>
                      </a>
                  </div>
                  <div class="products">
                      <div class="banner">
                          <div class="attention">
                              это пример баннера нельзя использовать
                              нужно попросить у Графического отдела
                          </div>
                          <img src="../assets/Баннер.jpg"
                          alt="баннер с акцией"
                          width="1038px"
                          height="335px">
                      </div>
                      <div class="hot_buttons">
                          <a class="nostyle">
                              <div class="hot_buttons_primary">
                                  <div class="icon_text">
                                      <div class="primary_icon"></div>
                                      Получить Баллы
                                  </div>
                              </div>
                          </a>
                          <a class="nostyle" >
                              <div class="hot_buttons_secondary">
                                  <div class="secondary_icon"></div>
                                  Как Получить Баллы
                              </div>
                          </a>
                          <a class="nostyle" >
                              <div class="hot_buttons_third">
                                  <div class="third_icon"></div>
                                  Подарить Баллы
                              </div>
                          </a>
                      </div>
                      <div class="radio_collection">
                          <div class="radio_button js_radio_button">
                              <input  class = "category" data-key = "all"
                              id="radio-1" type="radio"
                              name="radio" value="everything"
                              @change="onChange($event)"  checked >
                              <label  for="radio-1">Все товары</label>
                          </div>
                          <div class="radio_button js_radio_button">
                              <input class = "category" data-key = "clothes"
                              id="radio-2" type="radio" name="radio" value="clothes"
                              @change="onChange($event)">
                              <label  for="radio-2">Одежда</label>
                          </div>
                          <div class="radio_button js_radio_button">
                              <input  class = "category" data-key = "accessories"
                              id="radio-3" type="radio" name="radio" value="acc"
                              @change="onChange($event)">
                              <label  for="radio-3">Аксессуары</label>
                          </div>
                      </div>
                      <div class="products_gallery js_gallery" >
                          <div class="card" v-for="card in filtered" :key="card.id">
                              <div class="image">
                                  <img :src="card.img" alt="Футболка"
                                  width ="330" height="330">
                                <span v-if="card.isNew" class="badge">NEW</span>
                              </div>
                              <div class="description">
                                  <div class="price">
                                      {{card.price}} баллов
                                  </div>
                                  <h3 class="title">
                                      {{card.title}}
                                  </h3>
                                  <div class="sizes">
                                      Размеры S/M/L
                                  </div>
                                  <div class="butcontain">
                                      <button
                                      class="button"
                                      type="button"
                                      @click="showModal"
                                      >
                                      Заказать
                                  </button>
                                  </div>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>

          </div>
          <footer>
              <div class="info">
                  <div class="contacts">
                      <div class="kolesa_icon">
                          <a>© Kolesa Group</a>
                      </div>
                      <div class="contact_icons">
                          <a><div class="inst"></div></a>
                          <a><div class="ytb"></div></a>
                          <a><div class="vk"></div></a>
                      </div>
                  </div>
                  <div class="suggestion">
                      <div class="suggestion_text">
                          Есть идеи что улучшить?<br>
                          Не знаешь, с кем решить проблему?
                      </div>
                      <button class="suggest" type="button">Написать</button>
                  </div>
              </div>
          </footer>
      </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      currentTab: 'everything',
      isShowModal: false,
      acc: [
        {
          id: 8,
          title: 'Классная кружка',
          price: 2000,
          isNew: true,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 9,
          title: 'Классная игрушка',
          price: 5000,
          isNew: true,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/horsetoy.png'),
          details: 'Игрушка для детей',
          material: false,
        },
        {
          id: 10,
          title: 'Классная кружка',
          price: 2500,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 11,
          title: 'Классная кружка',
          price: 2200,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 12,
          title: 'Классная кружка',
          price: 1900,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 13,
          title: 'Классная кружка',
          price: 3000,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 14,
          title: 'Классная кружка',
          price: 4500,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
        {
          id: 15,
          title: 'Классная кружка',
          price: 999,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/bottle.jpg'),
          details: 'Бутылка для воды струбочкой',
          material: false,
        },
      ],
      clothes:
      [
        {
          id: 0,
          title: 'Классная футболка',
          price: 333,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: 'true',
        },
        {
          id: 1,
          title: 'Классное худи',
          price: 666,
          isNew: true,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/hood.jpg'),
          details: 'Брендированная толстовка от Qazaq Republic. Материал: Хлопок 80%, Вискоза 20%',
          material: true,
        },
        {
          id: 2,
          title: 'Классная красная футболка',
          price: 206,
          isNew: true,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/redshirt.png'),
          details: 'Удобная красная футболка для дома',
          material: true,
        },
        {
          id: 3,
          title: 'Классная футболка',
          price: 218,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: true,
        },
        {
          id: 4,
          title: 'Классная футболка',
          price: 3433,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: true,
        },
        {
          id: 5,
          title: 'Классная футболка',
          price: 6636,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: true,
        },
        {
          id: 6,
          title: 'Классная футболка',
          price: 2026,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: true,
        },
        {
          id: 7,
          title: 'Классная футболка',
          price: 2181,
          isNew: false,
          // eslint-disable-next-line global-require,import/no-dynamic-require,import/extensions
          img: require('../assets/tshirt.jpg'),
          details: 'Брендированная футболка от Qazaq Republic. Материал хлопок...',
          material: true,
        },
      ],
    };
  },

  computed: {
    filtered() {
      const sortByNew = (a, b) => {
        if (a.isNew && b.isNew) {
          return 0;
        }

        if (b.isNew) {
          return 1;
        }

        return -1;
      };

      if (this.currentTab === 'everything') {
        const arr = this.acc.concat(this.clothes);
        arr.sort(sortByNew);
        return arr;
      }
      const arr = [...this[this.currentTab]];
      arr.sort(sortByNew);
      return arr;
    },
  },

  methods: {
    closeModal() {
      this.isShowModal = false;
    },
    showModal() {
      this.isShowModal = true;
    },
    onChange(event) {
      this.currentTab = event.target.value;
    },
  },
};
</script>

<style>
@import '../styles/style.css';
</style>
