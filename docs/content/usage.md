# Usage

This is a command-line utility to browse, search, and filter databases. When you’re ready to boss it around, grab the full lexicon in [the commands section](./commands.md) — it's the tool's secret diary, except it wants you to read it.

## How the text UI flows

The tool is a text-based interface, so everything happens through the prompt you see in your terminal. The flow is simple:

1. The tool shows a prompt, optionally with context (project/database/activity).
2. It may list options, numbered from zero upward.
3. You send a response by typing either:
   - A [command](commands.md) (e.g., `lpj`, `backup`, `s -loc {CH} energy`), or
   - A number to pick one of the displayed options.
4. Press `Enter`, wait for the new output, and repeat.


:::{admonition} Seeing it live!
:class: tip

In the following asciinema recording, you can see how to invoke the tool, select a project, select a database, search for an activity, select an activity and print the metadata of the activity.

```{asciinema} asciinema/invoke.cast
```
:::

Because it’s entirely keyboard-driven, there’s no mouse interaction to worry about. It's more or less like a conversation: you give short instructions, it replies with lists, details, or questions. When a numbered list is on screen, responding with the corresponding number confirms the selection instantly. When you want to do something different, type the command and press `Enter`. Easy rhythm, minimal ceremony. ✨

## Tool invocation

The package provides an executable script: ``bw2-browser`` (regardless of the installed package, [bw25ui](https://pypi.org/project/bw25ui/) or [bw2ui](https://pypi.org/project/bw2ui/).

The basic way to invoke the tool is:

```console
  bw2-browser
```
This will start it, and immediately list the available projects.

![bw2-browser simple invocation](bw2-browser_simple_invocation_example.png)
![bw2-browser simple invocation output](bw2-browser_simple_invocation_example_output.png)

If you already know the project you want to start with, you can provide it as argument to the tool:

```console
  bw2-browser <project>
```

The same applies if you already know a database name or an activity id:

```console
  bw2-browser <project> <database>
```
```console
  bw2-browser <project> <database> <activity-id>
```

**Arguments**

+ ``project``

    Defines a project to start with

+ ``database``

    Defines a database to start with

+ ``activity-id``

    Defines an activity to start with


**Options**

  + ``-h`` ``--help``     
        Show help screen.

  + ``--version``     
        Show the current version of the tool.

