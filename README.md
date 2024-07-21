# ConfettiMakerLibrary

[![](https://jitpack.io/v/MaayanShiran/ConfettiMakerLibrary.svg)](https://jitpack.io/#MaayanShiran/ConfettiMakerLibrary)

ConfettiMakerLibrary is an Android library that provides a customizable ConfettiView for adding confetti animations to your applications.

## Features

- Customizable confetti shapes (circle, rectangle, snowflake)
- Configurable confetti colors, sizes, speeds, and gravity
- Easy integration with Android XML layout
- Supports dynamic runtime updates

## Installation

Add the JitPack repository to your root `build.gradle` file:

```gradle
allprojects {
    repositories {
        ...
        maven { url 'https://jitpack.io' }
    }
}
```

Add the dependency to your module build.gradle file:
```
dependencies {
    implementation("com.github.MaayanShiran:ConfettiMakerLibrary:1.00.13")
}
```

## XML Attributes

app:confettiColor - The color of the confetti (used if useSolidColor is true).
app:useSolidColor - Whether to use a single color or random colors.
app:minSize - The minimum size of the confetti.
app:maxSize - The maximum size of the confetti.
app:minSpeedX - The minimum horizontal speed of the confetti.
app:maxSpeedX - The maximum horizontal speed of the confetti.
app:minSpeedY - The minimum vertical speed of the confetti.
app:maxSpeedY - The maximum vertical speed of the confetti.
app:gravity - The gravity effect on the confetti.
app:shapeType - The shape of the confetti (0 for circle, 1 for rectangle, 2 for snowflake).

## Java Methods

setConfettiColor(int color) - Set the confetti color.
setUseSolidColor(boolean useSolidColor) - Set whether to use a single color or random colors.
setSizeRange(float minSize, float maxSize) - Set the size range of the confetti.
setSpeedXRange(float minSpeedX, float maxSpeedX) - Set the horizontal speed range of the confetti.
setSpeedYRange(float minSpeedY, float maxSpeedY) - Set the vertical speed range of the confetti.
setGravity(float gravity) - Set the gravity effect on the confetti.
setShapeType(int shapeType) - Set the shape type of the confetti.
getShapeType() - Get the current shape type of the confetti.
