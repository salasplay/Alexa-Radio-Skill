# Alexa-Skills
Desarrollo de skills alexa en español mx

Hola a todos alexa dev´s mi nombre es Oliver GOnzaléz y explicare como crear una skill de radio en español MX.
Primero debemos crear nuestra skill en español (mx) en este ejemplo se llamara “radio patito”
Después vamos a JSON Editor, eliminamos lo que esta pre-cargado y pegamos lo que tenemos en el archivo JSON es-MX:

{
    "interactionModel": {
        "languageModel": {
            "invocationName": "radio patito",
            "intents": [
                {
                    "name": "PlayStreamIntent",
                    "slots": [],
                    "samples": [
                        "reproduce",
                        "inicia",
                        "abre",
                        "sintoniza",
                        "toca",
                        "quiero escuchar",
                        "quiero oir"
                    ]
                },
                {
                    "name": "AboutIntent",
                    "slots": [],
                    "samples": [
                        "acerca",
                        "que es esto"
                    ]
                },
                {
                    "name": "AMAZON.PauseIntent",
                    "samples": []
                },
                {
                    "name": "AMAZON.ResumeIntent",
                    "samples": []
                },
                {
                    "name": "AMAZON.StopIntent",
                    "samples": [
                        "callate",
                        "detente"
                    ]
                },
                {
                    "name": "AMAZON.CancelIntent",
                    "samples": [
                        "salir"
                    ]
                },
                {
                    "name": "AMAZON.HelpIntent",
                    "samples": [
                        "ayuda",
                        "como funciona"
                    ]
                },
                {
                    "name": "AMAZON.NavigateHomeIntent",
                    "samples": []
                }
            ],
            "types": []
        }
    }
}
 Guardamos el modelo y hacemos la construccion del modelo (Build Model)
 
 ***Despues debemos ir a INTERFACES y activar AUDIO PLAYER
 
 Posteriormente usamos el codigo NodeJS del archivo index.js
