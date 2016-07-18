function createRequest() {
  var result = null;
  if (window.XMLHttpRequest) {
    result = new XMLHttpRequest();
    if (typeof xmlhttp.overrideMimeType != 'undefined') {
      result.overrideMimeType('text/xml'); // Or anything else
    }
  }
  else if (window.ActiveXObject) {
    result = new ActiveXObject("Microsoft.XMLHTTP");
  } 
  return result;
}

