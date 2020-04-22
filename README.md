To initialize the script Materialize Form

1. Include materialize.css file
2. Import ninja.js
3. Import Materialize from materialize.js
4. New Materialize().Form()
5. Provide ID of form when newing
6. Make sure all elements you want Materialized have `tabindex` attribute on them. Without this they will be skipped over and not included in your new Materialize Form

```html
<!DOCTYPE html>

<link href="Materialize/materialize.css" rel="stylesheet" />

<script type="module">
    
    import "./Materialize/ninja.js";

    import Materialize from "./Materialize/materialize.js";

    // add to window scope so it can be access in console, if you want
    window.NinjaForm = new Materialize( )
        .Form( {
            form: 'NinjaForm',
        } );

</script>

<div id="NinjaForm">
    <material text>
        <label for="default-text-field"><span>Default Text Field</span></label>
        <input type="text" id="default-text-field" name="default-text-field" value="" tabindex="1">
    </material>
</div>
```

[Materialize.Ninja! Docs](https://docs.materialize.ninja/)

[Materialize.Ninja! Demo](https://materialize.ninja/)
