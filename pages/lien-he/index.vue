<template>
    <div class="wrapper-column">
        <div class="map-container two-half-column">
            <googleMapComponent name="example"/>
        </div>

        <div class="wrapper-row centralize two-half-column contact-section">
            <div class="input-field-container two-half-row">
                <div class="wrapper-column input-field-inner">
                    <div>
                        <div>
                            <label for="name"><strong>Họ và Tên <strong style="color:red">*</strong></strong></label>
                        </div>
                        <div>
                            <input type="text" v-model="name" required >
                        </div>
                        <div>
                            <div class="invalid-feedback" style="color:red" v-if="name === ''">This field is required.</div>
                        </div>
                    </div>

                    <div>
                        <div>
                            <label for="email"><strong>Email <strong style="color:red">*</strong></strong></label>
                        </div>
                        <div>
                            <input type="text" v-model="email" required>
                        </div>
                        <div>
                            <div class="invalid-feedback" style="color:red" v-if="email === ''">This field is required.</div>
                        </div>
                    </div>

                    <div>
                        <div>
                            <label for="phone"><strong>Số điện thoại <strong style="color:red">*</strong></strong></label>
                        </div>
                        <div>
                            <input type="text" v-model="phone" required>
                        </div>
                        <div>
                            <div class="invalid-feedback" style="color:red" v-if="phone === ''">This field is required.</div>
                        </div>
                    </div>

                    <div>
                        <div>
                            <label for="message"><strong>Thông điệp <strong style="color:red">*</strong></strong></label>
                        </div>
                        <div>
                            <textarea name="" id="" cols="30" rows="10" v-model="message" required/>
                        </div>
                        <div>
                            <div class="invalid-feedback" style="color:red" v-if="message === ''">This field is required.</div>
                        </div>
                    </div>

                    <div class="submit-container">
	                    <button class="button submit-button" type="submit" title="submit" v-on:click="onSubmit()">
                            <span><span>Gửi đi</span></span>
                        </button>
                        <div>
                            <div class="invalid-feedback" style="color:red" v-if="checkSubmitError">Hãy sửa lỗi trước khi gửi mẫu này.</div>
                        </div>
                    </div>

                </div>
            </div>
            <div class="two-half-row">
                <div>
                    <h1 class="contact-title">THÔNG TIN LIÊN HỆ</h1>
                    <p><b>Trụ sở chính:</b> 11B-C5 Nguyễn Bỉnh Khiêm, Phường Bến Nghé, Quận 1, TP.Hồ Chí Minh</p>
                    <p><b>Điện thoại:</b> 08-7302 2888 – Hotline: 0907 617 916</p>
                    <p><b>Email:</b> hi@eazymarketing.net</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import googleMapComponent from '~/components/GoogleMap/googleMap.vue';

export default {
    components: {
        googleMapComponent,
    },
    data() {
        return {
            name: '',
            email: '',
            phone: '',
            message: '',
            attemptSubmit: false,
        }
    },
    computed: {
        checkSubmitError() {
            if (this.name == '' || this.email == '' || this.phone == '' || this.message == '')
                return true;
            return false; 
        }
    },
    methods: {
        onSubmit(){
            
        }
    }
}
</script>

<style scoped>
h1 {
    font-size: 28px;
}

button {
    border-radius: 2px;
    padding: 15px 0px 35px;
}

input {
    margin: 0;
    height: auto;
    padding: .75em;
    width: 100%;
    cursor: text;
    line-height: 1;
    
}

textarea {
    margin: 0;
    height: auto;
    padding: .75em;
    width: 100%;
    cursor: text;
    line-height: 1;
}

.wrapper-column {
    display: flex;
    flex-direction: column;

}

.wrapper-row {
    display: flex;
    flex-direction: row;
}

.centralize {
    justify-content: space-around;
    align-items: flex-start;
    align-content: center;

}

.contact-section{
    padding: 2% 13% 2%;
}

.map-container {
    width: 100%;
    height: 50%;
}

.two-half-column{
    width: 100%;
    height: 50%;
}

.two-half-row {
    width: 50%;
    height: 100%;
}

.input-field-container {
    padding-left: 0px;
    padding-right: 0px;
}

.input-field-inner {
    box-sizing: border-box;
    padding-left: 15px;
    padding-right: 15px;
    width: 90%;
}

.submit-button {
    width: 30%;
    color: #fff;
    background: #ffc000;
    float: right;
}

.submit-container {
    display: flex;
    flex-direction: column;
    align-items: flex-end;
}





</style>
