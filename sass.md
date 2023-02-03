# Guía Burros Sass

___

## Variables

Puedes definir variables en Sass con el signo de dólar `$` seguido del nombre de la variable. Por ejemplo:

    $color: #f00;
    $width: 100px;

___

## Anidación

Puedes anidar reglas CSS dentro de otras reglas CSS. Por ejemplo:

    nav {
      ul {
        margin: 0;
        padding: 0;
        list-style: none;
      }
      li { display: inline-block; }
      a {
        display: block;
        padding: 6px 12px;
        text-decoration: none;
      }
    }

Para selectores y pseudo-selectores, puedes anidarlos dentro de reglas CSS con el caracter `&` . Por ejemplo:

    a {
      color: #00f;
      &:hover { color: #f00; }
    }

Puedes anidar también clases e IDs. Por ejemplo:

    .page-container {
      .content { width: 100%; }
      #navigation { float: left; }
    }

___

## Separación en archivos

Puedes separar tu código en archivos y luego importarlos en tu archivo principal. No olvides que los archivos secundarios empiezan por `_` . Por ejemplo:

    // _reset.scss

    // _typography.scss

    // main.scss
    @import "reset";
    @import "typography";
___

## Mixins

Puedes definir mixins con el keyword `@mixin` . Por ejemplo:

    @mixin border-radius($radius) {
      -webkit-border-radius: $radius;
      -moz-border-radius: $radius;
      -ms-border-radius: $radius;
      -o-border-radius: $radius;
      border-radius: $radius;
    }

Para usar un mixin, usas el keyword `@include` . Por ejemplo:

        .box { @include border-radius(10px); }
___

## Extend

Puedes extender un selector con el keyword `@extend` . Por ejemplo:

    .message {
      border: 1px #ccc solid;
      padding: 10px;
      color: #333;
    }
    .success { @extend .message; border-color: green; }
    .error { @extend .message; border-color: red; }
    .warning { @extend .message; border-color: yellow; }

Para sobreescribir lo heredado basta con usar la propiedad después del `@extend`
___

## Operaciones

Puedes hacer operaciones matemáticas en Sass. Por ejemplo:

    .element {
      width: 100% / 3;
    }
___

## Funciones

Puedes usar funciones en Sass. Por ejemplo:

    @function double($n) {
        @return $n * 2;
    }
