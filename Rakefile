desc 'Runs jekyll serve with the --safe and --baseurl "" options.'
task :serve do
  system('jekyll serve --baseurl --incremental ""')
end

desc 'Runs jekyll build.'
task :build do
  system('jekyll build ')
end

desc 'Runs jekyll clean.'
task :clean do
  system('jekyll clean ')
end

desc 'Resume'
task :resume do
  system('pandoc -t markdown ~/Git/Personal/resume/Andy\ Choens\ -\ Resume.tex > ~/Git/Personal/choens.github.io/about/resume/index.md')
end

desc 'Projects'
task :projects do
  system('pandoc -t markdown ~/Git/Personal/resume/Andy\ Choens\ -\ Example\ Projects.tex > ~/Git/Personal/choens.github.io/about/projects/index.md')
end
