# SpotifyDataAnalysis.github.io

## Project-2
#### 1 Tell a story through data visualizations
#### 2 create an interactive way for others to explore this data
#### 3 create a 10 min presentation
#### 4 chose a project theme (Spotify and music?)
Specific Requirements
- visualization must include a API, HTML/CSS, JavaScript, and at least one database
- create
a D3 project (Nonstandard Graph or Chart)
Combo of Web Scraping and leaflet or plotly
A dashboard page with multiple charts that update the same data
a "thick"? Server????????
- Project should include at least one JS Library that we did not cover
- Project must be powered by a data set with at least 100 records
- Project must include some level of user-driven interaction
- Final Visualization should include at least 3 view

<!DOCTYPE html>
<!I used https://www.w3schools.com/bootstrap4/default.asp to create my starter code for this assignment. >
<html lang="en">
<head>
  <title>Project 2</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.16.0/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
  <style>
  .fakeimg {
    height: 200px;
    background: rgb(243, 245, 247);
  }
  </style>
</head>
<body>

<div class="jumbotron text-center" style="margin-bottom:0">
  <h1>Project 2</h1>
  <p>
At this point of our project, we are analizing the data nesscary to create our visuals which will soon be shared with on this page.
  </p> 
</div>


<div class="container" style="margin-top:30px">
  <div class="row">
    <div class="col-sm-4">
      <h2></h2>
      <p></p>
      <img class="rg_i Q4LuWd" src="data:image/png;base64,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" data-deferred="1" jsname="Q4LuWd" width="225" height="225" alt="Listening is everything - Spotify" data-iml="1215.0800000090385" data-atf="true">

  
      


<div>   </div>
      <h3>Links</h3>
      <p>Below are the links for our data set and visualization inspiration.</p>
      <ul class="nav nav-pills flex-column">
        <li class="nav-item">
          <a class="nav-link active" href="#">Hope Page</a>
        </li>
        <li class="nav-item">
          <a class="Data Set Link" href="https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks/discussion">Link to Dataset</a>
        </li>
        <li class="nav-item">
          <a class="3D Graph Link" href="https://www.nytimes.com/interactive/2015/03/19/upshot/3d-yield-curve-economic-growth.html">Link to 3D Graph Inspiration </a>
        </li>
        <li class="nav-item">
            <a class="Line Graph Link" href="https://www.kaggle.com/arunkothari/spotify-trends">Link to Graph Inspiration </a>
          </li>

      </ul>
      <hr class="d-sm-none">
    </div>
    <div class="col-sm-8">
        <h2>In our data analysis we plan on creating:</h2>
        <li>Time Analysis on music characteristics long-term (3-D Chart)</li>
        <li>Shorter term focus on how music characteristics changed in 2020 (zoom from above/interaction)</li>
        <li>Predict popular characteristics in 2021 to 2025</li>
        <li>Recommend popular newer songs in 2020-2021 based on user inputs</li>
        <li>Pop, Rock, Hip Hop, Country, Electronic/EDM genre user inputs</li>
        <br>
      
      </div>
  </div>
</div>
<br>
<h2>TITLE HEADING</h2>
<p>Some text..</p>
<p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
</div>

<div class="jumbotron text-center" style="margin-bottom:0">
  <p> Spotify project by Gabby Martin, Kaleb Nieman, Brian Young, and David High, presented on February 2nd, 2021.
  </p>
</div>

</body>
</html>

