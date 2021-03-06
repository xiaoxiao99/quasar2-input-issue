# quasar2-input-issue
To demo a quasar2 Q-input issue with Japanese IME on Android system.

This issue happens only if **ALL** the following conditions are true.
1. **Q-input** inside **Q-page** element, which is enclosed by **Q-page-container** then **Q-layout**. 
2. **Q-input** has validation rules
3. Android phone
4. Screen in portrait mode
5. Japense IME input SW keyboard

When all above are true, the keyboard inputs are always automatically cleared during composition, thus nothing left.

## How to produce this issue.
1. Open browser app on Android phone
2. Visist [https://xiaoxiao99.github.io/quasar2-input-issue/index.html](https://xiaoxiao99.github.io/quasar2-input-issue/index.html)
3. Switch input method to Japanese IME
4. Focus on input "w/o validation", type anything, no issue observed.
5. Focus on input "w/ validation", type something, the issue can be observed.

Here is a video of screen capture


https://user-images.githubusercontent.com/8103965/173372686-19b498c4-e674-43a1-9c69-709ba3c94664.mp4


The same code can be played with codepen here.
https://codepen.io/xiaoxiao22/pen/jOZQQzL
