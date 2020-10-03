---
layout: howto
title: How To Configure Your Website
---

Below are a few quick steps to help you begin configuring your GitHub site for use with Oral Histories as Data (OHD). 

{% include youtube/embed.html  video-id="lJ9b0VNJIMw" title="Making a Filter" display="d-none d-md-block" %}
## Step 1: Make a Template of OHD

- Go to the OHD homepage and click on the "Template" button toward the top right of the page. 
{% include bootstrap/figure.md img="howto/ohd_template.png" caption="" alt="picture of the button that enables user to create a new template in github" class="w-50" %}
- Then you'll need to name your repository.
{% include bootstrap/figure.md img="howto/name_repository.png" caption="" alt="image of the field users must fill out in order to create a name for their new template" class="w-50" %}
- Once you've named your repository, you'll need to click the "Create Repository From Template" button. 
{% include bootstrap/figure.md img="howto/create_repository_button.png" caption="" alt="picture of the create repository button located at the bottom of the page" class="w-50" %}

## Step 2: Create a New File

- Now you'll need to go into you "data" folder and then into the "transcripts" folder in your repository. 
- Once in transcripts click on "create new file".  
{% include bootstrap/figure.md img="howto/new_file.png" caption="" alt="picture of the create new file button in the newly created repository" class="w-50" %}
- Now you need to name your file according to your transcript. This will need to match the Markdown file you'll create later in this how-to. 
    - We recommend using the last name, or first and last name of the subject, in all lowercase letters with no spaces or unusual characters. 
    - Be sure to add ".csv" to the end of the filename as well. For example, a subject named John Smith would be named  "smith.csv" or "john_smith.csv."
{% include bootstrap/figure.md img="howto/name_file.png" caption="picture of the required field for naming your new file" alt="" class="w-50" %}
- Leave the file open on the page. We'll be adding to it via the next step.

{:.alert .alert-warning}
When you name your file be sure to include the type of file after the name you choose. In our case, you'll want to add a ".csv" to the end of the filename. (robert.csv) For example, if it is a markdown file, attach ".md" after the file name. For a markdown file, like the one we'll create below, you'll add a ".md" after the file name.

## Step 3: Moving the Transcript to a new GitHub file

- Open your transcript **in a text editor**.

{:.alert .alert-danger}
Make sure you open your transcript in a text editor. DO NOT OPEN UP THE CSV IN EXCEL!!! Excel might reformat your timestamps. We recommend using [Visual Studio Code](https://code.visualstudio.com/), but notepad or textedit (the default text editors on Windows and Mac machines, respectively) will also work. 
- Open the transcript in a text editor. 
- Select the entire text (ctrl + a) 
{% include bootstrap/figure.md img="howto/text_editor.png" caption="transcript selected in text editor" alt="" class="w-50" %}
- Copy and paste it into the new file open you created in step 2. 
{% include bootstrap/figure.md img="howto/github_pasted-transcript.png" caption="completed .csv file" alt="" class="w-50" %}
- Commit the change at bottom of page by scrolling to the bottom of the page and click "commit new file". 
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="" class="w-50" %}
- Below is what the CSV should look like after you've committed it on the GitHub webpage. 
{% include bootstrap/figure.md img="howto/github_csv.png" caption="This is how the CSV should look after you paste it into the new file and commit it." alt="complete and committed csv in github" class="w-50" %}

{:.alert .alert-warning .mb-4}
NOTE: If the CSV has a problem, GitHub will show you an error message that will say: "We can make this file beautiful and searchable if this error is corrected:" After that phrase, they will also point out a line number that is causing the problem. Open the file up by clicking on the pencil icon in the top right of the file area. Go to the line indicated and see if there's an obvious error. If you can't get it fixed, go back to your Google Sheet and see if there's anything to clean up. Even if there is nothing wrong, re-download the file as a CSV, open it in a text editor, then copy and paste it back into the problematic file on GitHub. Hopefully one of these steps clears up the problem. 

{% include youtube/embed.html  video-id="kfDeEfjl6nQ" title="Creating a .MD File" display="d-none d-md-block" %}
## Step 4: Creating a Markdown File

- Navigate back to the main page of your repository
- Click on the folder that says "_transcripts" 
{% include bootstrap/figure.md img="howto/transcripts.png" caption="" alt="_transcipts button" class="w-50" %}
- Open up any of the .md file examples that are in this folder
- Navigate to the button that says "raw" and click it
{% include bootstrap/figure.md img="howto/raw.png" caption="" alt="raw file button" class="w-50" %}
- Copy the text inside of this file
{% include bootstrap/figure.md img="howto/newcopyandpaste.png" caption="" alt="raw file text" class="w-50" %}
- Go back to the page with the example .md files
- Click the "Create New File" button
{% include bootstrap/figure.md img="howto/createnewmd.png" caption="" alt="create new file button" class="w-50" %}
- Name this file what you named your transcript file, but be sure to put .md rather than .csv, as this is a markdown file you are creating. 
{% include bootstrap/figure.md img="howto/mdname.png" caption="" alt="name field in new markdown file" class="w-50" %}
- Then paste the text you copied from the raw file into this new file
{% include bootstrap/figure.md img="howto/beforemd1.png" caption="Pasted text before editing" alt="pasted text in new .md file" class="w-50" %}
- Edit the text to fit your data 
{% include bootstrap/figure.md img="howto/aftermd2.png" caption="File after being edited for new file" alt="new .md file text after being edited for new file" class="w-50" %}


