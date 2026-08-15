# SatisfactoryModLoader [![CI](https://github.com/satisfactorymodding/SatisfactoryModLoader/actions/workflows/build.yml/badge.svg)](https://github.com/satisfactorymodding/SatisfactoryModLoader/actions/workflows/build.yml)

A tool used to load mods for the game Satisfactory. After Coffee Stain releases a proper Unreal modding API the project will continue as a utilities library.

This repository contains the SatisfactoryModLoader source code,
an ExampleMod with demos of some of the SML utilities,
a collection of editor utilities,
and more.
It also serves as the Unreal project used for developing mods.

## Documentation

Learn how to set up and use this repo on the [modding documentation](https://docs.ficsit.app/).

## Discord Server

Join our [discord server](https://discord.gg/QzcG9nX) to talk about SML and Satisfactory Modding in general.

## Security note for this fork

Earlier commits in this repository (before the cleanup in PR #1) contained a
hardcoded Epic Online Services `ClientSecret` and an `AndroidFileServer`
`SecurityToken`. The current tree uses `$(EOS_CLIENT_SECRET)` references and no
longer stores these values in `Config/DefaultEngine.ini`, but the old secrets
remain reachable in the Git history.

If you build from this fork, generate **fresh** credentials in the Epic
Developer Portal and supply `EOS_CLIENT_SECRET` at build/deploy time. Do not
reuse any values found in older commits or forks.

## DISCLAIMER

This software is provided by the author "as is". In no event shall the author be liable for any direct, indirect, incidental, special, exemplary, or consequential damages (including, but not limited to procurement of substitute goods or services; loss of use, data, or profits; or business interruption) however caused and on any
theory of liability, whether in contract, strict liability, or tort (including negligence or otherwise) arising in any way out of the use of this software, even if advised of the possibility of such damage.
