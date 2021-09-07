<template>
    <div>
        <v-divider></v-divider>
        <v-subheader class=".text-primary fs-2">{{ title }}</v-subheader>
        <v-divider></v-divider>
    </div>
</template>

<script>
export default {
    name: "SectionTitle",
    props: ["title"],
};
</script>
