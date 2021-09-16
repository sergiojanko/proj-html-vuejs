<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
                <i :class="icon"></i>
                <h5 class="card-title">{{title}}</h5>
                <p class="card-text">{{text}}</p>
        </div>
    </div>
</template>

<script>
export default {
name: "Card",
props: ["title","text","icon"]
}
</script>

<style>

</style>