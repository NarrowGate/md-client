<template>
    <section class="container">
        <form action="" class="contactForm">
            <div class="columns">
                
                <div class="column is-4">                    
                    <div class="field">
                        <label for="" class="label has-text-left">Name</label>
                        <div class="control">
                            <input type="text" class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Email</label>
                        <div class="control">
                            <input type="email" class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Phone</label>
                        <div class="control">
                            <input type="number" class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Suburb</label>
                        <div class="control">
                            <input type="text" class="input">
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Subject</label>
                        <div class="control">
                            <div class="select" style="width: 100%">
                                <select name="" id="">
                                    <option value="">General Enquiry</option>
                                    <option value="">Driving Lessons</option>
                                    <option value="">Lesson and Test</option>
                                </select>
                            </div>                            
                        </div>
                    </div>
                    <div class="field">
                        <label for="" class="label has-text-left">Enquiry</label>
                        <div class="control">                        
                            <textarea class="textarea" placeholder="10 lines of textarea" rows="10"></textarea>
                        </div>
                    </div>
                    <div class="field">
                        <div class="control">
                            <button class="button is-primary">Submit</button>
                        </div>
                    </div>
                </div>
                <div class="column is-4"></div>
            </div>
        </form>
    </section>
</template>

<style>
.contactForm {
    background: white;
    padding: 1rem;
}
</style>

