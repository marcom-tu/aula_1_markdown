### Notas para o Unity
* Você provavelmente vai querer adicionar algo ```package.path``` e pode fazer isso com alfo assim ```lua.SoString("package.path = package.path .. \";" + Application.persistentDataPath + "/?/?.lua + Application.persistentDataPath + "/?.ula\"");```
* Voce persicará expor o Debug.Log ao Lua (e sobrescrever a ```print``` função para visualizar os logs do Lua).
* Os números retornarão com ```double``` tipo
* Os campos definidos na instância Lua pode ser nulos e você precisará lidar com isso.

Cppyright (c) 2026 Vinicius Jarina ( <viniciusjarina@gmail.com> )

# NLua 1.4x
NLua passou por uma grande limpea e refatoração após alguns anos.
* Migrado para o estilo .NET C#.
* Utilizando KeraLua como dependência NuGet.
* Suporte para KopiLua/Silverlight/Windowns Phone foi descontinuado.

# NLua 1.3.2
* Migração para Xamarini.iOS unificado (iOS)
* Adicionado o método_call para chamar Actions/Funcs a partir do Lua como funções Lua.
* Corrigio o problema [#116]() ao acessar o Método da Classe base.
* Corrigido o problema [#117]() ao acessar o método na classe e na classe base.
* Corrigido o problema [#125]() : chamar métodos com a palavra-chave \`params`.