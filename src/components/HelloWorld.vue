<template>
<div class="hello">
  <template>
    <section>
        <b-field>
            <b-button
                label="Launch loading"
                type="is-primary"
                size="ismedium"
                @click="openLoading" />
        </b-field>
        <b-field>
            <b-switch type="is-info" v-model="isFullPage">Display loader over full page</b-switch>
        </b-field>
        <b-notification :closable="false">
            Discipline is what we require to drive our mission instead of motivation
            <b-loading :is-full-page="isFullPage" v-model="isLoading" :can-cancel="true"></b-loading>
        </b-notification>
    </section>
</template>

</div>
</template>

<script>
export default {
    name: 'HelloWorld',
    data() {
            return {
                isLoading: false,
                isFullPage: true
            }
        },
        methods: {
            openLoading() {
                this.isLoading = true
                setTimeout(() => {
                    this.isLoading = false
                }, 10 * 1000)
            }
        }

}
</script>

<style>
.hello{
    text-align: center;
}
</style>
