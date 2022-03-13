# Total-number-of-comments
Total number of comments
$.ajax({

  url: "/feeds/comments/default?alt=json-in-script",

  type: "get",

  dataType: "jsonp",

  success: function(data) {

    var totalcomments = data.feed.openSearch$totalResults.$t;

    $('.total-comments').html(totalcomments);

  }

});
