<template>
    <div class="justify-content-center md-toolbar md-primary mb-5">
        <div class="col-8 my-5">
            <button id="NavButtons" @click="go('CreateQuestion')" type="button" class="md-button md-raised mx-1">
                <div class="md-ripple">
                    <div class="md-button-content">Create A Question</div>
                </div>
            </button>
            <button id="NavButtons" @click="go('CreateQuizView')" type="button" class="md-button md-raised mx-1">
                <div class="md-ripple">
                    <div class="md-button-content">Create A Quiz</div>
                </div>
            </button>
            <button id="NavButtons" @click="go('SelectQuiz')" type="button" class="md-button md-raised mx-1">
                <div class="md-ripple">
                    <div class="md-button-content">Select A Quiz</div>
                </div>
            </button>
        </div>
    </div>

</template>

<script>
    import router from "../router.js";
    export default {
        name: "NavButtons",
        methods: {
            go(pageName) {
                router.push({ name: pageName });
            }
        }
    };
</script>
<style scoped>
    #NavButtons {
        background-color: #ffffe8 !important;
        color: #9c27b0 !important;
        font-weight: 700;

    }
</style>