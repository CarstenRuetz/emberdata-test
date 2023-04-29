<template>Test {{ test }}</template>

<script setup>
import Store from "@ember-data/store";
import Cache from "@ember-data/json-api";

class EmberStore extends Store {
    createCache(storeWrapper) {
        return new Cache(storeWrapper);
    }
}

const test = "123";
</script>
