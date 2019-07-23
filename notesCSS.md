# notes

## Sometimes anchor tag not landing in the coreect place, the best way to solve is that add another class, display as blcok, 
## then adjust padding-top and margin-top with same number, but padding go positive, and margin go negative

## Since ul and li elements are display: block by default — give them auto margins and a width that is smaller than their container.
### ul {
    width: 70%;
    margin: auto;
### }

### For centering a block of text 
### just need to give that block a width, then margin-left and right all be auto.

### to make a button vertically and horizontally center 
< id="wrapper">
  <button type="button">hello</button>
</>

#wrapper {
  width: 100%;
  height: 400px;
  border: 1px solid black;
  display: flex;
  align-items: center;
  justify-content: center;
}

button {
  height: 20px;
  width: 100px;
}

## About flexbox, when use flex box, text-align; float; clear and vertical-align will not working.
