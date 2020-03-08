<template>
  <div id="app">
    <div class="swipe">
      <span>スワイプ</span>
    </div>
    <div class="body">
      <Head />
      <Arms />
      <Legs />
    </div>
  </div>
</template>

<script>
import Head from './components/Head.vue';
import Arms from './components/Arms.vue';
import Legs from './components/Legs.vue';

export default {
  name: 'app',
  components: {
    Head,
    Arms,
    Legs,
  },
};
</script>

<style lang="scss">
/* http://meyerweb.com/eric/tools/css/reset/
  v2.0 | 20110126
  License: none (public domain)
*/

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
  box-sizing: border-box;
}
/* HTML5 display-role reset for older browsers */
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
body {
  line-height: 1;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: '';
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

#app {
  --color-line: #39200f;
  --color-body: #da00ff;
  --color-bg: #e3ff00;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--color-line);
  background-color: var(--color-bg);
  padding: 16px;
  min-height: 100vh;
  .swipe {
    display: block;
    height: 40vh;
    padding-top: 32px;
    span {
      position: relative;
      top: 80px;
      display: block;
      font-weight: bold;
      font-size: 24px;
    }
    &::before {
      content: '';
      width: 0;
      height: 0;
      border-right: 48px solid transparent;
      border-left: 48px solid transparent;
      border-bottom: 72px solid var(--color-line);
    }
  }
  .body {
    position: relative;
    width: 100%;
    height: 30000px;
    margin-bottom: 20500px;
    border-radius: 72px;
    background: var(--color-body);
    border: 16px solid var(--color-line);
  }
}
</style>
