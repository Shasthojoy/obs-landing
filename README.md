The Open Build Service Landing page
===================================

This page is based on [jekyll](https://github.com/mojombo/jekyll) and [foundation](http://foundation.zurb.com/)
and is served via [github pages](http://pages.github.com/) to [openbuildservice.org](http://www.openbuildservice.org)

### Markdown

GitHub Pages are written in kramdown. A quickref for the syntax can
be found [here](https://kramdown.gettalong.org/quickref.html).

### Local preview

Just run:

```
bundle exec jekyll serve
```

You may need to run `bundle install` before.


### Add new members to team page

Add the following lines at the end of the YAML front matter block:

- name: Example Name
  position: Frontend Developer
  email: example@suse.de
  github: examplegithub
  twitter: exampletwitter
  blog: https://examplename.com
  irc: exampleirc
  description: "Write a nice description of yourself.
  You can use **markdown** in ~~the~~ _description_.

  \nAnd add new paragraphs too."

You don't need to include all the fields, you can just remove the one you don't want to have.
If you use special characters you may need to sorround your text by `"`.


### Updating OBS documentation

The OBS documentation is stored in a [separate repository](https://github.com/openSUSE/obs-docu)
and is integrated into the OBS landing page via git submodules.

To update our documentation simply run the [update_documentation.sh]() script. This
updates the documentation sub-module, compiles it into html and creates a new commit
with the changes.

# License

The code in this repository is licensed under a [MIT license](LICENSE).

The blog's content is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License.
<img alt="CC" src="/images/icons/cc.png" width="18px"/>
<img alt="BY" src="/images/icons/by.png" width="18px"/>
