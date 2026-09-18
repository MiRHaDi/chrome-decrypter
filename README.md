# chrome-decrypter (legacy)

Historical Windows/Python code for reading saved Chrome credentials. The existing
Pipfile targets Python 3.6; compatibility with current Python, Windows, and Chrome
has not been verified. This repository should not be treated as a supported
password-recovery utility.

## Access your own saved passwords

Use [Google Password Manager in Chrome](https://support.google.com/chrome/answer/95606)
to view and manage your passwords, or follow Google's official
[import/export instructions](https://support.google.com/chrome/answer/13068232).
An exported password file contains plaintext secrets: keep it private and remove
it after the intended import. Do not add exported data to this repository.

## Repository status

- The historical source is `chrome_decrypt.py`; this maintenance change does not
  alter its extraction logic or add support for newer browser protection schemes.
- `Pipfile` and `Pipfile.lock` describe the historical environment. They are retained
  for provenance, not as a recommendation to install Python 3.6 today.
- The checked-in executable has been removed from the current tree. Its provenance
  and behavior were not verified in this maintenance pass; old Git commits still
  contain it. No executable was run to review this change.
- Generated executables, build directories, virtual environments, and typical
  credential exports are excluded from future commits via `.gitignore`.

There is no current runtime compatibility claim or supported binary release.
