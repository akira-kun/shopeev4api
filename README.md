# shopeev4api
Simplest API for shopee v4

change params [shopid,itemid] to grab any product info OR
exclude itemid from the url params and set limit to 999 to return all the products from any shopid


code
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


result
```
{
   "bff_meta":null,
   "error":0,
   "error_msg":null,
   "data":{
      "update_time":1685371438,
      "version":"1685371438",
      "sections":[
         {
            "total":135,
            "key":"shop_page_product_tab_main_sec",
            "index":[
               {
                  "data_type":"item",
                  "key":"item::8751544103",
                  "filtered":null,
                  "filtered_dunit":null
               }
            ],
            "data":{
               "item":[
                  {
                     "itemid":8751544103,
                     "shopid":285650840,
                     "name":"Roupa Tematica SUPER MARIO BROS ou LUIGI Fantasia",
                     "label_ids":[
                        1000022,
                        1006602,
                        700065053,
                        700070074,
                        1583603,
                        1428775,
                        298413358,
                        1593633
                     ],
                     "image":"br-11134207-7qukw-lf360p6zyj8r16",
                     "images":[
                        "br-11134207-7qukw-lf360p6zyj8r16",
                        "5c7c1c6773afba8128e8eadf9ce2afa2",
                        "8daed5d091f286d156dcef3d5bdd12c9",
                        "9d1166efda7fae78fab473f4e9cf2269",
                        "br-11134201-23010-gbfl522vsfmv30",
                        "br-11134207-7qukw-lf360p6zx4ob76",
                        "br-11134207-7qukw-lf360p6zzxt705"
                     ],
                     "currency":"BRL",
                     "stock":35,
                     "status":1,
                     "ctime":1620148251,
                     "sold":98,
                     "historical_sold":314,
                     "liked":false,
                     "liked_count":992,
                     "view_count":null,
                     "catid":100633,
                     "brand":"",
                     "cmt_count":157,
                     "flag":0,
                     "cb_option":0,
                     "item_status":"normal",
                     "price":5500000,
                     "price_min":5500000,
                     "price_max":6990000,
                     "price_min_before_discount":-1,
                     "price_max_before_discount":-1,
                     "hidden_price_display":null,
                     "price_before_discount":0,
                     "has_lowest_price_guarantee":false,
                     "show_discount":0,
                     "raw_discount":0,
                     "discount":null,
                     "is_category_failed":null,
                     "size_chart":"",
                     "video_info_list":[
                        
                     ],
                     "tier_variations":[
                        {
                           "name":"TAMANHO",
                           "options":[
                              "MARIO SIMPLES P-1A2 ANOS",
                              "MARIO SIMPLES - M-3-4 ANOS",
                              "LUIGI SIMPLES - P 1 A 2 ANOS",
                              "LUIGI SIMPLES M-3-4 ANOS",
                              "LUIGI COM LUVA - G 5 A 6 ANOS",
                              "MARIO COM LUVA - M 3 A 4 ANOS",
                              "MARIO COM LUVA G 5 A 6 ANOS",
                              "MARIO COM LUVA - P 2ANOS",
                              "LUIGI COM LUVA - 3 A 4 ANOS"
                           ],
                           "images":[
                              "br-11134207-7qukw-lf360p701cdn03",
                              "br-11134207-7qukw-lf360p702qy31c",
                              "br-11134207-7qukw-lf360p7045ij94",
                              "br-11134207-7qukw-lf360p705k2z11",
                              "br-11134207-7qukw-lf360p6zvq3v03",
                              "br-11134207-7qukw-lf360p6zubjf83",
                              "br-11134207-7qukw-lf360p6zswyz5f",
                              "br-11134207-7qukw-lgmn9zo3txf969",
                              "br-11134207-7qukw-lgmn9zo3vbzpaa"
                           ],
                           "properties":[
                              
                           ],
                           "type":0
                        }
                     ],
                     "item_rating":{
                        "rating_star":4.738853503184713,
                        "rating_count":[
                           157,
                           4,
                           2,
                           5,
                           9,
                           137
                        ],
                        "rcount_with_image":57,
                        "rcount_with_context":94
                     },
                     "item_type":0,
                     "reference_item_id":"",
                     "transparent_background_image":"",
                     "is_adult":false,
                     "badge_icon_type":0,
                     "shopee_verified":true,
                     "is_official_shop":false,
                     "show_official_shop_label":false,
                     "show_shopee_verified_label":true,
                     "show_official_shop_label_in_title":false,
                     "is_cc_installment_payment_eligible":false,
                     "is_non_cc_installment_payment_eligible":false,
                     "coin_earn_label":null,
                     "show_free_shipping":false,
                     "preview_info":null,
                     "coin_info":null,
                     "exclusive_price_info":null,
                     "bundle_deal_id":0,
                     "can_use_bundle_deal":false,
                     "bundle_deal_info":null,
                     "is_group_buy_item":null,
                     "has_group_buy_stock":null,
                     "group_buy_info":null,
                     "welcome_package_type":0,
                     "welcome_package_info":null,
                     "add_on_deal_info":null,
                     "can_use_wholesale":false,
                     "is_preferred_plus_seller":false,
                     "shop_location":"São Paulo",
                     "has_model_with_available_shopee_stock":false,
                     "voucher_info":null,
                     "is_on_flash_sale":false,
                     "spl_installment_tenure":null,
                     "is_live_streaming_price":null,
                     "shop_name":"PersonalizadosDaBella",
                     "shop_rating":4.82056,
                     "is_mart":false,
                     "pack_size":null,
                     "overlay_image":null,
                     "autogen_title":null,
                     "autogen_title_id":null,
                     "overlay_id":null,
                     "is_service_by_shopee":false,
                     "free_shipping_info":null,
                     "global_sold_count":314,
                     "repurchase_rate":0,
                     "best_selling_tag":0,
                     "flash_sale_stock":0,
                     "flash_sale_design_style":null,
                     "flash_sale_label_content":null,
                     "flash_sale_sold_percentage":null,
                     "info":"AB:5078_8351_35973|7905_11689_59740,REQID:1f8a1b84fcd61de40295573619ac1602,BND:shop_page_product_tab_main,QUE:spop_v1,QUES:spop_v1,RNK:shop_unify_v5_hinet_v2@BR_47181:{SCORE:1.949500},SECKEY:shop_page_product_tab_main_sec",
                     "data_type":"item",
                     "key":"item::8751544103",
                     "count":0,
                     "adsid":0,
                     "campaignid":0,
                     "deduction_info":"",
                     "video_display_control":0,
                     "deep_discount_skin":null,
                     "experiment_info":null,
                     "relationship_label":"",
                     "live_stream_session":null,
                     "new_user_label":null,
                     "wp_eligibility":null,
                     "platform_voucher":null,
                     "rcmd_reason":null,
                     "highlight_video":null,
                     "can_use_cod":false,
                     "pub_id":"",
                     "pub_context_id":"1f8a1b84fcd61de40295573619ac1602",
                     "friend_relationship_label":"",
                     "showing_rs_label":null,
                     "showing_friend_rs_label":null,
                     "show_flash_sale_label":false,
                     "search_id":"",
                     "ext_info":"",
                     "product_banners":null,
                     "top_product_label":null,
                     "fashion_item":null,
                     "image_search":null
                  }
               ],
               "keyword":null,
               "ads":null,
               "top_product":null,
               "collection":null,
               "item_lite":null,
               "voucher":null,
               "voucher_detail":null,
               "l1cat":null,
               "collection_lite":null,
               "l2cat":null,
               "shop":null,
               "shop_lite":null,
               "shopcat":null,
               "feed":null,
               "feed_tab":null,
               "stream":null,
               "promotion":null,
               "knode":null,
               "food_item":null,
               "l3cat":null,
               "video":null,
               "image_search_item":null
            },
            "item_card_type":"",
            "section_meta_data":null,
            "has_more":false,
            "pagination_type":"streaming"
         },
         {
            "total":85,
            "key":"shop_page_product_tab_main_sosec",
            "index":[
               
            ],
            "data":{
               "item":null,
               "keyword":null,
               "ads":null,
               "top_product":null,
               "collection":null,
               "item_lite":null,
               "voucher":null,
               "voucher_detail":null,
               "l1cat":null,
               "collection_lite":null,
               "l2cat":null,
               "shop":null,
               "shop_lite":null,
               "shopcat":null,
               "feed":null,
               "feed_tab":null,
               "stream":null,
               "promotion":null,
               "knode":null,
               "food_item":null,
               "l3cat":null,
               "video":null,
               "image_search_item":null
            },
            "item_card_type":"",
            "section_meta_data":null,
            "has_more":false,
            "pagination_type":"streaming"
         }
      ],
      "expire":1685371438,
      "tab_meta_data":null,
      "misc_info":null,
      "realtime_meta_data":null,
      "user_meta_data":{
         "is_new_user":false
      }
   }
}
```

```
view image with https://down-br.img.susercontent.com/file/[code-from-json-result]
https://down-br.img.susercontent.com/file/br-11134207-7qukw-lf360p701cdn03
```
