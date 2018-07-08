<template>
    <div class="container">
        <div class="inner-container">
            <div class="left-container">
                <div class="left-content">
                    <div>
                        <h1>Giới thiệu về chúng tôi</h1>
                    </div>
                    <div>
                        <p>
                            Eazy Marketing ra đời với những con người đam mê và giàu kinh nghiệm nhưng cũng liên tục đổi mới trong lĩnh vực Marketing và Kinh doanh. Sứ mệnh của chúng tôi là liên tục tìm tòi và đưa ra các giải pháp nâng cao nhận thức thương hiệu và gia tăng doanh số cho các doanh nghiệp theo cách thức đơn giản nhưng hiệu quả cao.
                        </p>
                        <p>Chúng tôi tập trung tư vấn chuyên sâu cho từng doanh nghiệp, đưa ra giải pháp PR, truyền thông và quảng cáo để truyền tải thông điệp của bạn đến đúng đối tượng mục tiêu.</p>
                        <h2><strong>ĐỘI NGŨ NÒNG CỐT&nbsp;</strong></h2>
                        <div class="member-info-list">
                            <ProfileItemList/>
                        </div>
                        
                    </div>
                </div>
            </div>
            <div class="right-container">2ddddddddddddddddddssssssssss</div>
        </div>
    </div>
</template>

<script>
import ProfileItemList from '~/components/Profile/ProfileItemList.vue';
export default {
    components: {
        ProfileItemList,
    }
}
</script>

<style scoped>
h1 {
    font-size: 28px;
}

h2 {
    text-align: center;
    font-size: 42px;
}

p {
    margin-bottom: 1.6em;
}

.container {
    display: flex;
    flex-direction: row;
    justify-content:center;
    align-items: center;
    align-content: center;
    background: #F5F5F5;
    height: auto;
    width: auto;
    max-width: 100%;
    max-height: 100%;
    margin: 0px;
}

.inner-container {
    display: flex;
    flex-direction: row;
    justify-content:center;
    align-items: flex-start;
    align-content: center;
    margin: 75px 75px 75px;
    
}

.left-container{
    display: flex;
    max-width: 65%;
    max-height: 100%;
    background: #fff;
}


.right-container{
    display: flex;
    max-width: 35%;
    max-height: 100%;
    background: #fff;
}

.left-content {
    display: flex;
    flex-direction: column;
    margin: 0;
    padding: 80px;
    margin: 10px 30px 10px;
}

.member-info-list {
    display:flex;
    flex-wrap:wrap;
    flex-direction:row;
    justify-content:flex-start;
    align-items:stretch;
    flex: 2;
    padding: 8px 5px 8px;
}

</style>
