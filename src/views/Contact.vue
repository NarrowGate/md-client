<template>
    <section class="container">
        <form v-on:submit.prevent class="contactForm">
            <div class="columns">
                
                <div class="column is-4">                    
                    <div class="field">
                        <label for="" class="label has-text-left">Name</label>
                        <div class="control">
                            <input type="text" v-model='name' class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Email</label>
                        <div class="control">
                            <input type="email" v-model='email' class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Phone</label>
                        <div class="control">
                            <input type="number"  v-model='phone' class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Suburb</label>
                        <div class="control">
                            <input type="text"  v-model='suburb' class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Subject</label>
                        <div class="control">
                            <div class="select" style="width: 100%">
                                <select name=""  v-model='subject'>
                                    <option disabled value="">Please Select One</option>
                                    <option value="General Enquiry">General Enquiry</option>
                                    <option value="Driving Lessons">Driving Lessons</option>
                                    <option value="Lesson and Test">Lesson and Test</option>
                                </select>
                            </div>                            
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Enquiry</label>
                        <div class="control">                        
                            <textarea class="textarea"  v-model='enquiry' placeholder="10 lines of textarea" rows="10"></textarea>
                        </div>
                    </div>
                    <div class="field">
                        <div class="control">
                            <button @click.prevent = "submitContact" class="button is-primary">Submit</button>
                        </div>
                    </div>
                </div>
                <div class="column is-4"></div>
            </div>
        </form>
    </section>
</template>
<script>
import axios from 'axios'
export default {

    data () {
        return {
            name : '',
            email: '',
            phone: '',
            suburb: '',
            subject: '',
            enquiry: ''
        }
    },

    methods: {
        submitContact () {

            var contactData = {
                name : this.name,
                email : this.email,
                phone : this.phone,
                suburb : this.suburb,
                subject : this.subject,
                enquiry : this.enquiry
            }

            // console.log(contactData)

            axios.post('/process-contact', contactData)
            .then((res) => {
                //console.log(res)
            })
            .catch((err) => {
                //console.log(err)
            });
        }
    }
}
</script>
<style>
.contactForm {
    background: white;
    padding: 1rem;
}
</style>
