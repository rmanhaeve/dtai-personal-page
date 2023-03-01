# Simple instructions


## Getting started

For more about how to use Jekyll, check out [this tutorial](https://www.taniarascia.com/make-a-static-website-with-jekyll/).



### Installation

Don't use Ruby 3, use Ruby 2, or use the original template instead: [https://github.com/alshedivat/al-folio](https://github.com/alshedivat/al-folio)

Assuming you have [Ruby v2](https://www.ruby-lang.org/en/downloads/) (Ruby+Devkit on Windows) and [Bundler](https://bundler.io/) installed on your system, first fork the theme to `github.com:<your-username>/<your-repo-name>` and do the following:

```bash
$ git clone git@github.com:<your-username>/<your-repo-name>.git
$ cd <your-repo-name>
$ bundle install
```

### Configuration



1. Launch the site by running this command, which will host the website on [http://localhost:4000/](http://localhost:4000/). Run this command after every ```_config.yml``` update.

```
bundle exec jekyll serve --watch
```

2. Go to ```_config.yml``` and update the properties:
- Your first name in ```first_name```
- Your last name in ```last_name```
- Your personnel number in ```ku_leuven_personnel_number``` to link up your publications (number AFTER the u)
- Your social media profiles that you would like to link 
- `show_news` to `false` if you don't want to post news message on your website.


3. Go to ```_pages/about.md``` and fill in your own biography to display.

4. Update ```assets/img/prof_pic.jpg``` to a picture of yourself (file name updatable in ```_pages/about.md```)

5. Add your teaching activities (teaching assistant, thesis students, seminars) to the csv files in ```_data/teaching/```.

6. Create your projects by copying and editing the content of the ```_projects folder```

7. If you prefer a different theme color, go to ```_sass/_variables.scss``` and change ```$theme-color: $blue;``` to any color defined above this line.


For more advanced info, see [the original al-folio template](https://github.com/alshedivat/al-folio).



### OPTIONAL: Publications with Jekyll-Scholar

By default, your publications will be retrieved from Lirias.
If you want more control over your publication page, you can use the Jekyll-Scholar plugin.

Advantages of Jekyll-Scholar:
- Use bibtex files to import your publications 
- Control which publications you show and how you group and order them
- Add extra fields to your bibtex entries to include links to paper arxiv page, pdfs, supplementary materials, code, slides, poster, videos, and anything else if you want to.
- Cite your and other's work anywhere in your website, simply using {% cite <bibtex-key> %}  

#### How to enable Jekyll-Scholar: 

1. Go to ```_config.yml``` and update the properties:
- Set ```use_scholar``` to ```true```
- Your last name in ```scholar: last_name```

2. Add your bibtex file to ```_bibliography/references.bib```. Now the basic publications page works!

3. You can now additionally add the following fields to your publications in BibTeX:
    
    1. ```abstract```: creates a button ```[Abstract]``` for showing the paper's abstract

    2.  ```arxiv```: links to the arXiv ID of your paper.
   
    3. ```video```: url of the video (e.g. talk recording)
  
    4. You can add attachments to your bibtex entries by storing them in ``assets/pdf/`` and linking to them in your bibtex entry. The possible attachments are ```pdf```,```supp```,```slides```,```poster```. Link to them by adding the filenames to the corresponding bibtex field.


4. Fill out information about your co-authors in ```_data/coauthors.yml``` to automatically link their namses to their personal websites.

5. *More documentation*: [Jekyll-Scholar](https://github.com/inukshuk/jekyll-scholar/) documentation for learning how to sort, group and filter your publications, how to cite papers, and how to use multiple bib files (e.g. to add an extra bib file with other papers that you like to cite).





### Deployment

After you are done, **commit** your final changes.
Now, you can deploy your website to [GitHub Pages](https://pages.github.com/) by running the deploy script:

```bash
$ ./bin/deploy [--user]
```
By default, the script uses the `master` branch for the source code and deploys the webpage to `gh-pages`.
The optional flag `--user` tells it to deploy to `master` and use `source` for the source code instead.
Using `master` for deployment is a convention for [user and organization pages](https://help.github.com/articles/user-organization-and-project-pages/).


## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
