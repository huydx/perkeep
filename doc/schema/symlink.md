# Symlink Schema

    {"camliVersion": 1,
     "camliType": "symlink",

      //
      // INCLUDE ALL REQUIRED & ANY OPTIONAL FIELDS FROM common.md
      //

      // Exactly one of:

      // If UTF-8:
      "symlinkTarget": "../foo/blah",

      // If unknown charset & have raw 8-bit filenames and can't convert
      // to UTF-8.  The array is a mix of UTF-8 and/or non-UTF-8 bytes (0-255).
      "symlinkTargetBytes": ["../foo/Am", 233, "lie.jpg"],  // e.g. Amélie in ISO-8859-1 when charset unknown
    }
