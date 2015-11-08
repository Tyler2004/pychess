# About #

This format has two main purposes:
  * Lets the client know which chess engines are installed, and where to look for them.
  * Cache and work as data model for engine information that would otherwise slow client at run time to discover.

There is currently no such thing as a 

&lt;level&gt;

 element as I believe it makes more sense to put that kind of stuff in the protocol handling code. Instead we cache engines supported commands, so that we know if e.g. the uci engines supports the UCI\_LimitStrength option, or if we should rather use "go depth" to variate playing strength.

# Example #
```
<engines>
    <engine protocol="cecp">
        <path>/usr/bin/gnuchess</path>
        <argument>--xboard</argument>
        <binname>gnuchess</binname>
        <md5>bee39e0ac125b46a8ce0840507dde50e</md5>
        <name>GNU Chess 5.07</name>
        <cecp-info>
            <supports command="setboard" supports="true" />
            <supports command="edit" supports="false" />
            <supports command="protover 2" supports="true" />
            <supports command="analyze" supports="true" />
            <supports command="sd" supports="false" />
            <supports command="depth" supports="true" />
        </cecp-info>
    </engine>
    
    <engine protocol="uci">
        <path>/usr/bin/fruit_21_static</path>
        <argument></argument>
        <binname>fruit_21_static</binname>
        <md5>34378c3de14d16f92ca30c34ed4fa5ca</md5>
        <name>Fruit 2.1</name>
        <uci-ids>
            <id name="name" value="Fruit 2.1" />
            <id name="author" value="Fabien Letouzey" />
        </uci-ids>
        <uci-options>
            <spin-option name="Hash" min="4" max="1024" default="16" />
            <check-option name="Ponder" default="false" />
            <combo-option name="NullMove Pruning" default="Fail High">
                <var value="Always" />
                <var value="Fail High" />
                <var value="Never" />
            </combo-option>
            <string-option name="BookFile" default="book_small.bin" />
            <button-option name="Fruit has no buttons" />
        </uci-options>
    </engine>
</engines>
```

# Document Type Definition (DTD) #

TODO