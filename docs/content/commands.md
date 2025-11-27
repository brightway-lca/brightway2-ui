# Commands

The tool speaks fluent command-line. Below is its full vocabulary, arranged by mood and mission. When in doubt, remember that commands are lower-case, arguments go after a space, and sarcasm is optional but encouraged.

## Basic Commands

- `?` / `help` – Prints the built-in help text. Think of it as the in-app fortune cookie.
- `autosave` – Toggles autosave of your last project/database/activity. Perfect for the indecisive.
- `number` – When shown a list, type its number to jump straight there. Spatial navigation for impatient humans.
- `l` – Re-list the current options when you've scrolled past oblivion.
- `n` – Next page of options. No swiping required.
- `p` / `p <page>` – Previous page or jump directly to `page`. Because guessing isn't fun.
- `h` – Shows recent history of selected projects, databases, and activities. Nostalgia mode.
- `wh` – Writes that history to a timestamped text file. Scrapbooking, anyone.
- `q` / `quit` – Exit the browser gracefully.
- `cp` – Nukes saved preferences (dev tool). Use only if you enjoy rebuilding settings from scratch.

## Project Commands

- `lpj` – Lists all available projects.
- `backup [directory]` – Backup the current project into a `.tar.gz`. Provide a directory if you insist on tidiness; otherwise the default location is used.
- `restore <archive> [--project NAME] [--overwrite]` – Restores a project from an archive. You can rename it on the fly, force overwrites (after confirming you really, really mean it), and the browser will switch to the restored project automatically.

## Database Commands

- `ldb` – Lists every database in the current project.
- `db <name>` – Switches to the specified database instantly.
- `s [needle]` – Searches activity names inside the current database. Combine with:
  - `-loc {LOCATION}` to filter by location.
  - `-cat {CAT::SUBCAT::…}` to zero in on categories.
  - `-rp {REFERENCE PRODUCT}` to hunt by reference product.
  - `-cas {000000-00-0}` for CAS-number sleuthing (biosphere databases only).

## Activity Commands

- `a <id>` – Jumps straight to an activity by code or integer ID (for BW25).
- `aa [name]` – Lists all activities in the current database, optionally sorted by name.
- `i` / `ii` – Shows concise or extended activity info. `ii` is basically `i` but more intimate.
- `r` – Picks a random activity. Because serendipity 💜.
- `u`, `up`, `uu`, `un` – Variations on "show upstream technosphere inputs", adding pedigree, formulas, or uncertainty details respectively.
- `d` – Shows downstream consumers of the current activity.
- `b` – Lists biosphere flows for the current activity.
- `pe` / `pei` – Displays production exchanges and their detailed metadata.
- `cfs` – Prints characterization factors for the current method/biosphere activity combo.
- `G` – Runs an LCIA on the current activity for the selected method(s). Multiverse-friendly (i.e.: _if a full method is selected, and not a specific category and subcategory, it will do the LCIA of all the categories and subcategories of the method).
- `ta` / `te` – After an LCIA, list top activities or top emissions.
- `ca [cutoff]` – Prints a recursive contribution analysis, optionally trimming at `cutoff`.
- `sc [cutoff]` – Similar, but for the supply chain view.
- `add` – Adds the current activity to the temporary analysis list.
- `lt` – Lists everything in that temporary list (a.k.a. `list` in earlier docs).
- `clear` – Empties the temporary list; therapeutic but irreversible.
- `G C` – (Typed as `GC`) Launches multi-activity LCIA for the temporary list plus the fully specified method.
- `GCH` – Draws a charming ASCII bar chart from the most recent `GC` results 🤓.

## Method Commands

- `lm` – Lists methods (or namespaces) available in the current project.
- `mi` – Shows metadata for the fully specified method/category/subcategory.

## Parameter Commands

- `lpam [-f] [-g {GROUP}]` – Lists all project/database/activity parameters. `-f` shows every column; `-g` filters by group.
- `lpamg` – Lists parameter groups.
- `ap [-f]` – Shows parameters for the current activity (`-f` for verbose mode).
- `dp [-f]` – Displays parameters for the current database.
- `pp [-f]` – Prints project-level parameters.
- `fp <name>` – Finds a parameter by exact name across scopes.
- `sp <pattern>` – Wildcard-friendly parameter.

## Misc Commands

- `tsv [filename]` – Writes the most recent tabulated results to TSV.
- `wh` – Already mentioned above, but worth remembering for logging your wanderings.
- `help` – Alias for `?`, in case muscle memory from every other CLI kicks in.

With this lexicon, you're ready to charm the tool into revealing every LCA secret it knows. Happy exploring!
