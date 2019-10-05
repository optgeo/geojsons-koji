# geojsons-koji
GeoJSONS for koji

総務省統計局の[平成27年国勢調査町丁・字等別境界データ](https://www.e-stat.go.jp/gis/statmap-search?page=1&type=2&aggregateUnitForBoundary=A&toukeiCode=00200521&toukeiYear=2015&serveyId=A002005212015&coordsys=1&format=shape)を加工して利用

# build
```console
git clone git@github.com:optgeo/geojsons-koji
cd geojsons-koji
rake
```
# properties: example
```json
{
"properties": {
    "AREA": 48473.27,
    "AREA_MAX_F": null,
    "CITY": "219",
    "CITY_NAME": "下田市",
    "CSS_NAME": null,
    "DUMMY1": "-",
    "GST_NAME": "下田市",
    "H27KAxx_": 1123,
    "H27KAxx_ID": 1122,
    "HCODE": 8101,
    "JINKO": 0,
    "KBSUM": 0,
    "KCODE1": "0000-00",
    "KEN": "22",
    "KEN_NAME": "静岡県",
    "KEYCODE1": "219000000",
    "KEYCODE2": null,
    "KEY_CODE": "22",
    "KIGO_D": null,
    "KIGO_E": null,
    "KIGO_I": null,
    "KIHON1": "0000",
    "KIHON2": "00",
    "MOJI": null,
    "N_CITY": null,
    "N_KEN": null,
    "PERIMETER": 1317.373,
    "PREF": "22",
    "PREF_NAME": "静岡県",
    "SETAI": 0,
    "SITYO_NAME": null,
    "S_AREA": "000000",
    "S_NAME": null,
    "X_CODE": 138.94161,
    "Y_CODE": 34.57509
  }
}
```
