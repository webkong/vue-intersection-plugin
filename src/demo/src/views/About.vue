<template>
  <div class="md-example-child md-example-child-result-page md-example-child-result-page-2">
    <md-result-page
            :buttons="buttons">
    </md-result-page>
  </div>
</template>

<script>
import Toast from "mand-mobile";
export default {
    name: 'result-page-demo',
    data() {
        return {
            buttons: [
                {
                    text: '普通按钮',
                    handler() {
                        Toast.succeed('普通操作')
                    },
                },
                {
                    text: '高亮按钮',
                    type: 'ghost-primary',
                    handler() {
                        Toast.succeed('不普通操作')
                    },
                },
            ],
        }
    },
}

</script>

<style>
  .md-result-page.customized img{
    height: 131px;
  }
</style>