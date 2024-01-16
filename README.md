<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Resim Galerisi</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

  <style>
    .container {
        border: 5px solid #3cb371;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        transition: box-shadow 0.3s ease-in-out;
    }
  </style>
</head>
<body>
    <div class="container">
        <div class="row">
            <h1 class="text-center text-success my-3">---RESİM GALERİSİ---</h1>
        </div>
        <div class="row">
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card" >
                    <img src="https://picsum.photos/id/16/800" class="card-img-top" alt="Deniz" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/12/800" class="card-img-top" alt="Sahil" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/19/800" class="card-img-top" alt="Ağaç Kökü" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/95/800" class="card-img-top" alt="Ağaç" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/38/800" class="card-img-top" alt="Bulut" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/66/800" class="card-img-top" alt="Doğa" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/94/800" class="card-img-top" alt="Merdiven" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/674/800" class="card-img-top" alt="Üzüm" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
            <div class="col-lg-4 col-md-6 col-sm-12 mb-4">
                <div class="card">
                    <img src="https://picsum.photos/id/41/800" class="card-img-top" alt="Damla" data-bs-toggle="modal" data-bs-target="#resimDetay">
                </div>
            </div>
        </div>
    </div>
    <h6 class ="text-center text-success my-3">Published by Azimenur Yıldız on January 16 2024</h6>

   <div class="modal fade" id="resimDetay" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
       <div class="modal-dialog modal-dialog-centered"> 
            <div class="modal-content"> 
               <div class="modal-body">
                 <img id="modal-image" src="" class="card-img-top" alt="Manzara">
              </div>
              <div class="modal-footer">
                 <button type="button" class="btn btn-danger text-success" data-bs-dismiss="modal">Close</button>
              </div>
            </div>
       </div>
   </div>


  <script>
    document.querySelectorAll(".card img").forEach(el => {
        el.addEventListener('click', () => {
            let src = el.getAttribute("src");

            let modalImage = document.getElementById("modal-image");
            modalImage.setAttribute("src", src);
        });
    });
  </script>
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>