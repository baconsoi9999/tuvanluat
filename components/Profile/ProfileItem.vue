<template>
    <div class="wrapper">
        <li>
            <a href="#">
                <div class="img-wrap">
                    <div class="member-image">
                        <img class="round-image" :src="imageurl" :alt="name">
                    </div>
                    <div class="member-info">
                        <div class="member-name">{{name}}</div>
                        <div class="member-role">{{role}}</div>
                    </div>
                </div>
            </a>
        </li>
    </div>
</template>

<script>
export default {
    props: [
        'name',
        'role',
        'imageurl'
    ],
}
</script>

<style scoped>
li {
  list-style-type: none;
}

.wrapper{
    padding: 20px 20px 20px 20px;
}

.img-wrap {
    width: 294px;
    height: 294px;
    top: 0px;
    left: 0px;
    position: relative;
}

.member-image {
    position: absolute;
}

.member-info {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    right: auto;
    left: 0;
    text-align: left;
    position: absolute;
    bottom: 0;
    float:left;
}

.member-name {
    line-height: 1;
    font-weight: 400;
    padding: 8px 15px;
    background: #ffc000;
    font-size: 18px;
    color: #fff;
    float: left;
}

.member-role {
    float: left;
    font-weight: 300;
    text-align: center;
    letter-spacing: 0.01em;
    background: #556270;
    font-size: 14px;
    color: #fff;
    padding: 5px;
    margin: 2px;
}

.round-image {
    border-radius: 50%;
}
</style>
