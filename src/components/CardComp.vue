<script lang="ts" setup>
import { defineProps } from 'vue'
defineProps<{
    subTitle?: string,
    descPar?: string,
    btnClass: string
}>()
</script>

<template>
    <div class="card-component">
        <div class="card-header">
            <button :class="btnClass">
                <slot name="button-slot"></slot>
            </button>
            <div class="card-header-right">
                <h4 class="sub-title">{{ subTitle }}</h4>
                <p class="desc-par">{{ descPar }}</p>
            </div>
        </div>
        <div class="card-bottom">
            <slot name="card-bottom"></slot>
        </div>
    </div>
</template>

<style scoped>
.card-component {
    background: var(--black-700);
    border-radius: 8px;
    padding: 12px;
    height: 100%;
}

.card-header {
    display: flex;
    align-items: flex-start;
    gap: 10px;
    margin-bottom: 20px;
}

.card-header button {
    width: 32px;
    height: 32px;
    border-radius: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    background: none;
    cursor: pointer;
    background: #262626;
    border: none;
}

.card-header-right {
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding-top: 4px;
}

.card-bottom {
    margin-left: 42px;
}
</style>