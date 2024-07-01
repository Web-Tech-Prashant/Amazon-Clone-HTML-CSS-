1. Cascading?
sol: Cascading comes from 1st word of CSS(Cascading style sheet).
    

2. how Cascading works?
sol: Suppose we are using <h1> tag element and apply css twice on same tag then it will take the last applied css.
     e.g:
            <style>
                h1{
                    color:red;
                }
                h1{
                    color:blue;
                }
            </style>
           <h1>This is Header</h1>

           Note: In the above eg. blue color will apply on h1 tag.

3. what is Specificity?
sol: In css each selector is given some specificity like, 
         h1 -> 0001 (thousand, hundred, tens, ones)

         Note: it will check the specifity and it will apply based on high specificity.

         Reference: css-tricks.com/specific-on-css-specificity

4. Which type of style has high priority?
sol:  1st priority-> inline style
      2nd and 3rd priority-> It depends how it is declared in <head> tag i.e on ordering. whoever comes last will have 2nd priority and so on..
      e.g: 
      <html>
      <head>
      <style>
        <link rel="stylesheet" href="styles.css">
        <style>
         h2{
            color:blue;
         }
        </style>
        </style>
      </head>
      </html>

      Note: in the above e.g, style will have highest priority and then link.