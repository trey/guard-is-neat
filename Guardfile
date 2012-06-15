guard 'sass', :input => 'assets/source/sass', :output => 'assets/compiled/css'
guard 'coffeescript', :input => 'assets/source/coffeescript', :output => 'assets/compiled/js'

guard 'process', :name => 'minify-css', :command => 'juicer merge assets/compiled/css/all.css -o public/css/all.min.css --force -s' do
  watch /^assets\/compiled\/css\/all.css/
end

guard 'process', :name => 'minify-js', :command => 'juicer merge assets/compiled/js/all.js -o public/js/all.min.js --force -s' do
  watch /^assets\/compiled\/js\/all.js/
end
