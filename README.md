# How do I embed a silent, looping MP4 into a GitHub README?

## Drag MP4 into markdown editor? ❌

Plays, but doesn't loop or autoplay.

https://github.com/user-attachments/assets/54e1231f-49a3-4b6b-868c-8168c16732fe

## Add markdown image reference to dragged file? ❌

Works in Safari but not in Chrome thanks to [this Safari-specific quirk](https://lapcatsoftware.com/articles/img1.html).

<img width="993" height="122" alt="image" src="https://github.com/user-attachments/assets/3429759f-6bc8-48e9-85b6-6e1839e98273" />

```markdown
![](https://github.com/user-attachments/assets/54e1231f-49a3-4b6b-868c-8168c16732fe)
```
![](https://github.com/user-attachments/assets/54e1231f-49a3-4b6b-868c-8168c16732fe)

## Add HTML video tag referencing the dragged file? ❌

Doesn't even show up. Is the markdown parser stripping them out? Do muted <1MB mp4 videos represent a security risk or something?

```markdown
<video playsinline autoplay loop muted>source src="https://github.com/user-attachments/assets/54e1231f-49a3-4b6b-868c-8168c16732fe" type="video/mp4"></video>
```

<video playsinline autoplay loop muted>source src="https://github.com/user-attachments/assets/54e1231f-49a3-4b6b-868c-8168c16732fe" type="video/mp4"></video>
