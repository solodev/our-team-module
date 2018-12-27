# our-team-module

## Prerequisites
<ul>
	<li><a target="_blank" href="https://getbootstrap.com/">Boostrap4</a></li>
</ul>

## Step 1: Add the Form
 - team-form.tpl

Create a calendar for the Team and upload the following form. Be sure to replace SITE_NAME with your site's name.

```
<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseStatus">Post Status<span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseStatus">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-6">
            <h2><label class="label-control" for="post_status">Post Status</label></h2>
            <select class="form-control" name="post_status" type="text">
              <option value="Draft">Draft</option>
              <option value="Published">Published</option>
            </select>
          </div>

         
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseImages">Team Info <span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseImages">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-6">
            <h2><label class="label-control" for="team_member_image">Team Member Image</label></h2>

            <p class="subText">(Required) The image that appears in the post and normal blogroll feed. Dimensions:
              951px by 561px.</p>
            <input class="file_upload" id="team_member_image" name="team_member_image" required="" type="file" />
          </div>

          <div class="col-md-6">
            <h2><label class="label-control" for="team_member_pos">Team Member Position</label></h2>
            <input class="form-control" id="team_member_pos" name="team_member_pos" required="" type="text" />
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseContact">Team Contact <span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseContact">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-3">
            <h2><label class="label-control" for="team_member_email">Team Member Email</label></h2>
            <input class="form-control" id="team_member_email" name="team_member_email" required="" type="text" />
          </div>

          <div class="col-md-3">
            <h2><label class="label-control" for="team_member_phone">Team Member Phone</label></h2>
            <input class="form-control" id="team_member_phone" name="team_member_phone" required="" type="text" />
          </div>

          <div class="col-md-3">
            <h2><label class="label-control" for="team_member_location">Team Member Location</label></h2>
            <input class="form-control" id="team_member_location" name="team_member_location" required="" type="text" />
          </div>

          <div class="col-md-3">
            <h2><label class="label-control" for="team_member_hours">Team Member Hours</label></h2>
            <input class="form-control" id="team_member_hours" name="team_member_hours" required="" type="text" />
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a aria-expanded="true" data-toggle="collapse" href="#collapseContent">Post Content<span
            class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseContent">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="heading_title">Heading Overwrite</label></h2>

            <p class="subText">(Optional) If specified, this will overwrite the article's title and become the main
              heading.</p>
            <input class="form-control" id="heading_title" name="heading_title" type="text" />
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_intro">Intro/Subtitle</label></h2>

            <p class="subText">(Required) Content that appears before the Body Content and the introductory paragraph
              on the blogroll.</p>
            <textarea class="form-control" id="post_intro" name="post_intro" required=""></textarea>
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_content">Body Content</label></h2>

            <p class="subText">(Required) The main content section for an article.</p>
            <textarea class="wysiwyg" id="post_content" name="post_content" required=""></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseMeta">META Data <span class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse" id="collapseMeta">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_title">Meta Title</label></h2>

            <p class="subText">(Optional) Include a custom META Title that will show in your browser tab and in the
              page's source code.</p>
            <input class="form-control" id="meta_title" name="meta_title" type="text" />
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_description">Meta Description</label></h2>

            <p class="subText">(Optional) Include a custom META Description that search engines will index. 50-160
              Characters</p>
            <textarea class="form-control" id="meta_description" name="meta_description"></textarea>
          </div>
        </div>

        <div class="row">
          <div class="col-md-12">
            <h2><label name="meta_keywords">Meta Keywords</label></h2>

            <p class="subText">(Optional) Include the main keywords of the blog article.</p>
            <textarea class="form-control" id="meta_keywords" name="meta_keywords"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseAdvanced">Advanced <span class="toggle"
            aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse" id="collapseAdvanced">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <h2><label class="label-control" for="post_javascript">Custom JavaScript</label></h2>

            <p class="subText">(Optional) Use the following textbox to embed any custom JavaScript including tracking
              pixels and Google Analytics scripts. Be sure to open your JavaScript with a &lt;script&gt; tag and close
              everything with a &lt;/script&gt; tag.</p>
            <textarea class="form-control" id="post_javascript" name="post_javascript"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<?php
            if(isset($dataVars['calendar_entry_id'])){     
              $calendar_entry = new Calendar_Entry($dataVars['calendar_entry_id']);
              if($calendar_entry->path) { 
          ?>

<div class="panel-group">
  <div class="panel panel-default">
    <div class="panel-heading">
      <h4 class="panel-title"><a data-toggle="collapse" href="#collapseURL">Post URL <span class="toggle" aria-hidden="true"></span></a></h4>
    </div>

    <div class="panel-collapse collapse in" id="collapseURL">
      <div class="panel-body">
        <div class="row">
          <div class="col-md-12">
            <p class="subText">You can access this blog post at the following URL:</p>
            <a href="https://www.SITE_NAME.com<?= $calendar_entry->path ?>" target="_blank">https://www.SITE_NAME.com
              <?= $calendar_entry->path ?></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<?php 
              } 
            }
           ?>
<script>
  $('.wysiwyg').ckeditor(function () {}, {
    customConfig: '/CK/config.js',
    height: '600px',
    basePath: '/CK/',
    toolbar: 'WP'
  });
</script>

```

