<script>
    let instructions =  [
        {
            name: "Abrir la billetera",
            description:
                "Abre una billetera Lightning que soporta LNURL. Sugerencia: Tu billetera Bitcoin Txoko LNbits funciona muy bien.",
        },
        {
            name: "Escanear código QR",
            description:
                "Escanea el código QR desde tu billetera o púlsalo para abrirlo en tu billetera. También puedes copiar la dirección Lightning y pegarla en tu billetera.",
        },
        {
            name: "Enviar sats",
            description:
                "Establece una cantidad a enviar y pulsa enviar.",
        },
        {
            name: "Comprobar el saldo",
            description:
                "Actualiza esta página para ver el saldo actualizado de la lotería.",
        },
    ];
</script>

<div class="m-6 p-2 sm:p-4 md:p-6 rounded-2xl border border-solid hover:border-bright bg-white font-mono max-w-lg">
    <div class="text-muted-bright mx-2 justify-center">
            <h2 class="font-bold text-xl text-center">Instrucciones</h2>
            {#each instructions as instruction, index}
            <div class="my-2">
                <h3 class="text-md font-semibold">{index+1}. {instruction.name}</h3>
                <p class="mx-2 mt">{instruction.description}</p>
            </div>
            {/each}
    </div>
</div>  
