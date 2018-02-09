# designkit-layout
1.0.0

Sass module for css flex layouts

## Install
```
npm i --save designkit-layout
```

### CSS

```css
/* Sizes:
  0    <= size < 600  Phone
  600  <= size < 960  Tablet
  960  <= size < 1200 Tablet-Landscape
  1200 <= size         PC
*/
[layout] {
  box-sizing: border-box;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
}

[layout=column] {
  -webkit-box-orient: vertical;
  -webkit-box-direction: normal;
      -ms-flex-direction: column;
          flex-direction: column;
}

[layout=row] {
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
      -ms-flex-direction: row;
          flex-direction: row;
}

[layout-padding] > [flex-sm],
[layout-padding] > [flex-lt-md] {
  padding: 4px;
}

[layout-padding],
[layout-padding] > [flex],
[layout-padding] > [flex-gt-sm],
[layout-padding] > [flex-md],
[layout-padding] > [flex-lt-lg] {
  padding: 8px;
}

[layout-padding] > [flex-gt-md],
[layout-padding] > [flex-lg] {
  padding: 16px;
}

[layout-margin] > [flex-sm],
[layout-margin] > [flex-lt-md] {
  margin: 4px;
}

[layout-margin],
[layout-margin] > [flex],
[layout-margin] > [flex-gt-sm],
[layout-margin] > [flex-md],
[layout-margin] > [flex-lt-lg] {
  margin: 8px;
}

[layout-margin] > [flex-gt-md],
[layout-margin] > [flex-lg] {
  margin: 16px;
}

[layout-wrap] {
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
}

[layout-fill] {
  margin: 0;
  min-height: 100%;
  width: 100%;
}

@-moz-document url-prefix() {
  [layout-fill] {
    margin: 0;
    width: 100%;
    min-height: auto;
    height: inherit;
  }
}

[flex] {
  box-sizing: border-box;
  -webkit-box-flex: 1;
      -ms-flex: 1;
          flex: 1;
}

[flex="0"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 0%;
          flex: 0 0 0%;
}

[layout="row"] > [flex="0"] {
  max-width: 0%;
}

[layout="column"] > [flex="0"] {
  max-height: 0%;
}

[flex="5"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 5%;
          flex: 0 0 5%;
}

[layout="row"] > [flex="5"] {
  max-width: 5%;
}

[layout="column"] > [flex="5"] {
  max-height: 5%;
}

[flex="10"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 10%;
          flex: 0 0 10%;
}

[layout="row"] > [flex="10"] {
  max-width: 10%;
}

[layout="column"] > [flex="10"] {
  max-height: 10%;
}

[flex="15"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 15%;
          flex: 0 0 15%;
}

[layout="row"] > [flex="15"] {
  max-width: 15%;
}

[layout="column"] > [flex="15"] {
  max-height: 15%;
}

[flex="20"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 20%;
          flex: 0 0 20%;
}

[layout="row"] > [flex="20"] {
  max-width: 20%;
}

[layout="column"] > [flex="20"] {
  max-height: 20%;
}

[flex="25"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 25%;
          flex: 0 0 25%;
}

[layout="row"] > [flex="25"] {
  max-width: 25%;
}

[layout="column"] > [flex="25"] {
  max-height: 25%;
}

[flex="30"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 30%;
          flex: 0 0 30%;
}

[layout="row"] > [flex="30"] {
  max-width: 30%;
}

[layout="column"] > [flex="30"] {
  max-height: 30%;
}

[flex="35"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 35%;
          flex: 0 0 35%;
}

[layout="row"] > [flex="35"] {
  max-width: 35%;
}

[layout="column"] > [flex="35"] {
  max-height: 35%;
}

[flex="40"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 40%;
          flex: 0 0 40%;
}

[layout="row"] > [flex="40"] {
  max-width: 40%;
}

[layout="column"] > [flex="40"] {
  max-height: 40%;
}

[flex="45"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 45%;
          flex: 0 0 45%;
}

[layout="row"] > [flex="45"] {
  max-width: 45%;
}

[layout="column"] > [flex="45"] {
  max-height: 45%;
}

[flex="50"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 50%;
          flex: 0 0 50%;
}

[layout="row"] > [flex="50"] {
  max-width: 50%;
}

[layout="column"] > [flex="50"] {
  max-height: 50%;
}

[flex="55"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 55%;
          flex: 0 0 55%;
}

[layout="row"] > [flex="55"] {
  max-width: 55%;
}

[layout="column"] > [flex="55"] {
  max-height: 55%;
}

[flex="60"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 60%;
          flex: 0 0 60%;
}

[layout="row"] > [flex="60"] {
  max-width: 60%;
}

[layout="column"] > [flex="60"] {
  max-height: 60%;
}

[flex="65"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 65%;
          flex: 0 0 65%;
}

[layout="row"] > [flex="65"] {
  max-width: 65%;
}

[layout="column"] > [flex="65"] {
  max-height: 65%;
}

[flex="70"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 70%;
          flex: 0 0 70%;
}

[layout="row"] > [flex="70"] {
  max-width: 70%;
}

[layout="column"] > [flex="70"] {
  max-height: 70%;
}

[flex="75"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 75%;
          flex: 0 0 75%;
}

[layout="row"] > [flex="75"] {
  max-width: 75%;
}

[layout="column"] > [flex="75"] {
  max-height: 75%;
}

[flex="80"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 80%;
          flex: 0 0 80%;
}

[layout="row"] > [flex="80"] {
  max-width: 80%;
}

[layout="column"] > [flex="80"] {
  max-height: 80%;
}

[flex="85"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 85%;
          flex: 0 0 85%;
}

[layout="row"] > [flex="85"] {
  max-width: 85%;
}

[layout="column"] > [flex="85"] {
  max-height: 85%;
}

[flex="90"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 90%;
          flex: 0 0 90%;
}

[layout="row"] > [flex="90"] {
  max-width: 90%;
}

[layout="column"] > [flex="90"] {
  max-height: 90%;
}

[flex="95"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 95%;
          flex: 0 0 95%;
}

[layout="row"] > [flex="95"] {
  max-width: 95%;
}

[layout="column"] > [flex="95"] {
  max-height: 95%;
}

[flex="100"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 100%;
          flex: 0 0 100%;
}

[layout="row"] > [flex="100"] {
  max-width: 100%;
}

[layout="column"] > [flex="100"] {
  max-height: 100%;
}

[flex="33"], [flex="34"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 33.33%;
          flex: 0 0 33.33%;
}

[flex="66"], [flex="67"] {
  -webkit-box-flex: 0;
      -ms-flex: 0 0 66.66%;
          flex: 0 0 66.66%;
}

[layout="row"] > [flex="33"], [layout="row"] > [flex="34"] {
  max-width: 33.33%;
}

[layout="row"] > [flex="66"], [layout="row"] > [flex="67"] {
  max-width: 66.66%;
}

[layout="column"] > [flex="33"], [layout="column"] > [flex="34"] {
  max-height: 33.33%;
}

[layout="column"] > [flex="66"], [layout="column"] > [flex="67"] {
  max-height: 66.66%;
}

[layout-align="center"],
[layout-align="center center"],
[layout-align="center start"],
[layout-align="center end"] {
  -webkit-box-pack: center;
      -ms-flex-pack: center;
          justify-content: center;
}

[layout-align="end"],
[layout-align="end center"],
[layout-align="end start"],
[layout-align="end end"] {
  -webkit-box-pack: end;
      -ms-flex-pack: end;
          justify-content: flex-end;
}

[layout-align="space-around"],
[layout-align="space-around center"],
[layout-align="space-around start"],
[layout-align="space-around end"] {
  -ms-flex-pack: distribute;
      justify-content: space-around;
}

[layout-align="space-between"],
[layout-align="space-between center"],
[layout-align="space-between start"],
[layout-align="space-between end"] {
  -webkit-box-pack: justify;
      -ms-flex-pack: justify;
          justify-content: space-between;
}

[layout-align="center center"],
[layout-align="start center"],
[layout-align="end center"],
[layout-align="space-between center"],
[layout-align="space-around center"] {
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
}

[layout-align="center start"],
[layout-align="start start"],
[layout-align="end start"],
[layout-align="space-between start"],
[layout-align="space-around start"] {
  -webkit-box-align: start;
      -ms-flex-align: start;
          align-items: flex-start;
}

[layout-align="center end"],
[layout-align="start end"],
[layout-align="end end"],
[layout-align="space-between end"],
[layout-align="space-around end"] {
  -webkit-box-align: end;
      -ms-flex-align: end;
          align-items: flex-end;
}

[flex-order="0"] {
  -webkit-box-ordinal-group: 1;
      -ms-flex-order: 0;
          order: 0;
}

[flex-order="1"] {
  -webkit-box-ordinal-group: 2;
      -ms-flex-order: 1;
          order: 1;
}

[flex-order="2"] {
  -webkit-box-ordinal-group: 3;
      -ms-flex-order: 2;
          order: 2;
}

[flex-order="3"] {
  -webkit-box-ordinal-group: 4;
      -ms-flex-order: 3;
          order: 3;
}

[flex-order="4"] {
  -webkit-box-ordinal-group: 5;
      -ms-flex-order: 4;
          order: 4;
}

[flex-order="5"] {
  -webkit-box-ordinal-group: 6;
      -ms-flex-order: 5;
          order: 5;
}

[flex-order="6"] {
  -webkit-box-ordinal-group: 7;
      -ms-flex-order: 6;
          order: 6;
}

[flex-order="7"] {
  -webkit-box-ordinal-group: 8;
      -ms-flex-order: 7;
          order: 7;
}

[flex-order="8"] {
  -webkit-box-ordinal-group: 9;
      -ms-flex-order: 8;
          order: 8;
}

[flex-order="9"] {
  -webkit-box-ordinal-group: 10;
      -ms-flex-order: 9;
          order: 9;
}

[offset="5"] {
  margin-left: 5%;
}

[offset="10"] {
  margin-left: 10%;
}

[offset="15"] {
  margin-left: 15%;
}

[offset="20"] {
  margin-left: 20%;
}

[offset="25"] {
  margin-left: 25%;
}

[offset="30"] {
  margin-left: 30%;
}

[offset="35"] {
  margin-left: 35%;
}

[offset="40"] {
  margin-left: 40%;
}

[offset="45"] {
  margin-left: 45%;
}

[offset="50"] {
  margin-left: 50%;
}

[offset="55"] {
  margin-left: 55%;
}

[offset="60"] {
  margin-left: 60%;
}

[offset="65"] {
  margin-left: 65%;
}

[offset="70"] {
  margin-left: 70%;
}

[offset="75"] {
  margin-left: 75%;
}

[offset="80"] {
  margin-left: 80%;
}

[offset="85"] {
  margin-left: 85%;
}

[offset="90"] {
  margin-left: 90%;
}

[offset="95"] {
  margin-left: 95%;
}

[offset="33"], [offset="34"] {
  margin-left: 33.33%;
}

[offset="66"], [offset="67"] {
  margin-left: 66.66%;
}

/**
 * `hide-gt-sm show-gt-lg` should hide from 600px to 1200px
 * `show-md hide-gt-sm` should show from 0px to 960px and hide at >960px
 * `hide-gt-md show-gt-sm` should show everywhere (show overrides hide)`
 */
