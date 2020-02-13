# git_tut
testli


'If Not value.EndsWith(New Char() {" "c}) Then value = value + "  "
                    'TBE 11/09/2019: replacing line above because:
                    ' In "ItemNumber 12" we face 80 characters, but this string should be exactly 79 characters long.
                    'The last 3 characters (77. to 79.) are representing the type of the document ...
                    '(In this case we have "HV" And therefore we only need one more space at the end of the string, but we have two in the XML.)
                    'new rule: The QR Code is exactly 79 characters long and we should fill up with spaces until we have exactly 79 characters.
                    While value.Length < 79
                        value = value + " "
                    End While