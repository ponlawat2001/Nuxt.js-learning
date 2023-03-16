<template>
    <div class="dropdown">
        <button class="dropdown-toggle" @click="show = !show">
            {{ label }}
            <span class="arrow">▼</span>
        </button>
        <ul class="dropdown-menu" v-show="show">
            <li v-for="item in items" @click="selectItem(item)">
                {{ item.text }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    props: {
        label: {
            type: String,
            required: true
        },
        items: {
            type: Array,
            required: true
        }
    },
    data() {
        return {
            show: false
        }
    },
    methods: {
        selectItem(item) {
            this.$emit("selected", item)
            this.show = false
        }
    }
}
</script>

<style>
.dropdown {
    position: relative;
    display: inline-block;
}

.dropdown-toggle {
    cursor: pointer;
    background-color: white;
    border: 1px solid #ddd;
    border-radius: 4px;
    padding: 8px 20px;
}

.dropdown-menu {
    position: absolute;
    top: 100%;
    left: 0;
    z-index: 1000;
    display: none;
    float: left;
    min-width: 160px;
    padding: 5px 0;
    margin: 2px 0 0;
    list-style: none;
    background-color: #fff;
    background-clip: padding-box;
    border: 1px solid #ccc;
    border: 1px solid rgba(0, 0, 0, .15);
    border-radius: 4px;
    box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
}

.dropdown-menu.show {
    display: block;
}

.arrow {
    display: inline-block;
    margin-left: 5px;
    font-size: 12px;
}
</style>
