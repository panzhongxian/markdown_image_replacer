### Install

```bash
pip install markdown-image-replacer
```

### Usage

The following command will parse the mardown file specified by the first argument, move the local images or download remote images to the directory combined by the last two parameters, and generate a new mardown file specified by the `dst_md_file`.

The `dst_img_root` is the root directory which may be used in website frame work. The `dst_img_rel_dir` should be the relavant directory from `dst_img_root`, which will be written into the image url inside markdown file.

```bash
python -m markdown_image_replacer \
   $HOME/blog/content/posts/my-first-post.md \
   --src_img_root $HOME/blog/static \
   --dst_md_file $HOME/blog/content/posts/my-first-post2.md \
   --dst_img_root $HOME/blog/static \
   --dst_img_rel_dir images/my-first-post
```




