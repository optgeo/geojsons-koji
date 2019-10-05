# https://www.e-stat.go.jp/gis/statmap-search/data?dlserveyId=A002005212015&code=08&coordSys=1&format=shape&downloadType=5

task :default do
  %w{08 09 10 11 12 13 14 19 20 22}.each {|pref|
    url = "https://www.e-stat.go.jp/gis/statmap-search/data?" +
      "dlserveyId=A002005212015&code=#{pref}&coordSys=1&" + 
      "format=shape&downloadType=5"
    sh "curl -o #{pref}.zip '#{url}'"
    sh "unzip #{pref}.zip"
    sh "rm #{pref}.zip"
    sh "rm #{pref}.geojsons" if File.exist?("#{pref}.geojsons")
    sh "ogr2ogr -f GeoJSONSeq #{pref}.geojsons h27ka#{pref}.shp"
    sh "rm h27ka#{pref}.*"
  }
end

