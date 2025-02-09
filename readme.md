# RTL Style Example plugin

This is a demo plugin to show that RTL styles are not being enqueued correctly when generated by wp-scripts & `register_block_type_from_metadata`.

To test it out, download the repo & drop it into the plugins directory of a WordPress install. Or use `wp-env start` from the root of the project (requires wp-env to be globally installed). `SCRIPT_DEBUG` should be false.

Create a post and add the "RTL Style Example" block. View post on the frontend. On an LTR langauge site (English), the text should have a border on the left.

Switch your site language to an RTL language (Settings > General), the admin and frontend will flip to use RTL styles. View the post again, and the border is still on the left. It _should_ be on the right, in RTL.

| LTR | RTL (incorrect) |
|---|---|
| ![ltr](https://github.com/ryelle/rtl-style-example/assets/541093/ab1fa193-5e55-4fe2-9fe8-5daf9c573f46) | ![rtl](https://github.com/ryelle/rtl-style-example/assets/541093/0e7fcd28-209e-4922-a87d-c72faa23c478) |