{:.alert .alert-warning .mb-4}
NOTE: change the "object-id" field so that it is the same as the name of your file (and the CSV you created earlier)

- Write a brief description of the changes you made and then commit them at the bottom 
- Once you are done, navigate to your new file, it should look like the example below
{% include bootstrap/figure.md img="howto/comletemd.png" caption="" alt="the newly created md file" class="w-50" %}

### Optional: adding an audio or video file using av_source

{:.alert .alert-info}
You may want to include an auditory or visual component to your transcript. You'll need to incorporate some simple information in the header of your markdown file. By including a video or audio file, you can correspond recorded dialogue to your written transcript. 

- Look in the header of your markdown file. You'll see that there is a space for av_source. Here you have four options, using OHD: `mp3, youtube,  soundcloud, or vimeo`. 

Using all lowercase letters, type the platform's name where your file is uploaded. 
{% include bootstrap/figure.md img="howto/avid1.png" caption="" alt="opened file, ready for editing" class="w-50" %}
- Below av_source, you'll see a space for your file's audiovideo-id. Fill in this information. 
{% include bootstrap/figure.md img="howto/avid2.png" caption="" alt="opened file, ready for editing" class="w-50" %}
- Below are pictures indicating the location of various audiovideo-id locations on different platforms. 
{% include bootstrap/figure.md img="howto/youtubeid.png" caption="location of your youtube audiovideo-id" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/vimeoid2.png" caption="location of your vimeo audiovideo-id" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/soundcloud_path_copy.png" caption="location of your the URL path" alt="opened file, ready for editing" class="w-50" %}


{:.alert .alert-warning .mb-4}
NOTE: if you want to utilize an mp3 file, you can create also create a webpage to house your file and link the URL, in quotation marks, in the audiovideo-id. You can store mp3s in your GitHub repository, but be aware that GitHub only allows a small amount of space to each repository. It's probably best practice to link them from elsewhere. You will also need to change av_source to "mp3". Follow the visualizations below for instruction. 

- If you have a page for your mp3 file copy the URL. 

{% include bootstrap/figure.md img="howto/url_mp3_final.png" caption="" alt="mp3 page URL" %}

- Copy and paste URL with quotation marks included. 

{% include bootstrap/figure.md img="howto/final_source.png" caption="" alt="Included URL for mp3 feature" %}

- Change *av_source* to "mp3". 

{% include bootstrap/figure.md img="howto/url_mp3_final.png" caption="s" alt="av_source edited to include mp3 file" %}



## Step 5: Setting up the visualization(s)

{:.alert .alert-info}
OHD offers a way to categorize your transcripts using tags. This is done through two locations: the "tag" column cells in your transcript's CSV and the filters.csv file, which is already provided for you in the structure of OHD. If you are not aware of either of these files, first visit our steps on "[How To Prepare Your Data](prepareyourdata.html)." 


{% include youtube/embed.html  video-id="esUuJbhXKW4" title="Creating Filters" display="d-none d-md-block" %}
- Open the filters.csv file you created in your text editor. 
- Navigate to the "_data" folder 
- Open the "_data" folder and click the pencil icon to edit the file
- Copy and paste the filters.csv you created in the Prepare Your Data tutorial over into the existing content. 
- Alternatively, you can simply edit the CSV file here. (Below is how the file looks when opened with the pencil icon.)
{% include bootstrap/figure.md img="howto/texteditorfile.png" caption="Filters.csv as it looks in a text editor" alt="opened file, ready for editing" class="w-50" %}
{% include bootstrap/figure.md img="howto/githubfile.png" caption="filters.csv copied into GitHub" alt="filters.csv copied into GitHub" class="w-50" %}
- Commit the change at the bottom of the page by clicking the commit button (be sure to write a commit message so you can track your changes)
{% include bootstrap/figure.md img="howto/commit_file.png" caption="" alt="picture of the commit button at bottom of page" class="w-50" %}
- However you edited it, the finished CSV should look like the example below (with your new tags and descriptions) in GitHub
{% include bootstrap/figure.md img="howto/githubfilefinal.png" caption="CSV after being transferred to GitHub" alt="finished csv after being transferred to github" class="w-50" %}
- Below is a slightly more robust example of what your visualization will look like. 
{% include bootstrap/figure.md img="howto/visualization.png" caption="finished OHD visual" alt="picture of finished visualization" class="w-50" %}




