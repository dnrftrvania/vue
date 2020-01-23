<!-- <template>
    <div>
        <div class="container">
            <form v-on:submit.prevent="Login">
                <b-form-group
                id="lbl_email"
                label="email"
                label-for="input_email"
                >
                <b-form-input id="input_email" v-model="email" trim></b-form-input>
                </b-form-group>

                <b-form-group
                id="lbl_password"
                label="Password"
                label-for="input_password"
                >
                <b-form-input type="password" id="input_password" v-model="password" trim></b-form-input>
                </b-form-group>

                <button
                    type="submit"
                    href="#pablo"
                    class="btn btn-primary btn-round btn-lg btn-block"
                    tabindex="4"
                    pill
                    >LOGIN
                </button>
            </form>
        </div>
    </div>
</template>
<script>
export default {
    data() {
      return {
        email: '',
        password: ''
      }
    },
    methods: {
        Login: function(){
            let email = this.email 
            let password = this.password
            this.$store.dispatch('login', { email, password })
            .then(() => this.$router.push('/'))
            .catch(err => console.log(err))
        }
    }
}
</script>
-->