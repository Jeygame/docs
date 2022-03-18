# Jeygame Functions

The main functions of Jeygame are meant to help you set up your game, and aren't entirely needed.

### `Jeygame.Make(instanceName : String, ?attributes : Object)`
Makes and returns an instance. You can set properties of the instance with the `attributes` argument, in a syntax of
```json
{
  "name": "value",
  "otherAttribute": "value"
}
```

#### Usage
```js
const Sprite = Jeygame.Make("Sprite", {
  "name": "Player"
})
```

#### Returns
```js
JeygameInternals.Instances.Sprite
```

### `Jeygame.Init(size : Jeygame.Vector2, ?appendTo : Element)`
Creates a canvas with the size of `size`, with an optional `appendTo` value to automatically append the canvas to.

#### Returns
```js
{
  "Game": JeygameInternals.Instances.GameController,
  "Canvas": HTMLCanvasElement,
  "CTX": CanvasRenderingContext2d
}
```
