# PKS - Personalized Key Stats

Technologies: Rust, Tauri, Leptos

## Notes

1.Ideally, creating a rust file with an object with all the letters and key press combinations as a key and 0 as value  
2. When user presses key, the file is accessed and the letter corresponding to the key pressed increments by 1  
3. When user requests for data aggregation, return heatmap of keyboard presses and statistics and values of key-presses based off of object data

Thinking about project structure:
`main.rs`: final logic
`input.rs`: location for data regardingl key logging
`stats.rs`: locaction for data aggregation and processing (heatmap included here)
`optimal_setup.rs`: location where aggregated data is utilized to recommend optimal keyboard setup

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer).

## Contributing

1. Ensure that you have the required prerequisites installed:
   • [Rust and Cargo](https://www.rust-lang.org/tools/install)
   • [Tauri](https://tauri.app/v1/guides/getting-started/prerequisites/)

2. Fork the `pks` repository to your own GitHub account
3. Clone your forked repository to your local machine.

```bash
git clone https://github.com/<your-github-username>/pks.git
```

4. Navigate to the project and build the application

```bash
cd pks
cargo tauri dev
```

### Scripts

`cargo tauri dev`: start tauri dev window
`RUST_BACKTRACE=1 tauri dev`: (Linux and macOS) Rerun tauri dev with granular stack trace

(Windows)

```bash
$ set RUST_BACKTRACE=1
$ tauri dev
```

## License

This project is licensed under the terms of the [MIT LICENSE](./LICENSE)
