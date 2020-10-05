<template>
    <li> <a style="color: white" href="/object">{{ obj.title }} </a>  </li>
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