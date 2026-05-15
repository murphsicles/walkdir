# @fs/walkdir — Recursive Directory Walking for Zeta

Auto-converted from [walkdir](https://crates.io/crates/walkdir) v2.5.0 via [Dark Factory](https://github.com/murphsicles/dark-factory).

## Features
- Recursive directory traversal with iterator API
- Configurable max depth, sorting, and filtering
- Follow symlinks option
- skip_current_dir — skip entries without error
- Efficient directory entry caching
- Cross-platform path handling

## Usage
```zeta
for entry in WalkDir::new("/tmp").max_depth(3).sort_by(|a,b| a.cmp(b)) {
    let entry = entry.unwrap();
    println!("{}", entry.path().display());
}
```

## Stats: ~1,610 lines across 7 source files, 0 unsupported items

## License
MIT