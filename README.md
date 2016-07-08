## Template_formatting_system

###Example input:

<pre>
!name1=John Q.
!name2=Smith
!salutation=Dear @name1 @name2
1 Infinite Loop
!product=Horcrux Widget
Somewheresville, CA 98765


@salutation,


Thank you for your interest in @{product}s.
Unfortunately, we sold our last @product yesterday.


@name1, if you have any more questions about our products,
email us at support@@horcrux.com, tweet to @@horcrux_support,
or call us @@ 1-800-HORCRUX.
</pre>

###System should generate the following output:
<pre>
1 Infinite Loop
Somewheresville, CA 98765


Dear John Q. Smith,


Thank you for your interest in Horcrux Widgets.
Unfortunately, we sold our last Horcrux Widget yesterday.


John Q., if you have any more questions about our products,
email us at support@horcrux.com, tweet to @horcrux_support,
or call us @ 1-800-HORCRUX.
</pre>
