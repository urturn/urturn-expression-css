require "json"

desc "Compile the css"
task :compile do
  system("compass compile && git add css")
end

task :install do
  puts("install Git pre-commit hook")
  system("cp git-pre-commit-hook .git/hooks/pre-commit")
  system("chmod u+x .git/hooks/pre-commit")
end

task :publish do
  puts("tag a new version of urturn-expression-css")
  version = JSON.parse(File.read("package.json"))['version']
  system("git tag v#{version}")
  system("git push && git push --tags")
end

task :precommit => :compile