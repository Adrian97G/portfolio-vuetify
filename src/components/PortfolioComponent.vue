<template>
    <v-container class="my-15">
        <v-row justify="center">
            <v-flex xs12 lg12 align-self-center>
                <v-subheader class="text-h4 justify-center">Portfolio</v-subheader>
                <p class="text-center">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Quidem, quaerat nobis! Earum placeat necessitatibus, provident nulla totam officiis voluptatum reprehenderit.</p>
            </v-flex>
            <v-flex xs12>
                <div class="text-center">
                    <v-chip @click="activePortfolio = 'webapp'" :color="activePortfolio === 'webapp'? 'success' : ''" class="mx-5">Web App</v-chip>
                    <v-chip @click="activePortfolio = 'mobileapp'" :color="activePortfolio === 'mobileapp'? 'success' : ''" class="mx-5">Movile App</v-chip>
                    <v-chip @click="activePortfolio = 'desktopapp'" :color="activePortfolio === 'desktopapp'? 'success' : ''" class="mx-5">Desktop App</v-chip>
                </div>
            </v-flex>
            <slot v-if="activePortfolio === 'webapp'">
                <v-col lg="3" v-for="(web,webindex) in webApps" :key="webindex">
                <v-card>
                    <v-img
                        :src="web.image"
                        class="white--text align-end"
                        gradient="to bottom, rgba(0, 0, 0, .1), rgba(0, 0, 0, .5)"
                        height="200px"
                    >
                        <v-card-title>{{web.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
            </slot>
            <slot v-if="activePortfolio === 'mobileapp'">
                <v-col lg="3" v-for="(mobile,mobileindex) in mobileApps" :key="mobileindex">
                <v-card>
                    <v-img
                        :src="mobile.image"
                        class="white--text align-end"
                        gradient="to bottom, rgba(0, 0, 0, .1), rgba(0, 0, 0, .5)"
                        height="200px"
                    >
                        <v-card-title>{{mobile.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
            </slot>
            <slot v-if="activePortfolio === 'desktopapp'">
                <v-col lg="3" v-for="(desktop,desktopindex) in desktopApps" :key="desktopindex">
                <v-card>
                    <v-img
                        :src="desktop.image"
                        class="white--text align-end"
                        gradient="to bottom, rgba(0, 0, 0, .1), rgba(0, 0, 0, .5)"
                        height="200px"
                    >
                        <v-card-title>{{desktop.title}}</v-card-title>
                    </v-img>
                </v-card>
            </v-col>
            </slot>
        </v-row>
    </v-container>
</template>

<script>
    export default {
        name: "PortfolioComponent",
        data(){
            return{
                activePortfolio:'webapp',
                webApps:[
                    {title:'Web App 1', image:'https://img.freepik.com/vector-gratis/desarrollo-aplicaciones-pagina-destino_52683-47903.jpg?w=740&t=st=1704747484~exp=1704748084~hmac=6e6866ec58792e7917ba618b738b59f4ab7e16f1591f988e77e58f1775078b7c'},
                    {title:'Web App 2', image:'https://img.freepik.com/vector-gratis/banner-desarrollo-aplicaciones_33099-1720.jpg?w=740&t=st=1704747597~exp=1704748197~hmac=baddedf0ca9d69457ef83abffdfcbd6be92ec1f8364f443ed896a14ba9829691'},
                    {title:'Web App 3', image:'https://img.freepik.com/vector-gratis/pagina-inicio-interfaz-usuario-ux-diseno-plano_23-2149093998.jpg?w=740&t=st=1704747624~exp=1704748224~hmac=e0da8534f93b777dbb82aa231271c16ec91cd314859b06ccb92dcef0e77f8d7b'},
                    {title:'Web App 4', image:'https://img.freepik.com/vector-gratis/conjunto-plantillas-diseno-pagina-destino-sitio-web-moderno-telefono-movil-o-tableta-articulos-galeria-formulario-contacto-ilustracion-aislada-plana_1284-60948.jpg?w=740&t=st=1704747641~exp=1704748241~hmac=3b7eacb8a11c9b22007f3009f4d96c6f4a6ae1e7c623bf67463b852b62ce3de9'},
                    {title:'Web App 5', image:'https://img.freepik.com/vector-gratis/pagina-inicio-ui-ux-degradado_52683-69488.jpg?w=740&t=st=1704747657~exp=1704748257~hmac=f748c6fd89e1fc02094279a02860c300edcc10ad114c30a00e2c250bf2132347'},
                    {title:'Web App 6', image:'https://img.freepik.com/vector-gratis/pagina-inicio-isometrica-ui-ux_52683-67970.jpg?w=740&t=st=1704747822~exp=1704748422~hmac=9550a0094b86d41f94f33def29c23621a545a077c13730b8d2ccf1e78705e293'},
            ],
                mobileApps:[
                    {title:'Mobile App 1', image:'https://img.freepik.com/vector-gratis/desarrolladores-computadoras-telefonos-inteligentes-que-trabajan-aplicacion-sola-pagina-gente-pequena-aplicacion-sola-pagina-pagina-web-spa-concepto-tendencia-desarrollo-web-ilustracion-aislada-violeta-vibrante-brillante_335657-984.jpg?w=740&t=st=1704749875~exp=1704750475~hmac=3ee6c008e5457a8cf24f54046c417b3ca2c9f03bd38680a132c5c36c52d825bc'},
                    {title:'Mobile App 2', image:'https://img.freepik.com/vector-gratis/plantilla-pagina-destino-isometrica-ui-ux_52683-67972.jpg?w=740&t=st=1704749973~exp=1704750573~hmac=22f1bd2eb3e7bd5d29e1e234e373f809a2cff89f8ac3ea38ad10a7c016b7bdae'},
                    {title:'Mobile App 3', image:'https://img.freepik.com/vector-gratis/pagina-destino-telefono-inteligente_23-2148337743.jpg?w=740&t=st=1704749990~exp=1704750590~hmac=ea7749b8ef6aeda353d3deff2dc489b0621e50161c53cbcab83e635fbe44dfae'},
                    {title:'Mobile App 4', image:'https://img.freepik.com/vector-gratis/plantilla-pagina-destino-plana-ui-ux_23-2149054885.jpg?w=740&t=st=1704749999~exp=1704750599~hmac=ebcff90847b438b4de44952ec31f2f71a7aea8f2825f48f4457828f7cdad837a'},
                    {title:'Mobile App 5', image:'https://img.freepik.com/vector-gratis/plantilla-pagina-destino-cms_52683-56270.jpg?w=740&t=st=1704750009~exp=1704750609~hmac=65ecf99ed57bfb2cdb9e3e80b8c2c7fc76188ac8f0cfba3e46e1c8f3e1b5cee1'},
            ],
                desktopApps:[
                    {title:'Desktop App 1', image:'https://img.freepik.com/vector-gratis/interfaz-usuario-aterrizaje-isometrico-diseno-receptivo_107791-8071.jpg?w=740&t=st=1704750019~exp=1704750619~hmac=b21ac626c1ed325226f37ff42526ff702c8bac3916be37ae6eb612875180b357'},
                    {title:'Desktop App 2', image:'https://img.freepik.com/vector-premium/desarrollo-aplicaciones-moviles-plantilla-pagina-destino_138260-28.jpg?w=740'},
                    {title:'Desktop App 3', image:'https://img.freepik.com/vector-gratis/coleccion-elementos-degradados-ui-ux_79603-1923.jpg?w=740&t=st=1704750038~exp=1704750638~hmac=bc75d35345317a647e3698a3e5b24877415363e061b3c15e1417a34c0e7a8e99'},
                    {title:'Desktop App 4', image:'https://img.freepik.com/vector-gratis/fondo-degradado-ui-ux_23-2149065783.jpg?w=740&t=st=1704750048~exp=1704750648~hmac=e4f03702a41c5a59d10d8a409b55a27b4c41840adfe7082699675fbb64a68cfd'},
                    {title:'Desktop App 5', image:'https://img.freepik.com/vector-gratis/plantilla-pagina-aterrizaje-degradada-ui-ux_23-2149051196.jpg?w=740&t=st=1704750060~exp=1704750660~hmac=070b3583399ac6888d0e028f43402d0f23458b117fb7c32180a5cd0fec3438f1'},
                    {title:'Desktop App 6', image:'https://img.freepik.com/vector-gratis/interfaz-aplicacion-compra-muebles_23-2148660330.jpg?w=740&t=st=1704750068~exp=1704750668~hmac=2efaf524335407aa47a0c82691b0c97fc448b0b27ce5aa39f8acdb6f018b2b79'},
            ],
        }
    }
}
</script>