# Tom's Lab Pages

## https://tom-gilbertsons-lab.github.io

*Using the https://github.com/LeNPaul/academic theme.*


## Getting started 
Sign up to github and ask to be added as a member of the lab organisation & as a collaborator on this repository.\
You can make content changes directly via the Github text editor/ file uploader. 
You can make changes by 
-  editing existing files
-  adding or deleting new files (& file paths)
  
On git(hub) changes are saved via commits. To commit a change, press the green **Commit changes** button on top right of the editor page.   

## How to 

### Add yourself to the lab pages

#### To the [people](https://tom-gilbertsons-lab.github.io/people) pages: 
'People' are listed in the [people.yml file](_data/people.yml) (.yml files are a standardised data serialisation format). 

The yml is divided into two sections, people & prev-people (so add yourself to people). 

For a new person, you want to add an entry following the pattern below (read the existing ones):
```
- {name: 'Firstname Lastname', title: 'Student/ Clinical Fellow/ Role', department: 'Neuroscience',
  institution: 'School of Medicine, University of Dundee', institution_address: 'Ninewells Hospital & Medical School, Dundee',
  email: 'youremail@dundee.ac.uk', office: 'Lab Block L6 C 044, Ninewells Hospital & Medical School, Dundee',
  image: 'assets/img/placeholder.png', url: 'your-name',
  one-line-statement: 'State in one line what you do'}
```
Most of this is just text (i.e what you type in your entry is what will show up on the page) but there are two non-text fields:
`image: 'assets/img/placeholder.png'` & `url: 'your-name`,

**The image** field is a relative link to a picture (the one in [`assets/img/placeholder.png`](assets/img/placeholder.png) is a placeholder, so keep this if you don't have a photo.\ 
To upload a photo, name the photo something sensible (i.e your-name.png or jpg), navigate to [`assets/img/`](assets/img/), and upload by clicking 'add files by upload'.\
Then if you change the link in your entry in the  [people.yml file](_data/people.yml) to `image: 'assets/img/your-name.png'` (or `.jpg`) then your photo will appear by your name on the [people](https://tom-gilbertsons-lab.github.io/people) page. 

**The url** field directs to personal one-page site where you can show more about yourself and your research. Feel free to leave the field blank, however if you do want to make use of this instructions are detailed in the next section. 

#### Add your own one-page: 
In the YAML line above you see `url: 'your-name'`. If you add your own name, save and commit, this sets up a relative link to a page that you can create.

In the [`people`](people/) directory, you'll see files with `persons-name.md` - this contains the content that the link `url: 'persons-name'` will take you to when clicked. 

Feel free to duplicate the content of an exisiting file in [`people`](people/).\
Duplicate this by looking at the file, select 'raw' and copy that across to a new file.\
Save as  `your-name.md` (make sure the  `url: 'your-name'` and the `your-name` in `your-name.md` are identical).\
Add some info about your research, save & commit this, and your one-page site will be accessible via the `more info` link from the main people page. 

## Front page
The home page shows text from the [`index.md`](index.md) and the image at  [`assets/img/home.png`](assets/img/home.png), along with featured publications and recent posts.

## Add publications & talks 
Publications are listed in the [`_data/publications.yml`](_data/publications.yml) file (and PDFs may be served via the `publications` directory).\
The [`_data/publications.yml`](_data/publications.yml) file also has a set for featured publications, try to update this as new papers come out (& leave good ones up!) as these sow on the front page. 

### Add a post
Posts disseminating news/ updates may be placed in the [`_posts/`](_posts) directory. Again, just copy an exisiting post from that dir and rename with format `YY-MM-DD-post-name.md`. The site should pick it up when it rebuilds. 

## License & Theme
Adapted from  GitHub at https://github.com/LeNPaul/academic. The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
