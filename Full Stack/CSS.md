# Making a UL with classes have properties or not (ul[class] and ul:not(class))

## **If ul has class then apply** the properties 

```css
ul[class] {
list-style:none;
other properties
}
```

## **If ul has no class then apply** the properties inside it 

```css
ul:not[class] {
Properties if ul has no class
}
```

