require './lib/search.rb'

namespace :search do
  task :split do
    Docsplit.extract_text(Dir['./docs/*.[pP][dD][fF]'], output: './docs')
  end

  namespace :table do
    task :create do
      Search::Table.create!
    end

    task :load do
      Search::Table.load!
    end
  end
end
