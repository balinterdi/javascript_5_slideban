!SLIDE

# Körültekintő #

    alert("Ezt nem kellett volna")

!SLIDE incremental transition=fade

# Udvarias #

    confirm("Bocs, de télleg?")

!SLIDE incremental transition=fade

# Barátságos #

    update: (function(){

      // see: http://support.microsoft.com/kb/276228
      var SELECT_ELEMENT_INNERHTML_BUGGY = (function(){
        var el = document.createElement("select"),
            isBuggy = true;
        el.innerHTML = "<option value=\"test\">test</option>";
        if (el.options && el.options[0]) {
          isBuggy = el.options[0].nodeName.toUpperCase() !== "OPTION";
        }
        el = null;
        return isBuggy;
      })();
      ...
    })

!SLIDE incremental transition=fade

# Konzekvens #

    '' == '0' // false
    0 == ''   // true
    0 == '0'  // true

!SLIDE incremental transition=fade

# Kiismerhető #

    <script language="JavaScript" type="text/javascript">
    /* <![CDATA[ */
    // content of your Javascript goes here
    /* ]]> */
    </script>