@media (max-width: 599px) {
  [hide-sm]:not([show-sm]):not([show]), [hide]:not([show-sm]):not([show]) {
    display: none;
  }
  [flex-order-sm="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-sm="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-sm="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-sm="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-sm="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-sm="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-sm="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-sm="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-sm="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-sm="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-sm="center"],
  [layout-align-sm="center center"],
  [layout-align-sm="center start"],
  [layout-align-sm="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-sm="end"],
  [layout-align-sm="end center"],
  [layout-align-sm="end start"],
  [layout-align-sm="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-sm="space-around"],
  [layout-align-sm="space-around center"],
  [layout-align-sm="space-around start"],
  [layout-align-sm="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-sm="space-between"],
  [layout-align-sm="space-between center"],
  [layout-align-sm="space-between start"],
  [layout-align-sm="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-sm="center center"],
  [layout-align-sm="start center"],
  [layout-align-sm="end center"],
  [layout-align-sm="space-between center"],
  [layout-align-sm="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-sm="center start"],
  [layout-align-sm="start start"],
  [layout-align-sm="end start"],
  [layout-align-sm="space-between start"],
  [layout-align-sm="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-sm="center end"],
  [layout-align-sm="start end"],
  [layout-align-sm="end end"],
  [layout-align-sm="space-between end"],
  [layout-align-sm="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-sm] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-sm=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-sm=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-sm="5"] {
    margin-left: 5%;
  }
  [offset-sm="10"] {
    margin-left: 10%;
  }
  [offset-sm="15"] {
    margin-left: 15%;
  }
  [offset-sm="20"] {
    margin-left: 20%;
  }
  [offset-sm="25"] {
    margin-left: 25%;
  }
  [offset-sm="30"] {
    margin-left: 30%;
  }
  [offset-sm="35"] {
    margin-left: 35%;
  }
  [offset-sm="40"] {
    margin-left: 40%;
  }
  [offset-sm="45"] {
    margin-left: 45%;
  }
  [offset-sm="50"] {
    margin-left: 50%;
  }
  [offset-sm="55"] {
    margin-left: 55%;
  }
  [offset-sm="60"] {
    margin-left: 60%;
  }
  [offset-sm="65"] {
    margin-left: 65%;
  }
  [offset-sm="70"] {
    margin-left: 70%;
  }
  [offset-sm="75"] {
    margin-left: 75%;
  }
  [offset-sm="80"] {
    margin-left: 80%;
  }
  [offset-sm="85"] {
    margin-left: 85%;
  }
  [offset-sm="90"] {
    margin-left: 90%;
  }
  [offset-sm="95"] {
    margin-left: 95%;
  }
  [offset-sm="33"], [offset-sm="34"] {
    margin-left: 33.33%;
  }
  [offset-sm="66"], [offset-sm="67"] {
    margin-left: 66.66%;
  }
  [flex-sm] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-sm="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-sm="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-sm="0"] {
    max-height: 0%;
  }
  [flex-sm="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-sm="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-sm="5"] {
    max-height: 5%;
  }
  [flex-sm="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-sm="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-sm="10"] {
    max-height: 10%;
  }
  [flex-sm="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-sm="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-sm="15"] {
    max-height: 15%;
  }
  [flex-sm="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-sm="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-sm="20"] {
    max-height: 20%;
  }
  [flex-sm="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-sm="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-sm="25"] {
    max-height: 25%;
  }
  [flex-sm="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-sm="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-sm="30"] {
    max-height: 30%;
  }
  [flex-sm="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-sm="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-sm="35"] {
    max-height: 35%;
  }
  [flex-sm="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-sm="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-sm="40"] {
    max-height: 40%;
  }
  [flex-sm="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-sm="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-sm="45"] {
    max-height: 45%;
  }
  [flex-sm="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-sm="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-sm="50"] {
    max-height: 50%;
  }
  [flex-sm="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-sm="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-sm="55"] {
    max-height: 55%;
  }
  [flex-sm="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-sm="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-sm="60"] {
    max-height: 60%;
  }
  [flex-sm="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-sm="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-sm="65"] {
    max-height: 65%;
  }
  [flex-sm="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-sm="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-sm="70"] {
    max-height: 70%;
  }
  [flex-sm="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-sm="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-sm="75"] {
    max-height: 75%;
  }
  [flex-sm="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-sm="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-sm="80"] {
    max-height: 80%;
  }
  [flex-sm="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-sm="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-sm="85"] {
    max-height: 85%;
  }
  [flex-sm="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-sm="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-sm="90"] {
    max-height: 90%;
  }
  [flex-sm="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-sm="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-sm="95"] {
    max-height: 95%;
  }
  [flex-sm="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-sm="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-sm="100"] {
    max-height: 100%;
  }
  [flex-sm="33"], [flex-sm="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-sm="66"], [flex-sm="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-sm="33"], [layout="row"] > [flex-sm="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-sm="66"], [layout="row"] > [flex-sm="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-sm="33"], [layout="column"] > [flex-sm="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-sm="66"], [layout="column"] > [flex-sm="67"] {
    max-height: 66.66%;
  }
}

@media (min-width: 600px) {
  [flex-order-gt-sm="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-gt-sm="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-gt-sm="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-gt-sm="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-gt-sm="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-gt-sm="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-gt-sm="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-gt-sm="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-gt-sm="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-gt-sm="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-gt-sm="center"],
  [layout-align-gt-sm="center center"],
  [layout-align-gt-sm="center start"],
  [layout-align-gt-sm="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-gt-sm="end"],
  [layout-align-gt-sm="end center"],
  [layout-align-gt-sm="end start"],
  [layout-align-gt-sm="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-gt-sm="space-around"],
  [layout-align-gt-sm="space-around center"],
  [layout-align-gt-sm="space-around start"],
  [layout-align-gt-sm="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-gt-sm="space-between"],
  [layout-align-gt-sm="space-between center"],
  [layout-align-gt-sm="space-between start"],
  [layout-align-gt-sm="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-gt-sm="center center"],
  [layout-align-gt-sm="start center"],
  [layout-align-gt-sm="end center"],
  [layout-align-gt-sm="space-between center"],
  [layout-align-gt-sm="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-gt-sm="center start"],
  [layout-align-gt-sm="start start"],
  [layout-align-gt-sm="end start"],
  [layout-align-gt-sm="space-between start"],
  [layout-align-gt-sm="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-gt-sm="center end"],
  [layout-align-gt-sm="start end"],
  [layout-align-gt-sm="end end"],
  [layout-align-gt-sm="space-between end"],
  [layout-align-gt-sm="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-gt-sm] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-gt-sm=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-gt-sm=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-gt-sm="5"] {
    margin-left: 5%;
  }
  [offset-gt-sm="10"] {
    margin-left: 10%;
  }
  [offset-gt-sm="15"] {
    margin-left: 15%;
  }
  [offset-gt-sm="20"] {
    margin-left: 20%;
  }
  [offset-gt-sm="25"] {
    margin-left: 25%;
  }
  [offset-gt-sm="30"] {
    margin-left: 30%;
  }
  [offset-gt-sm="35"] {
    margin-left: 35%;
  }
  [offset-gt-sm="40"] {
    margin-left: 40%;
  }
  [offset-gt-sm="45"] {
    margin-left: 45%;
  }
  [offset-gt-sm="50"] {
    margin-left: 50%;
  }
  [offset-gt-sm="55"] {
    margin-left: 55%;
  }
  [offset-gt-sm="60"] {
    margin-left: 60%;
  }
  [offset-gt-sm="65"] {
    margin-left: 65%;
  }
  [offset-gt-sm="70"] {
    margin-left: 70%;
  }
  [offset-gt-sm="75"] {
    margin-left: 75%;
  }
  [offset-gt-sm="80"] {
    margin-left: 80%;
  }
  [offset-gt-sm="85"] {
    margin-left: 85%;
  }
  [offset-gt-sm="90"] {
    margin-left: 90%;
  }
  [offset-gt-sm="95"] {
    margin-left: 95%;
  }
  [offset-gt-sm="33"], [offset-gt-sm="34"] {
    margin-left: 33.33%;
  }
  [offset-gt-sm="66"], [offset-gt-sm="67"] {
    margin-left: 66.66%;
  }
  [flex-gt-sm] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-gt-sm="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-gt-sm="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-gt-sm="0"] {
    max-height: 0%;
  }
  [flex-gt-sm="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-gt-sm="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-gt-sm="5"] {
    max-height: 5%;
  }
  [flex-gt-sm="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-gt-sm="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-gt-sm="10"] {
    max-height: 10%;
  }
  [flex-gt-sm="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-gt-sm="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-gt-sm="15"] {
    max-height: 15%;
  }
  [flex-gt-sm="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-gt-sm="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-gt-sm="20"] {
    max-height: 20%;
  }
  [flex-gt-sm="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-gt-sm="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-gt-sm="25"] {
    max-height: 25%;
  }
  [flex-gt-sm="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-gt-sm="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-gt-sm="30"] {
    max-height: 30%;
  }
  [flex-gt-sm="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-gt-sm="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-gt-sm="35"] {
    max-height: 35%;
  }
  [flex-gt-sm="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-gt-sm="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-gt-sm="40"] {
    max-height: 40%;
  }
  [flex-gt-sm="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-gt-sm="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-gt-sm="45"] {
    max-height: 45%;
  }
  [flex-gt-sm="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-gt-sm="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-gt-sm="50"] {
    max-height: 50%;
  }
  [flex-gt-sm="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-gt-sm="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-gt-sm="55"] {
    max-height: 55%;
  }
  [flex-gt-sm="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-gt-sm="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-gt-sm="60"] {
    max-height: 60%;
  }
  [flex-gt-sm="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-gt-sm="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-gt-sm="65"] {
    max-height: 65%;
  }
  [flex-gt-sm="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-gt-sm="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-gt-sm="70"] {
    max-height: 70%;
  }
  [flex-gt-sm="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-gt-sm="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-gt-sm="75"] {
    max-height: 75%;
  }
  [flex-gt-sm="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-gt-sm="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-gt-sm="80"] {
    max-height: 80%;
  }
  [flex-gt-sm="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-gt-sm="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-gt-sm="85"] {
    max-height: 85%;
  }
  [flex-gt-sm="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-gt-sm="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-gt-sm="90"] {
    max-height: 90%;
  }
  [flex-gt-sm="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-gt-sm="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-gt-sm="95"] {
    max-height: 95%;
  }
  [flex-gt-sm="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-gt-sm="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-gt-sm="100"] {
    max-height: 100%;
  }
  [flex-gt-sm="33"], [flex-gt-sm="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-gt-sm="66"], [flex-gt-sm="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-gt-sm="33"], [layout="row"] > [flex-gt-sm="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-gt-sm="66"], [layout="row"] > [flex-gt-sm="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-gt-sm="33"], [layout="column"] > [flex-gt-sm="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-gt-sm="66"], [layout="column"] > [flex-gt-sm="67"] {
    max-height: 66.66%;
  }
}

@media (min-width: 600px) and (max-width: 959px) {
  [hide]:not([show-gt-sm]):not([show-md]):not([show]), [hide-gt-sm]:not([show-gt-sm]):not([show-md]):not([show]) {
    display: none;
  }
  [hide-md]:not([show-md]):not([show]) {
    display: none;
  }
  [flex-order-md="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-md="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-md="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-md="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-md="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-md="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-md="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-md="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-md="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-md="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-md="center"],
  [layout-align-md="center center"],
  [layout-align-md="center start"],
  [layout-align-md="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-md="end"],
  [layout-align-md="end center"],
  [layout-align-md="end start"],
  [layout-align-md="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-md="space-around"],
  [layout-align-md="space-around center"],
  [layout-align-md="space-around start"],
  [layout-align-md="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-md="space-between"],
  [layout-align-md="space-between center"],
  [layout-align-md="space-between start"],
  [layout-align-md="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-md="center center"],
  [layout-align-md="start center"],
  [layout-align-md="end center"],
  [layout-align-md="space-between center"],
  [layout-align-md="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-md="center start"],
  [layout-align-md="start start"],
  [layout-align-md="end start"],
  [layout-align-md="space-between start"],
  [layout-align-md="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-md="center end"],
  [layout-align-md="start end"],
  [layout-align-md="end end"],
  [layout-align-md="space-between end"],
  [layout-align-md="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-md] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-md=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-md=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-md="5"] {
    margin-left: 5%;
  }
  [offset-md="10"] {
    margin-left: 10%;
  }
  [offset-md="15"] {
    margin-left: 15%;
  }
  [offset-md="20"] {
    margin-left: 20%;
  }
  [offset-md="25"] {
    margin-left: 25%;
  }
  [offset-md="30"] {
    margin-left: 30%;
  }
  [offset-md="35"] {
    margin-left: 35%;
  }
  [offset-md="40"] {
    margin-left: 40%;
  }
  [offset-md="45"] {
    margin-left: 45%;
  }
  [offset-md="50"] {
    margin-left: 50%;
  }
  [offset-md="55"] {
    margin-left: 55%;
  }
  [offset-md="60"] {
    margin-left: 60%;
  }
  [offset-md="65"] {
    margin-left: 65%;
  }
  [offset-md="70"] {
    margin-left: 70%;
  }
  [offset-md="75"] {
    margin-left: 75%;
  }
  [offset-md="80"] {
    margin-left: 80%;
  }
  [offset-md="85"] {
    margin-left: 85%;
  }
  [offset-md="90"] {
    margin-left: 90%;
  }
  [offset-md="95"] {
    margin-left: 95%;
  }
  [offset-md="33"], [offset-md="34"] {
    margin-left: 33.33%;
  }
  [offset-md="66"], [offset-md="67"] {
    margin-left: 66.66%;
  }
  [flex-md] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-md="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-md="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-md="0"] {
    max-height: 0%;
  }
  [flex-md="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-md="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-md="5"] {
    max-height: 5%;
  }
  [flex-md="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-md="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-md="10"] {
    max-height: 10%;
  }
  [flex-md="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-md="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-md="15"] {
    max-height: 15%;
  }
  [flex-md="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-md="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-md="20"] {
    max-height: 20%;
  }
  [flex-md="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-md="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-md="25"] {
    max-height: 25%;
  }
  [flex-md="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-md="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-md="30"] {
    max-height: 30%;
  }
  [flex-md="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-md="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-md="35"] {
    max-height: 35%;
  }
  [flex-md="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-md="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-md="40"] {
    max-height: 40%;
  }
  [flex-md="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-md="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-md="45"] {
    max-height: 45%;
  }
  [flex-md="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-md="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-md="50"] {
    max-height: 50%;
  }
  [flex-md="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-md="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-md="55"] {
    max-height: 55%;
  }
  [flex-md="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-md="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-md="60"] {
    max-height: 60%;
  }
  [flex-md="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-md="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-md="65"] {
    max-height: 65%;
  }
  [flex-md="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-md="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-md="70"] {
    max-height: 70%;
  }
  [flex-md="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-md="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-md="75"] {
    max-height: 75%;
  }
  [flex-md="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-md="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-md="80"] {
    max-height: 80%;
  }
  [flex-md="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-md="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-md="85"] {
    max-height: 85%;
  }
  [flex-md="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-md="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-md="90"] {
    max-height: 90%;
  }
  [flex-md="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-md="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-md="95"] {
    max-height: 95%;
  }
  [flex-md="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-md="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-md="100"] {
    max-height: 100%;
  }
  [flex-md="33"], [flex-md="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-md="66"], [flex-md="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-md="33"], [layout="row"] > [flex-md="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-md="66"], [layout="row"] > [flex-md="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-md="33"], [layout="column"] > [flex-md="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-md="66"], [layout="column"] > [flex-md="67"] {
    max-height: 66.66%;
  }
}

@media (min-width: 960px) {
  [flex-order-gt-md="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-gt-md="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-gt-md="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-gt-md="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-gt-md="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-gt-md="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-gt-md="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-gt-md="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-gt-md="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-gt-md="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-gt-md="center"],
  [layout-align-gt-md="center center"],
  [layout-align-gt-md="center start"],
  [layout-align-gt-md="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-gt-md="end"],
  [layout-align-gt-md="end center"],
  [layout-align-gt-md="end start"],
  [layout-align-gt-md="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-gt-md="space-around"],
  [layout-align-gt-md="space-around center"],
  [layout-align-gt-md="space-around start"],
  [layout-align-gt-md="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-gt-md="space-between"],
  [layout-align-gt-md="space-between center"],
  [layout-align-gt-md="space-between start"],
  [layout-align-gt-md="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-gt-md="center center"],
  [layout-align-gt-md="start center"],
  [layout-align-gt-md="end center"],
  [layout-align-gt-md="space-between center"],
  [layout-align-gt-md="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-gt-md="center start"],
  [layout-align-gt-md="start start"],
  [layout-align-gt-md="end start"],
  [layout-align-gt-md="space-between start"],
  [layout-align-gt-md="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-gt-md="center end"],
  [layout-align-gt-md="start end"],
  [layout-align-gt-md="end end"],
  [layout-align-gt-md="space-between end"],
  [layout-align-gt-md="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-gt-md] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-gt-md=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-gt-md=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-gt-md="5"] {
    margin-left: 5%;
  }
  [offset-gt-md="10"] {
    margin-left: 10%;
  }
  [offset-gt-md="15"] {
    margin-left: 15%;
  }
  [offset-gt-md="20"] {
    margin-left: 20%;
  }
  [offset-gt-md="25"] {
    margin-left: 25%;
  }
  [offset-gt-md="30"] {
    margin-left: 30%;
  }
  [offset-gt-md="35"] {
    margin-left: 35%;
  }
  [offset-gt-md="40"] {
    margin-left: 40%;
  }
  [offset-gt-md="45"] {
    margin-left: 45%;
  }
  [offset-gt-md="50"] {
    margin-left: 50%;
  }
  [offset-gt-md="55"] {
    margin-left: 55%;
  }
  [offset-gt-md="60"] {
    margin-left: 60%;
  }
  [offset-gt-md="65"] {
    margin-left: 65%;
  }
  [offset-gt-md="70"] {
    margin-left: 70%;
  }
  [offset-gt-md="75"] {
    margin-left: 75%;
  }
  [offset-gt-md="80"] {
    margin-left: 80%;
  }
  [offset-gt-md="85"] {
    margin-left: 85%;
  }
  [offset-gt-md="90"] {
    margin-left: 90%;
  }
  [offset-gt-md="95"] {
    margin-left: 95%;
  }
  [offset-gt-md="33"], [offset-gt-md="34"] {
    margin-left: 33.33%;
  }
  [offset-gt-md="66"], [offset-gt-md="67"] {
    margin-left: 66.66%;
  }
  [flex-gt-md] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-gt-md="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-gt-md="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-gt-md="0"] {
    max-height: 0%;
  }
  [flex-gt-md="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-gt-md="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-gt-md="5"] {
    max-height: 5%;
  }
  [flex-gt-md="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-gt-md="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-gt-md="10"] {
    max-height: 10%;
  }
  [flex-gt-md="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-gt-md="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-gt-md="15"] {
    max-height: 15%;
  }
  [flex-gt-md="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-gt-md="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-gt-md="20"] {
    max-height: 20%;
  }
  [flex-gt-md="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-gt-md="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-gt-md="25"] {
    max-height: 25%;
  }
  [flex-gt-md="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-gt-md="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-gt-md="30"] {
    max-height: 30%;
  }
  [flex-gt-md="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-gt-md="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-gt-md="35"] {
    max-height: 35%;
  }
  [flex-gt-md="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-gt-md="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-gt-md="40"] {
    max-height: 40%;
  }
  [flex-gt-md="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-gt-md="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-gt-md="45"] {
    max-height: 45%;
  }
  [flex-gt-md="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-gt-md="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-gt-md="50"] {
    max-height: 50%;
  }
  [flex-gt-md="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-gt-md="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-gt-md="55"] {
    max-height: 55%;
  }
  [flex-gt-md="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-gt-md="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-gt-md="60"] {
    max-height: 60%;
  }
  [flex-gt-md="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-gt-md="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-gt-md="65"] {
    max-height: 65%;
  }
  [flex-gt-md="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-gt-md="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-gt-md="70"] {
    max-height: 70%;
  }
  [flex-gt-md="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-gt-md="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-gt-md="75"] {
    max-height: 75%;
  }
  [flex-gt-md="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-gt-md="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-gt-md="80"] {
    max-height: 80%;
  }
  [flex-gt-md="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-gt-md="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-gt-md="85"] {
    max-height: 85%;
  }
  [flex-gt-md="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-gt-md="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-gt-md="90"] {
    max-height: 90%;
  }
  [flex-gt-md="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-gt-md="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-gt-md="95"] {
    max-height: 95%;
  }
  [flex-gt-md="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-gt-md="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-gt-md="100"] {
    max-height: 100%;
  }
  [flex-gt-md="33"], [flex-gt-md="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-gt-md="66"], [flex-gt-md="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-gt-md="33"], [layout="row"] > [flex-gt-md="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-gt-md="66"], [layout="row"] > [flex-gt-md="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-gt-md="33"], [layout="column"] > [flex-gt-md="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-gt-md="66"], [layout="column"] > [flex-gt-md="67"] {
    max-height: 66.66%;
  }
}

@media (min-width: 960px) and (max-width: 1199px) {
  [hide]:not([show-gt-sm]):not([show-gt-md]):not([show-lg]):not([show]), [hide-gt-sm]:not([show-gt-sm]):not([show-gt-md]):not([show-lg]):not([show]), [hide-gt-md]:not([show-gt-sm]):not([show-gt-md]):not([show-lg]):not([show]) {
    display: none;
  }
  [hide-lg]:not([show-lg]):not([show]) {
    display: none;
  }
  [flex-order-lg="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-lg="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-lg="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-lg="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-lg="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-lg="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-lg="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-lg="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-lg="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-lg="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-lg="center"],
  [layout-align-lg="center center"],
  [layout-align-lg="center start"],
  [layout-align-lg="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-lg="end"],
  [layout-align-lg="end center"],
  [layout-align-lg="end start"],
  [layout-align-lg="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-lg="space-around"],
  [layout-align-lg="space-around center"],
  [layout-align-lg="space-around start"],
  [layout-align-lg="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-lg="space-between"],
  [layout-align-lg="space-between center"],
  [layout-align-lg="space-between start"],
  [layout-align-lg="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-lg="center center"],
  [layout-align-lg="start center"],
  [layout-align-lg="end center"],
  [layout-align-lg="space-between center"],
  [layout-align-lg="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-lg="center start"],
  [layout-align-lg="start start"],
  [layout-align-lg="end start"],
  [layout-align-lg="space-between start"],
  [layout-align-lg="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-lg="center end"],
  [layout-align-lg="start end"],
  [layout-align-lg="end end"],
  [layout-align-lg="space-between end"],
  [layout-align-lg="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-lg] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-lg=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-lg=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-lg="5"] {
    margin-left: 5%;
  }
  [offset-lg="10"] {
    margin-left: 10%;
  }
  [offset-lg="15"] {
    margin-left: 15%;
  }
  [offset-lg="20"] {
    margin-left: 20%;
  }
  [offset-lg="25"] {
    margin-left: 25%;
  }
  [offset-lg="30"] {
    margin-left: 30%;
  }
  [offset-lg="35"] {
    margin-left: 35%;
  }
  [offset-lg="40"] {
    margin-left: 40%;
  }
  [offset-lg="45"] {
    margin-left: 45%;
  }
  [offset-lg="50"] {
    margin-left: 50%;
  }
  [offset-lg="55"] {
    margin-left: 55%;
  }
  [offset-lg="60"] {
    margin-left: 60%;
  }
  [offset-lg="65"] {
    margin-left: 65%;
  }
  [offset-lg="70"] {
    margin-left: 70%;
  }
  [offset-lg="75"] {
    margin-left: 75%;
  }
  [offset-lg="80"] {
    margin-left: 80%;
  }
  [offset-lg="85"] {
    margin-left: 85%;
  }
  [offset-lg="90"] {
    margin-left: 90%;
  }
  [offset-lg="95"] {
    margin-left: 95%;
  }
  [offset-lg="33"], [offset-lg="34"] {
    margin-left: 33.33%;
  }
  [offset-lg="66"], [offset-lg="67"] {
    margin-left: 66.66%;
  }
  [flex-lg] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-lg="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-lg="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-lg="0"] {
    max-height: 0%;
  }
  [flex-lg="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-lg="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-lg="5"] {
    max-height: 5%;
  }
  [flex-lg="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-lg="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-lg="10"] {
    max-height: 10%;
  }
  [flex-lg="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-lg="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-lg="15"] {
    max-height: 15%;
  }
  [flex-lg="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-lg="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-lg="20"] {
    max-height: 20%;
  }
  [flex-lg="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-lg="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-lg="25"] {
    max-height: 25%;
  }
  [flex-lg="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-lg="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-lg="30"] {
    max-height: 30%;
  }
  [flex-lg="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-lg="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-lg="35"] {
    max-height: 35%;
  }
  [flex-lg="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-lg="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-lg="40"] {
    max-height: 40%;
  }
  [flex-lg="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-lg="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-lg="45"] {
    max-height: 45%;
  }
  [flex-lg="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-lg="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-lg="50"] {
    max-height: 50%;
  }
  [flex-lg="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-lg="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-lg="55"] {
    max-height: 55%;
  }
  [flex-lg="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-lg="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-lg="60"] {
    max-height: 60%;
  }
  [flex-lg="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-lg="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-lg="65"] {
    max-height: 65%;
  }
  [flex-lg="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-lg="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-lg="70"] {
    max-height: 70%;
  }
  [flex-lg="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-lg="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-lg="75"] {
    max-height: 75%;
  }
  [flex-lg="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-lg="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-lg="80"] {
    max-height: 80%;
  }
  [flex-lg="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-lg="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-lg="85"] {
    max-height: 85%;
  }
  [flex-lg="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-lg="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-lg="90"] {
    max-height: 90%;
  }
  [flex-lg="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-lg="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-lg="95"] {
    max-height: 95%;
  }
  [flex-lg="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-lg="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-lg="100"] {
    max-height: 100%;
  }
  [flex-lg="33"], [flex-lg="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-lg="66"], [flex-lg="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-lg="33"], [layout="row"] > [flex-lg="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-lg="66"], [layout="row"] > [flex-lg="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-lg="33"], [layout="column"] > [flex-lg="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-lg="66"], [layout="column"] > [flex-lg="67"] {
    max-height: 66.66%;
  }
}

@media (min-width: 1200px) {
  [hide-gt-sm]:not([show-gt-sm]):not([show-gt-md]):not([show-gt-lg]):not([show]), [hide-gt-md]:not([show-gt-sm]):not([show-gt-md]):not([show-gt-lg]):not([show]), [hide-gt-lg]:not([show-gt-sm]):not([show-gt-md]):not([show-gt-lg]):not([show]), [hide]:not([show-gt-sm]):not([show-gt-md]):not([show-gt-lg]):not([show]) {
    display: none;
  }
  [flex-order-gt-lg="0"] {
    -webkit-box-ordinal-group: 1;
        -ms-flex-order: 0;
            order: 0;
  }
  [flex-order-gt-lg="1"] {
    -webkit-box-ordinal-group: 2;
        -ms-flex-order: 1;
            order: 1;
  }
  [flex-order-gt-lg="2"] {
    -webkit-box-ordinal-group: 3;
        -ms-flex-order: 2;
            order: 2;
  }
  [flex-order-gt-lg="3"] {
    -webkit-box-ordinal-group: 4;
        -ms-flex-order: 3;
            order: 3;
  }
  [flex-order-gt-lg="4"] {
    -webkit-box-ordinal-group: 5;
        -ms-flex-order: 4;
            order: 4;
  }
  [flex-order-gt-lg="5"] {
    -webkit-box-ordinal-group: 6;
        -ms-flex-order: 5;
            order: 5;
  }
  [flex-order-gt-lg="6"] {
    -webkit-box-ordinal-group: 7;
        -ms-flex-order: 6;
            order: 6;
  }
  [flex-order-gt-lg="7"] {
    -webkit-box-ordinal-group: 8;
        -ms-flex-order: 7;
            order: 7;
  }
  [flex-order-gt-lg="8"] {
    -webkit-box-ordinal-group: 9;
        -ms-flex-order: 8;
            order: 8;
  }
  [flex-order-gt-lg="9"] {
    -webkit-box-ordinal-group: 10;
        -ms-flex-order: 9;
            order: 9;
  }
  [layout-align-gt-lg="center"],
  [layout-align-gt-lg="center center"],
  [layout-align-gt-lg="center start"],
  [layout-align-gt-lg="center end"] {
    -webkit-box-pack: center;
        -ms-flex-pack: center;
            justify-content: center;
  }
  [layout-align-gt-lg="end"],
  [layout-align-gt-lg="end center"],
  [layout-align-gt-lg="end start"],
  [layout-align-gt-lg="end end"] {
    -webkit-box-pack: end;
        -ms-flex-pack: end;
            justify-content: flex-end;
  }
  [layout-align-gt-lg="space-around"],
  [layout-align-gt-lg="space-around center"],
  [layout-align-gt-lg="space-around start"],
  [layout-align-gt-lg="space-around end"] {
    -ms-flex-pack: distribute;
        justify-content: space-around;
  }
  [layout-align-gt-lg="space-between"],
  [layout-align-gt-lg="space-between center"],
  [layout-align-gt-lg="space-between start"],
  [layout-align-gt-lg="space-between end"] {
    -webkit-box-pack: justify;
        -ms-flex-pack: justify;
            justify-content: space-between;
  }
  [layout-align-gt-lg="center center"],
  [layout-align-gt-lg="start center"],
  [layout-align-gt-lg="end center"],
  [layout-align-gt-lg="space-between center"],
  [layout-align-gt-lg="space-around center"] {
    -webkit-box-align: center;
        -ms-flex-align: center;
            align-items: center;
  }
  [layout-align-gt-lg="center start"],
  [layout-align-gt-lg="start start"],
  [layout-align-gt-lg="end start"],
  [layout-align-gt-lg="space-between start"],
  [layout-align-gt-lg="space-around start"] {
    -webkit-box-align: start;
        -ms-flex-align: start;
            align-items: flex-start;
  }
  [layout-align-gt-lg="center end"],
  [layout-align-gt-lg="start end"],
  [layout-align-gt-lg="end end"],
  [layout-align-gt-lg="space-between end"],
  [layout-align-gt-lg="space-around end"] {
    -webkit-box-align: end;
        -ms-flex-align: end;
            align-items: flex-end;
  }
  [layout-gt-lg] {
    box-sizing: border-box;
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
  }
  [layout-gt-lg=column] {
    -webkit-box-orient: vertical;
    -webkit-box-direction: normal;
        -ms-flex-direction: column;
            flex-direction: column;
  }
  [layout-gt-lg=row] {
    -webkit-box-orient: horizontal;
    -webkit-box-direction: normal;
        -ms-flex-direction: row;
            flex-direction: row;
  }
  [offset-gt-lg="5"] {
    margin-left: 5%;
  }
  [offset-gt-lg="10"] {
    margin-left: 10%;
  }
  [offset-gt-lg="15"] {
    margin-left: 15%;
  }
  [offset-gt-lg="20"] {
    margin-left: 20%;
  }
  [offset-gt-lg="25"] {
    margin-left: 25%;
  }
  [offset-gt-lg="30"] {
    margin-left: 30%;
  }
  [offset-gt-lg="35"] {
    margin-left: 35%;
  }
  [offset-gt-lg="40"] {
    margin-left: 40%;
  }
  [offset-gt-lg="45"] {
    margin-left: 45%;
  }
  [offset-gt-lg="50"] {
    margin-left: 50%;
  }
  [offset-gt-lg="55"] {
    margin-left: 55%;
  }
  [offset-gt-lg="60"] {
    margin-left: 60%;
  }
  [offset-gt-lg="65"] {
    margin-left: 65%;
  }
  [offset-gt-lg="70"] {
    margin-left: 70%;
  }
  [offset-gt-lg="75"] {
    margin-left: 75%;
  }
  [offset-gt-lg="80"] {
    margin-left: 80%;
  }
  [offset-gt-lg="85"] {
    margin-left: 85%;
  }
  [offset-gt-lg="90"] {
    margin-left: 90%;
  }
  [offset-gt-lg="95"] {
    margin-left: 95%;
  }
  [offset-gt-lg="33"], [offset-gt-lg="34"] {
    margin-left: 33.33%;
  }
  [offset-gt-lg="66"], [offset-gt-lg="67"] {
    margin-left: 66.66%;
  }
  [flex-gt-lg] {
    box-sizing: border-box;
    -webkit-box-flex: 1;
        -ms-flex: 1;
            flex: 1;
  }
  [flex-gt-lg="0"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 0%;
            flex: 0 0 0%;
  }
  [layout="row"] > [flex-gt-lg="0"] {
    max-width: 0%;
  }
  [layout="column"] > [flex-gt-lg="0"] {
    max-height: 0%;
  }
  [flex-gt-lg="5"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 5%;
            flex: 0 0 5%;
  }
  [layout="row"] > [flex-gt-lg="5"] {
    max-width: 5%;
  }
  [layout="column"] > [flex-gt-lg="5"] {
    max-height: 5%;
  }
  [flex-gt-lg="10"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 10%;
            flex: 0 0 10%;
  }
  [layout="row"] > [flex-gt-lg="10"] {
    max-width: 10%;
  }
  [layout="column"] > [flex-gt-lg="10"] {
    max-height: 10%;
  }
  [flex-gt-lg="15"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 15%;
            flex: 0 0 15%;
  }
  [layout="row"] > [flex-gt-lg="15"] {
    max-width: 15%;
  }
  [layout="column"] > [flex-gt-lg="15"] {
    max-height: 15%;
  }
  [flex-gt-lg="20"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 20%;
            flex: 0 0 20%;
  }
  [layout="row"] > [flex-gt-lg="20"] {
    max-width: 20%;
  }
  [layout="column"] > [flex-gt-lg="20"] {
    max-height: 20%;
  }
  [flex-gt-lg="25"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 25%;
            flex: 0 0 25%;
  }
  [layout="row"] > [flex-gt-lg="25"] {
    max-width: 25%;
  }
  [layout="column"] > [flex-gt-lg="25"] {
    max-height: 25%;
  }
  [flex-gt-lg="30"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 30%;
            flex: 0 0 30%;
  }
  [layout="row"] > [flex-gt-lg="30"] {
    max-width: 30%;
  }
  [layout="column"] > [flex-gt-lg="30"] {
    max-height: 30%;
  }
  [flex-gt-lg="35"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 35%;
            flex: 0 0 35%;
  }
  [layout="row"] > [flex-gt-lg="35"] {
    max-width: 35%;
  }
  [layout="column"] > [flex-gt-lg="35"] {
    max-height: 35%;
  }
  [flex-gt-lg="40"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 40%;
            flex: 0 0 40%;
  }
  [layout="row"] > [flex-gt-lg="40"] {
    max-width: 40%;
  }
  [layout="column"] > [flex-gt-lg="40"] {
    max-height: 40%;
  }
  [flex-gt-lg="45"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 45%;
            flex: 0 0 45%;
  }
  [layout="row"] > [flex-gt-lg="45"] {
    max-width: 45%;
  }
  [layout="column"] > [flex-gt-lg="45"] {
    max-height: 45%;
  }
  [flex-gt-lg="50"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 50%;
            flex: 0 0 50%;
  }
  [layout="row"] > [flex-gt-lg="50"] {
    max-width: 50%;
  }
  [layout="column"] > [flex-gt-lg="50"] {
    max-height: 50%;
  }
  [flex-gt-lg="55"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 55%;
            flex: 0 0 55%;
  }
  [layout="row"] > [flex-gt-lg="55"] {
    max-width: 55%;
  }
  [layout="column"] > [flex-gt-lg="55"] {
    max-height: 55%;
  }
  [flex-gt-lg="60"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 60%;
            flex: 0 0 60%;
  }
  [layout="row"] > [flex-gt-lg="60"] {
    max-width: 60%;
  }
  [layout="column"] > [flex-gt-lg="60"] {
    max-height: 60%;
  }
  [flex-gt-lg="65"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 65%;
            flex: 0 0 65%;
  }
  [layout="row"] > [flex-gt-lg="65"] {
    max-width: 65%;
  }
  [layout="column"] > [flex-gt-lg="65"] {
    max-height: 65%;
  }
  [flex-gt-lg="70"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 70%;
            flex: 0 0 70%;
  }
  [layout="row"] > [flex-gt-lg="70"] {
    max-width: 70%;
  }
  [layout="column"] > [flex-gt-lg="70"] {
    max-height: 70%;
  }
  [flex-gt-lg="75"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 75%;
            flex: 0 0 75%;
  }
  [layout="row"] > [flex-gt-lg="75"] {
    max-width: 75%;
  }
  [layout="column"] > [flex-gt-lg="75"] {
    max-height: 75%;
  }
  [flex-gt-lg="80"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 80%;
            flex: 0 0 80%;
  }
  [layout="row"] > [flex-gt-lg="80"] {
    max-width: 80%;
  }
  [layout="column"] > [flex-gt-lg="80"] {
    max-height: 80%;
  }
  [flex-gt-lg="85"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 85%;
            flex: 0 0 85%;
  }
  [layout="row"] > [flex-gt-lg="85"] {
    max-width: 85%;
  }
  [layout="column"] > [flex-gt-lg="85"] {
    max-height: 85%;
  }
  [flex-gt-lg="90"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 90%;
            flex: 0 0 90%;
  }
  [layout="row"] > [flex-gt-lg="90"] {
    max-width: 90%;
  }
  [layout="column"] > [flex-gt-lg="90"] {
    max-height: 90%;
  }
  [flex-gt-lg="95"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 95%;
            flex: 0 0 95%;
  }
  [layout="row"] > [flex-gt-lg="95"] {
    max-width: 95%;
  }
  [layout="column"] > [flex-gt-lg="95"] {
    max-height: 95%;
  }
  [flex-gt-lg="100"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 100%;
            flex: 0 0 100%;
  }
  [layout="row"] > [flex-gt-lg="100"] {
    max-width: 100%;
  }
  [layout="column"] > [flex-gt-lg="100"] {
    max-height: 100%;
  }
  [flex-gt-lg="33"], [flex-gt-lg="34"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 33.33%;
            flex: 0 0 33.33%;
  }
  [flex-gt-lg="66"], [flex-gt-lg="67"] {
    -webkit-box-flex: 0;
        -ms-flex: 0 0 66.66%;
            flex: 0 0 66.66%;
  }
  [layout="row"] > [flex-gt-lg="33"], [layout="row"] > [flex-gt-lg="34"] {
    max-width: 33.33%;
  }
  [layout="row"] > [flex-gt-lg="66"], [layout="row"] > [flex-gt-lg="67"] {
    max-width: 66.66%;
  }
  [layout="column"] > [flex-gt-lg="33"], [layout="column"] > [flex-gt-lg="34"] {
    max-height: 33.33%;
  }
  [layout="column"] > [flex-gt-lg="66"], [layout="column"] > [flex-gt-lg="67"] {
    max-height: 66.66%;
  }
}

```

## Author

Jason Melgoza

## License

MIT
