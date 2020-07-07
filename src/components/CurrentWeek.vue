<template>
    <div class="current_week_container">
        {{ date.locale("cs").format("D. M.") }} -
        {{ date.clone().locale("cs").add(6, "days").format("D. M. Y") }}
    </div>
</template>

<script>
import moment from "moment"
export default {
    name: "CurrentWeek",
    props: {
        date: moment,
    },
}
</script>

<style>
.current_week_container {
    width: 90%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 15px;
    color: white;
    text-align: center;
    font-weight: bold;
    font-size: 14px;
}
</style>
