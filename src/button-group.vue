<template>
    <div class="m-button-group">
        <slot></slot>
    </div>
</template>
<script></script>
<style lang="scss">
    .m-button-group {
        display: inline-flex;
        vertical-align: middle;
        > .m-button {
            border-radius: 0;
            &:not(:first-child) {
                margin-left: -1px;
            }
            &:first-child {
                border-top-left-radius: var(--border-radius);
                border-bottom-left-radius: var(--border-radius);
            }
            &:last-child {
                border-top-right-radius: var(--border-radius);
                border-bottom-right-radius: var(--border-radius);
            }
            &:hover {
                position: relative;
                z-index: 1;
            }
        }
    }
</style>
