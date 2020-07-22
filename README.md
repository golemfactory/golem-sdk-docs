# Golem SDK Docs

The repo consist of two main branches, `master` and `prod`. 

`prod` is connected with gitbook so any change there will be instantly available on public doc.

`master` branch is for tracking md files from linked submodules and map those files to appropriate documentation directories.

## How it works

To add new md files into documentation, edit `map.txt` file by adding `source_path=target_path` pair on each line. When those changes merged in master, related github actions will be triggered and create a PR which has a target folder as defined in `map.txt`. You can either merge this pr into `prod` and do markdown edits on gitbook, or can resolve if any conflicts beforehead.

To be able to see new documentation files in gitbook don't forget to add your `target path` into [SUMMARY.md](./SUMMARY.md)
