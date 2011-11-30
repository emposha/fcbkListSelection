=======================
 fcbkListSelection 1.10
=======================
fcbkListSelection is a fancy item selector, just like the friends selector you can see on Facebook.
It is built with jQuery javascript framework, with wide range of options.
You can check out the Demo `here <http://www.emposha.com/demo/fcbklistselection/>`_.

- supported Jquery versions: 1.2.x, 1.3.x, 1.4.x
 
Changelog:

- 1.1: added preselected items
- 1.0: project started

Coded by: emposha <admin@emposha.com>

Copyright: `Emposha.com <http://www.emposha.com>`_

License: Distributed under MIT license

-----------
HTML Markup
-----------

The html pattern required for this plugin to work is (see index.html):

    <ul id="fcbklist">
        <li>        
            <strong>Manuel Mujica Lainez</strong><br /> 
            <span class="fcbkitem_text">auto complete & pre added values.</span>
            <input type="hidden" name="fcbklist_value[]" value="Manuel Mujica Lainez" />       
        </li>
        <li>        
            <strong>Gustavo Nielsen</strong><br />
            <span class="fcbkitem_text">If you have any comments or requests, please post them and</span>
            <input type="hidden" name="fcbklist_value[]" value="Gustavo Nielsen" />         
        </li> 
        [...]    
    </ul>

----------------
Javascript usage
----------------

In <script> tag, put:

    $(document).ready(function() {
      $.fcbkListSelection(elem, width, height, row);
    });

Options are:

- `elem`: ul element id or object
- `width`: width of ul
- `height`: height of each element
- `row`: number of items in row


For example: 

    $.fcbkListSelection("#fcbklist", 400, 50, 2);