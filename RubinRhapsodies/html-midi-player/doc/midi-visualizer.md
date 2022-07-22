# midi-visualizer

MIDI visualizer element.

The visualizer is implemented via SVG elements which support styling as described
[here](https://magenta.github.io/magenta-js/music/demos/visualizer.html).

See also the
[`@magenta/music/core/visualizer` docs](https://magenta.github.io/magenta-js/music/modules/_core_visualizer_.html).

## Properties

| Property       | Attribute | Type                                     | Description                                      |
|----------------|-----------|------------------------------------------|--------------------------------------------------|
| `config`       |           | `VisualizerConfig`                       | Magenta visualizer config object                 |
| `noteSequence` |           | `INoteSequence \| null`                  | Magenta note sequence object representing the currently displayed content |
| `src`          | `src`     | `string \| null`                         | MIDI file URL                                    |
| `type`         | `type`    | `"piano-roll" \| "waterfall" \| "staff"` | Visualizer type                                  |

## Methods

| Method             | Type                                      |
|--------------------|-------------------------------------------|
| `clearActiveNotes` | `(): void`                                |
| `redraw`           | `(activeNote?: INote \| undefined): void` |
| `reload`           | `(): void`                                |
