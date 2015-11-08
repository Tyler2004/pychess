# Example #

```
<chesstheme>
    <meta>
        <name>Candy</name>
        <version>0.5</version>
        <author name="J. Random" email="j@random.com" http="..." />
        <note>
            Bla...
        </note>
    </meta>
    <board>
        <!-- This can contain the cordinates build into the background img -->
        <!-- I think it would be cool if not squared cords e.g. round cords
             were supported. This would require a way to dertimine which cord
             has been clicked -->
    </board>
    <clock>
        <!-- ? -->
    </clock>
    <piece>
        <white>
            <king path="whiteking.png" />
            <queen path="whitequeen.png" />
            <bishop path="whitebishop.png" />
            <knight path="whiteknight.png" />
            <rook path="whiterook.png" />
            <pawn path="whitepawn.png" />
        </white>
        <black>
            <king path="blackking.png" />
            <queen path="blackqueen.png" />
            <bishop path="blackbishop.png" />
            <knight path="blackknight.png" />
            <rook path="blackrook.png" />
            <pawn path="blackpawn.png" />
        </black>
    </piece>
    <sound>
        <checkmate type="beep" />
        <check type="mute" />
        <piecemove type="sound" path="dak.ogg" />
        ...
    </sound>
</chesstheme>
```

# Document Type Definition (DTD) #

TODO
