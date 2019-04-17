<template>
    <div class="alert alert-info alert-dismissible fade show" v-if="!hidden">
        [Built using Vue] - Use this space to summarize your privacy and cookie use policy.
        <a
            :href="privacyLink"
        >Learn More</a>.
        <button type="button" class="accept-policy close" @click="setCookie">
            <span aria-hidden="true">Accept</span>
        </button>
    </div>
</template>

<script>
export default {
    props: ["privacyLink", "cookieString"],
    data() {
        return {
            hidden: false
        };
    },
    methods: {
        setCookie() {
            document.cookie = this.cookieString;
            this.hidden = true;
        }
    }
};
</script>