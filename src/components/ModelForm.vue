<template>
    <div class="con">
        <section class="form-register">
            <h4>Formulario Registro</h4>
                <input class="controls" type="text" name="nombres" id="nombres" placeholder="Ingrese su nombre" v-model="inputNombre">
                <input class="controls" type="text" name="apellidos" id="apellidos" placeholder="Ingrese su apellido" v-model="inputApellido">
                <input class="controls" type="email" name="correo" id="correo" placeholder="Ingrese su correo" v-model="inputcorreo">
                <input class="controls" type="password" name="password" id="password" placeholder="Ingrese su contraseña" v-model="inputcontraseña">

                <label>Selecciona tu pais en el cuadro:</label>
                <select class="controls" type="text" name="select" id="select" placeholder="Ingresa tu pais" v-model="country">   
                    
                    <option value="Chile">Chile</option>
                    <option value="Argentina">Argentina</option>
                    <option value="Peru">Peru</option>
                    <option value="Brazil">Brazil</option>

                </select>

                <p>Estoy de acuerdo con <a href="">Terminos y condiciones </a></p>
                <input class="botons" type="submit" value="Registrar">
                <p><a href="">¿Ya tengo cuenta?</a></p>
        </section>
    </div>

    <div class="form-result">                                          
        <h3>{{ inputNombre }}</h3>
        <h3>{{ inputApellido }}</h3>
        <h3>{{ inputcorreo }}</h3>
        <h3>{{ inputcontraseña }}</h3>
        <h3>{{ country }}</h3>

    </div>

</template>

<script setup>
    import { ref } from 'vue'

    let inputNombre = ref('')
    let inputApellido = ref('')
    let inputcorreo = ref('')
    let inputcontraseña = ref('')
    let country = ref('Chile')
</script>


<style scoped>



*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.form-register{
    width: 400px;
    background: #24303c;
    padding: 30px;
    margin: auto;
    margin-top: 100px;
    border-radius: 4px;
    font-family: 'calibri';
    color: white;
    box-shadow: 7px 13px 37px #000 ;
}

.form-register h4{
    font-size: 22px;
    margin-bottom: 20px;
}

.controls{
    width: 100%;
    background: #24303c;
    padding: 10px;
    border-radius: 4px;
    margin-bottom: 16px;
    border: 1px solid #1f53c5 ;
    font-family: 'calibri';
    font-size: 18px;
    color: white;
}

.form-register p{
    height: 40px;
    text-align: center;
    font-size: 18px;
    line-height: 40px;

}

.form-register a:hover{
    color: white;
    text-decoration: underline;
}
.form-register .botons{
    width: 100%;
    background: green;
    border: none;
    padding: 12px;
    color: white;
    margin: 16px 0;
    font-size: 16px;
    align-items: center;
}

.form-result{
    width: 400px;
    background: #24303c;
    padding: 30px;
    margin: auto;
    margin-top: 100px;
    border-radius: 4px;
    font-family: 'calibri';
    color: white;
    box-shadow: 7px 13px 37px #000 ;
}
.form-result h3{
    font-family: 'calibri';
}
</style>