<script>
    export default {
        props: [
            'friendName',
            'href',
            'desc',
            'logoHref'
        ]
    }
</script>

<template>
    <a class="shadow-lg w-auto h-auto flex backdrop-blur-md border-2 border-slate-800 rounded-md hover:shadow-md cstm-font-bmo" :href="href">
        <div class="w-1/3 ml-2">
             <img :src="logoHref" width="64" height="64">
        </div>
        <div class="items-center w-2/3 h-auto mt-1">
            {{ friendName }}
            <div class="mt-1">
                {{ desc }}
            </div>
        </div>
        
    </a>
</template>