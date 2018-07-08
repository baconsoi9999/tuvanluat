<template>
    <div>
        <ul class="member-info">
            <ProfileItem
                v-for="member in members"
                :key="member.name"
                :name="member.name"
                :imageurl="member.imageurl"
                :role="member.role"
            />
        </ul>
    </div>
</template>

<script>
import ProfileItem from './ProfileItem.vue';

export default {
    components: {
        ProfileItem,
    },
    data () {
        return {
            members: [
                {
                    name: 'Đồng Thanh Tùng',
                    role: 'Creative Director',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/dong-thanh-tung.jpg'
                },
                {
                    name: 'Bình Nguyễn',
                    role: 'Content Manager',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/binh-nguyen.jpg'
                },
                {
                    name: 'Ngô Tuấn Duy',
                    role: 'Product Manager',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/ngo-tuan-duy.jpg'
                },
                {
                    name: 'Đồng Thanh Tùng',
                    role: 'Creative Director',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/dong-thanh-tung.jpg'
                },
                {
                    name: 'Bình Nguyễn',
                    role: 'Content Manager',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/binh-nguyen.jpg'
                },
                {
                    name: 'Ngô Tuấn Duy',
                    role: 'Product Manager',
                    imageurl: 'https://eazymarketing.net/wp-content/uploads/2018/06/ngo-tuan-duy.jpg'
                },

            ],
        }
    }
}
</script>

<style scoped>
ul {
    list-style-type: none;
}

.member-info {
    display:flex;
    flex-wrap:wrap;
    flex-direction:row;
    justify-content:center;
    align-items:stretch;
    flex: 1;
    padding: 0px
}

</style>
