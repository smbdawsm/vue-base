<template>
    <li> {{ obj.title }} </li>
</template>

<script>
export default {
    props: {
        obj : {
            type: Object,
            required: true
        }
    }
}
</script>