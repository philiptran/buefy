<template>
    <div>
        <h1 class="title is-spaced">Select</h1>
        <h2 class="subtitle">
            Select an item in a dropdown list.
            Use with <strong><router-link to="/documentation/field">Field</router-link></strong> to access all functionalities
        </h2>
        <hr>

        <Example :component="ExSimple" :code="ExSimpleCode" vertical/>

        <Example :component="ExMultiple" :code="ExMultipleCode" title="Multiple" vertical/>

        <Example :component="ExIcons" :code="ExIconsCode" title="Icons" vertical/>

        <Example :component="ExSizes" :code="ExSizesCode" title="Sizes" vertical/>

        <ApiView :data="api"/>
    </div>
</template>

<script>
    import api from './api/select'

    import ExSimple from './examples/ExSimple'
    import ExSimpleCode from '!!raw-loader!./examples/ExSimple'

    import ExMultiple from './examples/ExMultiple'
    import ExMultipleCode from '!!raw-loader!./examples/ExMultiple'

    import ExIcons from './examples/ExIcons'
    import ExIconsCode from '!!raw-loader!./examples/ExIcons'

    import ExSizes from './examples/ExSizes'
    import ExSizesCode from '!!raw-loader!./examples/ExSizes'

    export default {
        data() {
            return {
                api,
                ExSimple,
                ExMultiple,
                ExIcons,
                ExSizes,
                ExSimpleCode,
                ExMultipleCode,
                ExIconsCode,
                ExSizesCode
            }
        }
    }
</script>
