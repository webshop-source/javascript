Code Sample for Ajax Username Check:
Javascript 
$('#username').on('blur', function () {
  $.ajax({
    url: 'check_username.php',
    type: 'POST',
    data: { username: $(this).val() },
    success: function (response) {
      $('#userMsg').html(response); }});});
