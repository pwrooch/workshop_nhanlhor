<template>
    <div class="mb-4">
        <b-card no-body class="overflow-hidden" >
            <b-row no-gutters>
                <b-col md="6">
                    <b-card-img :src=image alt="Image"
                        class="rounded-0"></b-card-img>
                </b-col>
                <b-col md="6">
                    <b-card-body :title=title>
                        <b-card-text>
                            {{ description }}
                        </b-card-text>
                        <b-card-text>
                            {{ date }}
                        </b-card-text>
                        <b-button href="" variant="outline-success">รายละเอียด</b-button>
                    </b-card-body>
                </b-col>
            </b-row>
        </b-card>
    </div>
</template>


<script>
export default {
    props: {
        title: {
            type: String,
            required: true
        }, 
        description: {
            type: String,
            required: true
        },
        image: {
            type: String,
            required: true
        },
        date: {
            type:String,
            required:true
        }
    }
}



</script>