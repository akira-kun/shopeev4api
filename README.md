# shopeev4api
Simplest API for shopee v4

change params [shopid,itemid] to grab any product info OR
exclude itemid from the url params to return all the products


```
<div id="test"></div> 

<script>
fetch(`https://api.allorigins.win/get?url=${encodeURIComponent('https://shopee.com.br/api/v4/recommend/recommend?bundle=shop_page_product_tab_main&limit=1&offset=0&shopid=285650840&itemid=8751544103')}`)
.then(response => {
	if (response.ok) return response.json()
	throw new Error('Network response was not ok.')
})
.then(data => document.getElementById("test").innerHTML = data.contents);
</script>
```
