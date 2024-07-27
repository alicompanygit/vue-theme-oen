<template>
    <div>
        <table class="w-100">
            <thead>
                <tr class="bg-thed">
                    <th class="text-center align-middle p-1" v-for="item in head" v-html="item" scope="col"></th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="item, index in body"
                    :class="['mt-4', item.change > 0 ? 'bg-green' : '', item.change < 0 ? 'bg-red' : '']">
                    <th scope="row" class="text-center align-middle p-1">
                        <img src="../assets/icon/star.svg" alt="">
                        {{ index + 1 }}
                    </th>
                    <td class="text-center align-middle p-1">
                        <img src="../assets/icon/bitcoin.png" alt="">
                        {{ item.name }}
                    </td>
                    <td class="text-center align-middle p-1" v-html="'$' + item.price"></td>
                    <td class="text-center align-middle p-1" v-html="item.change + '%'"></td>
                    <td class="text-center align-middle p-1" v-html="'$' + item.market"></td>
                    <td class="text-center align-middle p-1">
                        <img v-if="item.change > 0" src="../assets/imgs/greenCandle.png" alt="">
                        <img v-else-if="item.change < 0" src="../assets/imgs/redCandle.png" alt="">
                        <img v-else src="../assets/imgs/yellowCandel.png" alt="">
                    </td>
                    <td class="align-middle text-end pe-2">
                        <button type="button" class="btn btn-outline-light rounded-pill px-4 py-6">Trade</button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>
<script setup>
import { ref, defineProps, onMounted } from 'vue';
const props = defineProps({
    body: {
        typeof: Object,
        default: [{ nemeSrc: '', name: 'lorem', price: 0, change: 0, market: 0 }]
    },
    head: {
        typeof: Array,
        default: ['#', 'Name', 'price', 'change', 'market Cap', 'chart', '']
    },
});
onMounted(() => {

})
</script>
<style lang="scss">
table,
th,
td {
    border-collapse: separate;
    border-spacing: 0px 15px;
    border: none;
    color: #fff;
}

.py-6 {
    padding-top: 5px;
    padding-bottom: 5px;
    font-size: 17px;
}

tr {
    background: linear-gradient(90deg, rgba(255, 255, 255, 0.07) 0%, rgba(255, 215, 73, 0.2) 100%);

    &:hover {
        transform: scale(1.01);
        background: linear-gradient(90deg, rgba(255, 255, 255, 0.07) 0%, rgba(255, 216, 73, 0.329) 100%);
    }
}

.bg-green {
    background: linear-gradient(90deg, rgba(255, 255, 255, 0.0525) 0%, rgba(47, 255, 28, 0.11) 100%);

    &:hover {
        background: linear-gradient(90deg, rgba(255, 255, 255, 0.0525) 0%, rgba(47, 255, 28, 0.315) 100%);
    }
}

.bg-red {
    background: linear-gradient(90deg, rgba(255, 255, 255, 0.0525) 0%, rgba(255, 0, 0, 0.075) 100%);

    &:hover {
        background: linear-gradient(90deg, rgba(255, 255, 255, 0.0525) 0%, rgba(255, 0, 0, 0.308) 100%);
    }

}

.bg-thed {
    background: linear-gradient(270deg, rgba(134, 91, 255, 0.2) 0%, rgba(170, 103, 255, 0.2) 100%);
}

th:first-child {
    border-top-left-radius: 999px;
}

th:last-child {
    border-bottom-right-radius: 999px;
}

th:first-child {
    border-bottom-left-radius: 999px;
}

th:last-child {
    border-top-right-radius: 999px;
}

td:first-child {
    border-top-left-radius: 999px;
}

td:last-child {
    border-bottom-right-radius: 999px;
}

td:first-child {
    border-bottom-left-radius: 999px;
}

td:last-child {
    border-top-right-radius: 999px;
}
</style>