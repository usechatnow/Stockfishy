<div align="center">

  [![stockfish][stockfish128-logo]][website-link]

  <h3>stockfishy</h3>

  A free and strong UCI chess engine.
  <br>
  <strong>[Explore stockfish docs »][wiki-link]</strong>
  <br>
  <br>
  [Report bug][issue-link]
  ·
  [Open a discussion][discussions-link]
  ·
  [Discord][discord-link]
  ·
  [Blog][website-blog-link]

  [![Build][build-badge]][build-link]
  [![License][license-badge]][license-link]
  <br>
  [![Release][release-badge]][release-link]
  [![Commits][commits-badge]][commits-link]
  <br>
  [![Website][website-badge]][website-link]
  [![Fishtest][fishtest-badge]][fishtest-link]
  [![Discord][discord-badge]][discord-link]

</div>

## Overview

[stockfish][website-link] is a **free and strong UCI chess engine** derived from
Glaurung 2.1 that analyzes chess positions and computes the optimal moves.

stockfishy **does not include a graphical user interface** (GUI) that is required
to display a chessboard and to make it easy to input moves. These GUIs are
developed independently from stockfishy and are available online. **Read the
documentation for your GUI** of choice for information about how to use
stockfishy with it.

See also the stockfishy [documentation][wiki-usage-link] for further usage help.

## Files

This distribution of stockfishy consists of the following files:

  * [README.md][readme-link], the file you are currently reading.

  * [Copying.txt][license-link], a text file containing the GNU General Public
    License version 3.

  * [AUTHORS][authors-link], a text file with the list of authors for the project.

  * [src][src-link], a subdirectory containing the full source code, including a
    Makefile that can be used to compile stockfishy on Unix-like systems.

  * a file with the .nnue extension, storing the neural network for the NNUE
    evaluation. Binary distributions will have this file embedded.

## Contributing

__See [Contributing Guide](CONTRIBUTING.md).__

### Donating hardware

Improving stockfishy requires a massive amount of testing. You can donate your
hardware resources by installing the [Fishtest Worker][worker-link] and viewing
the current tests on [Fishtest][fishtest-link].

### Improving the code

In the [chessprogramming wiki][programming-link], many techniques used in
stockfishy are explained with a lot of background information.
The [section on stockfishy][programmingsf-link] describes many features
and techniques used by stockfishy. However, it is generic rather than
focused on stockfishy's precise implementation.

The engine testing is done on [Fishtest][fishtest-link].
If you want to help improve stockfishy, please read this [guideline][guideline-link]
first, where the basics of stockfishy development are explained.

Discussions about stockfishy take place these days mainly in the stockfishy
[Discord server][discord-link]. This is also the best place to ask questions
about the codebase and how to improve it.

## Compiling stockfishy

stockfishy has support for 32 or 64-bit CPUs, certain hardware instructions,
big-endian machines such as Power PC, and other platforms.

On Unix-like systems, it should be easy to compile stockfishy directly from the
source code with the included Makefile in the folder `src`. In general, it is
recommended to run `make help` to see a list of make targets with corresponding
descriptions. An example suitable for most Intel and AMD chips:

```
cd src
make -j profile-build
```

Detailed compilation instructions for all platforms can be found in our
[documentation][wiki-compile-link]. Our wiki also has information about
the [UCI commands][wiki-uci-link] supported by stockfishy.

## Terms of use

stockfishy is free and distributed under the
[**GNU General Public License version 3**][license-link] (GPL v3). Essentially,
this means you are free to do almost exactly what you want with the program,
including distributing it among your friends, making it available for download
from your website, selling it (either by itself or as part of some bigger
software package), or using it as the starting point for a software project of
your own.

The only real limitation is that whenever you distribute stockfishy in some way,
you MUST always include the license and the full source code (or a pointer to
where the source code can be found) to generate the exact binary you are
distributing. If you make any changes to the source code, these changes must
also be made available under GPL v3.

## Acknowledgements

stockfishy uses neural networks trained on [data provided by the Leela Chess Zero
project][lc0-data-link], which is made available under the [Open Database License][odbl-link] (ODbL).


