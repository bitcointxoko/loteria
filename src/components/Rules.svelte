<script>
    let rules =  [
        {
            name: "👬 Equipos",
            description:
                "Forma equipos de no más de tres miembros por equipo. ",
        },
        {
            name: "❓ Preguntas",
            description:
                "El concurso de preguntas consta de 21 preguntas de opción múltiple. Con preguntas de desempate adicionales.",
        },
        {
            name: "⏳ Tiempo",
            description:
                "Tienes 3 minutos para responder a cada pregunta con tu equipo. No puedes utilizar un dispositivo conectado a Internet para responder a las preguntas. ",
        },
        {
            name: "💯 Puntos",
            description:
                "Una respuesta correcta vale un punto. No hay puntos por respuestas incorrectas. ",
        },
        {
            name: "🏆 Ganador",
            description:
                "El equipo con el mayor número de puntos gana los sats.",
        },
    ];
</script>

<div class="mx-6 mb-8 p-2 sm:p-4 md:p-6 rounded-2xl border border-solid hover:border-bright bg-white font-mono max-w-lg">
    <div class="text-muted-bright mx-2 justify-center">
            <h2 class="font-bold text-xl text-center">Reglas</h2>
            <ul>
                {#each rules as rule}
                <li class="my-2">
                    <h3 class="text-md font-semibold">{rule.name}</h3>
                    <p class="mx-2 mt">{rule.description}</p>
                </li>
                {/each}
            </ul>
    </div>
</div>  
