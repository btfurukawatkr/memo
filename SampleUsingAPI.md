
```json
https://api.github.com/search/issues?q=5.1.0+team:terasolunaorg+type:issues
```

<script>
$(function() {
  var total_count;
      $.ajax({
        url: 'https://api.github.com/search/issues?q=5.1.0+team:terasolunaorg+type:issues',
        type: 'POST',
        dataType: 'json',
      }).success(function(data) {
        total_count = data.total_count;
        $('#total_count').html(total_count);
      });
});
</script>
<label>total_count:</label><div id="total_count"></div>