## Step 2: Add the Repeater
 - team-repeater.tpl

Add the following repeater shortcode. 

```
<div class="row py-5">
  <div class="text-center col-md-8 mx-auto">
    <h2 class="text-uppercase">Building New Worlds Together</h2>
    <p>Meet the team of talented people that are leading our exploration of the moon and beyond.</p>
  </div>
</div>
  
<div class="row pb-5">
[repeater id='10' pages="22" order="start_time desc" display_type="news" where="post_status='Published'"]
  <div class="col-md-6 col-lg-3">
    <a href="{{path}}">
      <div class="position-relative bg-secondary bg-hover-secondary-dark">
        <img alt="Team Image" src="[get_asset_file_url id={{team_member_image}}]" class="w-100 img-fluid">
        <div class="text-white text-center border-top border-white w-100 p-2">
          <h2 class="mb-0 h6 text-uppercase">
          [is_set value={{heading_title}}]
          	{{heading_title}}
          [/is_set]
          [is_empty value={{heading_title}}]
          	{{event_title}}
          [/is_empty]
          </h2>
          <p class="mb-0"><small>{{team_member_pos}}</small></p>
        </div>
      </div>
    </a>
  </div>
[/repeater]
</div>
```

## Step 3: Add the Detail Template
- team-detail.tpl

```

[entry]
  <div class="row align-items-center mb-lg-5">
    <div class="col-md-3 text-lg-center text-left">
      <img alt="Image Title" class="w-225p img-fluid rounded-circle" src="[get_asset_file_url id={{team_member_image}}]">
    </div>
    <div class="col-md-9 mt-lg-0 mt-5">
      [is_set value={{team_member_pos}}]
        <h2 class="text-uppercase">{{team_member_pos}}</h2>
      [/is_set]

      <hr class="my-4">
      <div class="row">
        <div class="col-md-6">
          <p><i class="w-25p far fa-envelope pr-2"></i> <a href="mailto:{{team_member_email}}">{{team_member_email}}</a></p>
          <p><i class="w-25p fas fa-mobile-alt pr-2"></i> <a href="tel:{{team_member_phone}}">{{team_member_phone}}</a></p>
        </div>
        <div class="col-md-6">
          <p><i class="w-25p fas fa-map-marker-alt pr-2"></i>{{team_member_location}}</p>
          <p><i class="w-25p far fa-clock pr-2"></i>{{team_member_hours}}</p>
        </div>
      </div>
    </div>
  </div>
  <hr>
  <div class="row pt-4">
    <div class="col-sm-12">
      {{post_content}}
    </div>
  </div>
  {{post_javascript}}
[/entry] 

```

## Step 4: Add the SCSS/CSS
- /_/scss/team.scss

```
.w-25p {
 width: 25px;
}
```
