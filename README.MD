<!-- Preview = Ctrl + Maj + V on VsCode-->
# Animation en CSS
#### Les différentes manières d'en créer.
* ##### Exercice 1: Déplacer un bouton. 

```bash

# 1: Créer une div contenant un bouton dans mon HTML 

<div class="button_div1">
    <button> Cliquez ici </button>
</div>

# 2: Appliquer du style à mon bouton via mon CSS

.button_div1 {
    animation: apparition-down 0.8s ease-in-out; # Nom keyframe / Temps d'animation / effet de transition
    margin: 10px;
}

# 3: Déclarer un keyframe.

 @keyframes apparition {
    from {                                  # from = départ de l'animation
      opacity: 0;
      -webkit-transform: translateX(-3rem); # compatibilité Safari et Chrome
              transform: translateX(-3rem);
    }
    to {                                    # to = fin de l'animation 
      opacity: 1;
      -webkit-transform: translateX(0rem);
              transform: translateX(0rem);
    }
  }
```

