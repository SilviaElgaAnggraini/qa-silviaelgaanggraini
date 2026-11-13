// Tahun di footer
document.getElementById('year').textContent = new Date().getFullYear();

// Form kontak: kalau YOUR_FORM_ID belum diganti (Formspree), buka aplikasi email dengan isi terisi
var form = document.getElementById('cf');
form.addEventListener('submit', function (e) {
  if (form.action.indexOf('YOUR_FORM_ID') < 0) return;
  e.preventDefault();
  var d = new FormData(form);
  location.href = 'mailto:silviaelgaanggraini@gmail.com?subject=' +
    encodeURIComponent('Portfolio message from ' + d.get('name')) +
    '&body=' + encodeURIComponent(d.get('message') + '\n\n' + d.get('email'));
});