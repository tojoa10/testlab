Welcome to the Galaxy {{ site_name }} {{ lab_name }}! 



<!-- example grid system with links, 

note that many of the sections here are not yet actual sections as yml files, just here for examples

to link to a section, see what it is called in the yml file (it's id, on the first line)
then add Section, so data becomes dataSection

-->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Bootstrap Grid</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" />
  <style>
    body {
      background-color: white;
    }

    .grid-item {
      background-color: #cce5ff;
      border-radius: 10px;
      padding: 20px;
      text-align: center;
      font-size: 1em;
      font-weight: bold;
      transition: 0.3s;
      height: 100%;
      width: 100%;
    }

    .grid-item a {
      text-decoration: none;
      color: #0056b3;
      display: block;
      height: 100%;
    }

    .grid-item:hover {
      background-color: #99c2ff;
    }
  </style>
</head>
<body>

<div class="container mt-3">
  <div class="row g-2">
    <!-- Row 1 -->
    <!-- these get named for the sections that are in the yml files. 
    Look in the yml file and see what the "id" is at the top of the file
    then add that in here, with "Section" after it
    eg the Import Data section refers to the data.yml file
    which has id = import
    so to link to that data.yml file, add in #importSection
    don't forget the #
    -->
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#importSection">Import Data</a></div>
    </div>
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#qcSection">Quality Control</a></div>
    </div>
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#microbialSection">Microbial Profiling</a></div>
    </div>
    <!-- Row 2 -->
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#rnaseqSection">RNASeq</a></div>
    </div>
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#learnSection">Learn Galaxy</a></div>
    </div>
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#helpSection">Galaxy Help</a></div>
    </div>
    <!-- Row 3 -->
    <div class="col-md-4 d-flex">
      <div class="grid-item flex-fill"><a href="#agrfSection">Contact AGRF</a></div>
    </div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

