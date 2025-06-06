
* Fix Tgls on Windows + MingW64
  * Try to load [opengl32.dll] at startup on Windows.
  * Bring 64-bit Windows support by fixing selection of FFI ABI.
  * Unlock the full OpenGL API on Windows by implementing indirect
    procedure lookup with [wglGetProcAddress].
* Fix build system. Explicitely depend on `ctypes-foreign`. 
  Thanks to Etienne Millon for the patch (#29).
* Fix `Gl.debug_message_callback` raising `Ffi_stubs.CallToExpiredClosure`. 
  Thanks to Edwin Török for the report and the patch (#6).


v0.8.6 2022-02-10 La Forclaz (VS)
---------------------------------

* Handle `Pervasives` deprecation (and thus support OCaml 5.00).

v0.8.5 2016-11-25 Zagreb
------------------------

* Allow to optionally build GL and GL ES. Thanks to Peter Zotov for
  the patch.


v0.8.4 2016-06-03 Cambridge (UK)
-------------------------------

* Support for OpenGL ES 3.2
* Safe string support.
* Fix build on 32-bit platforms.
* Build system: allow to override host platform.
* Build system: rpi3 support.
* Untested Windows support.
* FreeBSD support. Thanks to Alexander Diemand for the help.
* Build depend on topkg.
* Relicensed from BSD3 to ISC.


v0.8.3 2015-03-15 La Forclaz (VS)
---------------------------------

Support for ctypes 0.4.0. Thanks to Peter Zotov for the patch. ctypes
switches from int64 to nativeint for representing pointers. This
impacts a few function signatures that change accordingly.


v0.8.2 2014-08-14 Cambridge (UK)
--------------------------------

Support for OpenGL 4.5 and OpenGL ES 3.1.


v0.8.1 2014-05-22 La Forclaz (VS)
---------------------------------

Support for ctypes 0.3. Thanks to Jeremy Yallop for the patch.


v0.8.0 2014-05-18 La Forclaz (VS)
---------------------------------

First release.
