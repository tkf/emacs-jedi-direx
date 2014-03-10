=================================================
 Tree style source code viewer for Python buffer
=================================================

You can view Python code (right) in a tree style viewer (left):

.. image:: http://farm4.staticflickr.com/3784/8804246558_0b3c998050_o.png
   :target: http://www.flickr.com/photos/arataka/8804246558/

TODO: make it installable via el-get and MELPA.


Setup
=====
Example to open the viewer by `C-c x` in Python buffer::

  (eval-after-load "python"
    '(define-key python-mode-map "\C-cx" 'jedi-direx:pop-to-buffer))
  (add-hook 'jedi-mode-hook 'jedi-direx:setup)


Requirements
============

- `jedi.el <http://tkf.github.io/emacs-jedi/>`_
- `direx.el <https://github.com/m2ym/direx-el>`_
