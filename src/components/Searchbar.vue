<template>
    <form class="d-flex" >
        <input class="form-control" type="text" placeholder="Search characters" v-model="searchText">
        <button type="submit" class="btn btn-primary mx-3" @click.prevent="$emit('search', searchText)">Search</button>
        <button class="btn btn-warning" @click.prevent="resetSearch">Reset</button>
    </form>
</template>

<script>
export default {
    name: "Searchbar",
    data() {
        return {
            searchText: ""
        }
    },
    methods: {
        resetSearch() {
            this.searchText = "";
            this.$emit('search', this.searchText);
        }
    }
}
</script>