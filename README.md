# Text Cursor

A cursor trail effect where multiple instances of text follow the mouse pointer with optional physics-like movements.

## Installs

```bash
npm install motion
```

## Usage

```jsx
import TextCursor from './TextCursor';

const Example = () => {
  return (
    <div style={{ height: '100vh', width: '100vw' }}>
      <TextCursor 
        text="Hello" 
        color="#ff0000" 
      />
    </div>
  );
};

export default Example;
```

## Props

| Prop | Type | Default | Description |
| :--- | :--- | :--- | :--- |
| `text` | `string` | `'⚛️'` | The text/emoji to use for the trail particles. |
| `spacing` | `number` | `100` | Distance between generated trail particles. |
| `followMouseDirection` | `boolean` | `true` | Whether particles rotate to face mouse movement direction. |
| `randomFloat` | `boolean` | `true` | Adds random floating animation to particles. |
| `exitDuration` | `number` | `0.5` | Duration of the fade-out animation. |
| `removalInterval` | `number` | `30` | Interval (ms) for cleaning up old particles. |
| `maxPoints` | `number` | `5` | Maximum number of particles in the trail. |
