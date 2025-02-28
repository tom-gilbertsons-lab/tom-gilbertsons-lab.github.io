# Tom's Lab Pages

## https://tom-gilbertsons-lab.github.io

*Using the https://github.com/LeNPaul/academic theme.*

You can make content changes via the Github text editor/ file uploader (i.e. no need to pull the repo & push changes; to do so follow instructions at https://github.com/LeNPaul/academic for info on how to run a local dev server etc.). 

Steps to make changes are outlined below. 

Before you start, sign up to github and ask to be added as a member of the organisation/ collaborator on this repository.

There are two ways to make changes to the repo via github itself- one is to edit an existing file (

## How to... 

### Add yourself to the lab pages

#### To the 'people' pages: 
'People' are listed in the [people.yml file](_data/people.yml) (.yml files are a standardised data serialisation format). 

There are two sections, people & prev-people (so add yourself to people). 

For a new person, you want to add an entry following the pattern below:
```
- {name: 'Dr Isla Barnard', title: 'Postdoctoral Research Assistant', department: 'Physics & Biomedical Engineering',
  institution: 'School of Science & Engineering, University of Dundee', institution_address: 'Fulton Building, Dundee',
  email: 'ibarnard001@dundee.ac.uk', office: 'Lab Block L6 C 044, Ninewells Hospital & Medical School, Dundee',
  image: 'assets/img/placeholder.png', url: 'isla-barnard',
  one-line-statement: 'Computational physicist (numerical methods + some web tools)'}
```
Most of this is just text (i.e what you type is what will show up on the page) but there are two non-text fields:
`image: 'assets/img/placeholder.png'` & `url: 'isla-barnard'`,

**The image** field is a relative link to a picture (the one above is a placeholder; keep this if you don't have a photo!). 
To upload a photo, name it something sensible (i.e your-name.png or jpg), navigate to [`assets/img/`](assets/img/), and upload by clicking 'add files by upload'. Then if you change the link in your entry as per above to `image: 'assets/img/your-name.png'` then your photo should appear by your name on the 'People' page. 

**The url** field is a relative link to a personal page where you can add a bit more info about yourself and your research. Feel free to leave it blank, however if you do want to make use of this instructions are detailed in the next section. 

#### Add your own one-page: 
In the YAML line above you see `url: 'isla-barnard'`. If you add your own name, save and commit, this sets up a relative link to a page that you can create.

In [`people`](people/), you'll see files with `persons-name.md` - this is the link that the `url: 'persons-name'` will take you to when clicked. 

Feel free to duplicate the content of an exisiting file in [`people`](people/) (do this by looking at the file, select 'raw' and copy that across to a new , save as  `your-name.md` (make sure the  `url: 'your-name'` and the `your-name` in `your-name.md` are identical); and add some info about yourself. When you save & commit this, you'll get this content up as a `more info` link from the main people page. 

## Front page
The home page shows text from the [`index.md`](index.md) and the image at  [`assets/img/home.png`](assets/img/home.png). It also contains featured publications and recent 'posts'; instructions on how to add these are below. 
he `_layouts/home.html` layout defines the home page for this theme. An introduction to your research group or to yourself can be provided, along with a list of featured publications. There is also a section for providing any updates through posts placed in the `_posts` directory.

### Add a post to the posts
There is also a section for providing any updates via posts placed in the [`_posts/`](_posts) directory. Again just copy the an exisiting post from that dir The format of this should be `YY-MM-DD-post-name.md` and the site should pick it up when it builds. 
### Add a publication

The front pages show a set that are set in featured so try to update this as new papers come out (& leave good ones up! )
The `_layouts/publications.html` layout can be used to showcase selected publications, or the entire catalogue of publications. Direct links to the paper can be used, or a PDF copy of the paper can be served. Publications are defined in the `_data/publications.yml` file, and any PDF files that are served can be placed in the `publications` directory.


#### Theme
Adapted from  GitHub at https://github.com/LeNPaul/academic; for info on how to run local development have a look there.
## License
The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
