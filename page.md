#分页  
```js
  function ajax(url, callback) {

  var xhr = new XMLHttpRequest();

  xhr.open('GET', url, true);

  xhr.onreadystatechange = function() {

    if (xhr.readyState === 4 && xhr.status === 200) {
      callback(xhr.responseText);
    }

  };
  xhr.send();
}
function getPageData(pageNo) {
  ajax('/page' + pageNo + '.html', function(data) {
    document.getElementById('container').innerHTML = data;
  });
}

getPageData(1);
```
