<template>
    <h1>single slot</h1>
    <slot></slot>
    <h2>multiple slot with name</h2>
    <header>
    <slot name="header"></slot>
    </header>
</template>

<script>
export default{
    name:'ChildSlot',
    props:{
        data:String,
    }
}
</script>