# Tom's Lab Pages

## https://tom-gilbertsons-lab.github.io

**Using the https://github.com/LeNPaul/academic theme.**

You can make content changes via the Github text editor/ file uploader (i.e. no need to pull the repo & push changes; but if you do want to do that follow instructions at https://github.com/LeNPaul/academic for info on how to run local development server etc). 

It's not completely self-explanatory to make changes; but steps are outlined below. Before you start, sign up to github and ask to be added as a member of the organisation/ collaborator on this repository.

## How to... 

### Add yourself to the lab pages

#### To the 'people' pages: 
'People' are listed in the [people.yml file](_data/people.yml) (if not familiar, YAML is a standardised data serialisation format). 

There are two sections, people & prev-people (so add yourself to people). 

For a new person you want to add lines/ a line; following the pattern below:
```
- {name: 'Dr Isla Barnard', title: 'Postdoctoral Research Assistant', department: 'Physics & Biomedical Engineering',
  institution: 'School of Science & Engineering, University of Dundee', institution_address: 'Fulton Building, Dundee',
  email: 'ibarnard001@dundee.ac.uk', office: 'Lab Block L6 C 044, Ninewells Hospital & Medical School, Dundee',
  image: 'assets/img/placeholder.png', url: 'isla-barnard',
  one-line-statement: 'Computational physicist (numerical methods + some web tools'}
```
Most of this is just text (i.e what you type is what will show up on the page) but there are two non-text fields:
`image: 'assets/img/placeholder.png'` & `url: 'isla-barnard'`,

The image is a relative link to a picture (the one above is a placeholder; keep this if you don't have a photo!). 
To upload a photo, name it something sensible (i.e your-name.png or jpg); navigate to [assets/img/](assets/img/); click 'add files by upload'; and upload your file. Then if you change the link in your line as per above to `image: 'assets/img/your-name.png',` 

The url is a relative link to a personal page where you can add a bit more info about yourself and your research, and add some other links if you wish. You can leave it blank if you wish, and instructions are detailed in the next section but if you want to make use of this. 

#### Add your own one-page: 
In the YAML line above you see `url: 'isla-barnard'`. If you add your own name, 



The `_layouts/people.html` layout can be used to showcase and describe people in your research group. People are defined in the `_data/settings.yml` file, and markdown pages for each person with the `_layouts/page.html` layout can be placed in the `people` directory. 



## Front page
Home pages shows some info and also recent 'posts' if you want to use them. They can also just be deleted or not used,
he `_layouts/home.html` layout defines the home page for this theme. An introduction to your research group or to yourself can be provided, along with a list of featured publications. There is also a section for providing any updates through posts placed in the `_posts` directory.

### Add a post to the posts

The following sections describe usage instructions for this Jekyll theme,including available layouts, includes, sass and/or assets.


### Add a publication

The front pages show a set that are set in featured so try to update this as new papers come out (& leave good ones up! )
The `_layouts/publications.html` layout can be used to showcase selected publications, or the entire catalogue of publications. Direct links to the paper can be used, or a PDF copy of the paper can be served. Publications are defined in the `_data/publications.yml` file, and any PDF files that are served can be placed in the `publications` directory.


#### Home

T

#### Theme
Adapted from  GitHub at https://github.com/LeNPaul/academic; for info on how to run local development server have a look there.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
