# Atividade – Intents no Android

Projeto simples para demonstrar Intent explícita e Intent implícita.

## Intent explícita
No `MainActivity`, o botão "Intent Explícita" abre diretamente a `SegundaActivity`.

```java
Intent intent = new Intent(MainActivity.this, SegundaActivity.class);
startActivity(intent);
```

## Intent implícita
O botão "Intent Implícita" abre o Google no navegador padrão:

```java
Intent intent = new Intent(
    Intent.ACTION_VIEW,
    Uri.parse("https://www.google.com")
);
startActivity(intent);
```

## Como executar
1. Abra a pasta do projeto no Android Studio.
2. Aguarde o Gradle sincronizar.
3. Execute em um emulador ou dispositivo Android.
4. Teste os dois botões.
