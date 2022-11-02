<template>
    <div class="row g-0">
        <div class="col-2 offset-1 text-start">
            <Navigation />
        </div>
        <div class="col-8 text-start">
            <div class="mt-3 btnTitle" :style="[btnStyle, btnSet, btnBoxShadow]">
                <span v-html="iconPosition1" />
                Button
                <span v-html="iconPosition2" />
            </div>
            <ButtonDefault @btnStyle1="btnDefault"/>
            <ButtonOutline @btnStyle2="btnOutline"/>
            <ButtonText @btnStyle3="btnText"/>
            <ButtonDisableShadow @btnStyle4="btnDisableShadow"/>
            <ButtonDisabled @btnStyle5="btnDisabled" @btnStyle6="btnDisabledText"/>
            <ButtonIcon @icon1="iconLeft(); increment()" @icon2="iconRight(); increment()"/>
            <ButtonSize @btnStyle9="btnSm" @btnStyle10="btnMd" @btnStyle11="btnLg"/>
            <ButtonColor @btnStyle12="btnDefault" @btnStyle13="btnPrimary" @btnStyle14="btnSecondary" @btnStyle15="btnDanger"/>

            <br><br>
            <div class="iconSource mt-5">Icons: <a href="https://fontawesome.com/icons/cart-plus?s=solid&f=classic">https://fontawesome.com/icons/cart-plus?s=solid&f=classic</a></div>
            <div class="createdBy mt-5 mb-5">created by <a href="https://github.com/hasanaimroatun/wpu-buttonComponentChallenge">hasanaimroatun</a> - devChallenges.io</div>
        </div>
    </div>
</template>

<script>
    import ButtonDefault from './ButtonDefault.vue'
    import ButtonOutline from './ButtonOutline.vue'
    import ButtonText from './ButtonText.vue'
    import ButtonDisableShadow from './ButtonDisableShadow.vue'
    import ButtonDisabled from './ButtonDisabled.vue'
    import ButtonIcon from './ButtonIcon.vue'
    import ButtonSize from './ButtonSize.vue'
    import ButtonColor from './ButtonColor.vue'
    import Navigation from './Navigation.vue'

    export default {
        name: 'Button-component',
        components: {
            Navigation,
            ButtonDefault,
            ButtonOutline,
            ButtonText,
            ButtonDisableShadow,
            ButtonDisabled,
            ButtonIcon,
            ButtonSize,
            ButtonColor
        },
        data() {
            const btnIcons = ['<i class="fa-solid fa-paper-plane"/>', '<i class="fa-solid fa-trash"/>', '<i class="fa-solid fa-thumbs-up"/>', '<i class="fa-solid fa-upload"/>', '<i class="fa-solid fa-download"/>']
            return {  
                btnStyle: {
                    border: '1px solid white',
                    marginLeft: '-25px',
                },
                btnSet: {
                    width: '130px',
                    padding: '7px',
                    borderRadius: '6px',
                    textAlign: 'center',
                },
                btnBoxShadow: {},
                btnIcons,
                iconPosition1: ' ',
                iconPosition2: ' ',
                num: 0
            };
        },
        methods: {
            btnDefault() {
                this.btnStyle = {
                    backgroundColor: '#E0E0E0',
                    border: '1px solid #E0E0E0'
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            btnOutline() {
                this.btnStyle = {
                    color: '#3D5AFE',
                    border: '1px solid #3D5AFE',
                    boxShadow: '1px 1px 5px grey'
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            btnText() {
                this.btnStyle = {
                    color: '#3D5AFE',
                    border: '1px solid white'
                }
                this.btnBoxShadow = {
                    boxShadow: 'none'
                }
            },
            btnDisableShadow() {
                this.btnBoxShadow = {
                    boxShadow: 'none'
                }
            },
            btnDisabled() {
                this.btnStyle = {
                    backgroundColor: '#E0E0E0',
                    color: '#9E9E9E',
                    border: '1px solid #E0E0E0',
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            btnDisabledText() {
                this.btnStyle = {
                    color: '#9E9E9E',
                    border: '1px solid white'
                },
                this.btnBoxShadow = {
                    boxShadow: 'none'
                }
            },
            btnSm() {
                this.btnSet = {
                    width: '93px',
                    fontSize: '14px',
                    borderRadius: '6px',
                    textAlign:'center',
                    paddingLeft: '8px',
                    paddingRight: '8px'
                }
            },
            btnMd() {
                this.btnSet = {
                    width: '101px',
                    fontSize: '16px',
                    borderRadius: '6px',
                    textAlign:'center',
                    padding: '2px 8px 2px'
                }
            },
            btnLg() {
                this.btnSet = {
                    width: '113px',
                    fontSize: '18px',
                    borderRadius: '6px',
                    textAlign:'center',
                    padding: '4px 8px 4px'
                }
            },
            btnPrimary() {
                this.btnStyle = {
                    backgroundColor: '#2962FF',
                    border: '1px solid #2962FF',
                    color: 'white',
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            btnSecondary() {
                this.btnStyle = {
                    backgroundColor: '#455A64',
                    border: '1px solid #455A64',
                    color: 'white'
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            btnDanger() {
                this.btnStyle = {
                    backgroundColor: '#D32F2F',
                    border: '1px solid #D32F2F',
                    color: 'white'
                },
                this.btnBoxShadow = {
                    boxShadow: '1px 1px 5px grey'
                }
            },
            iconLeft() {
                this.iconPosition1 = this.btnIcons[this.num],
                this.iconPosition2 = ''
            },
            iconRight() {
                this.iconPosition1 = '',
                this.iconPosition2 = this.btnIcons[this.num]
            },
            increment() {
                this.num === 4? this.num = this.num - 4: this.num = this.num + 1
            }
        }
    }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500;700&family=Noto+Sans:wght@500;700&family=Poppins:wght@500;600&family=Ubuntu+Mono&display=swap');

.btnTitle {
    font-family: 'Poppins', sans-serif;
    font-weight: 500;
    font-size: 24px;
    line-height: 36px;
    color: #4F4F4F;
}

.label {
    font-family: 'Ubuntu Mono', monospace;
    font-weight: 400;
    font-size: 12px;
    line-height: 12px;
    color: #000000;
    margin-bottom: 12px;
}

button {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 500;
}

.iconSource {
    font-family:  'Ubuntu Mono', monospace;
    font-weight: 400;
    font-size: 12px;
    line-height: 12px;
    color: #828282;
}

.createdBy {
    font-family: 'Montserrat', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 17.07px;
    color: #A9A9A9;
}

.iconSource a,
.createdBy a {
    color: inherit;
    text-decoration: none;
}

.createdBy a {
    font-weight: 700;
}

.iconSource a:hover,
.createdBy a:hover {
    color: #4F4F4F;
}

@media screen and (max-width:768px) {
    .label,
    .iconSource,
    .createdBy {
        padding-left: 45px;
    }

    .btnTitle {
        position: relative;
        left: 45px;
    }
}
</style>