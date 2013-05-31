desc "Compile the css"
task :compile do
  system("compass compile && git add css")
end

task :install do
  puts("install Git pre-commit hook")
  system("cp git-pre-commit-hook .git/hooks/pre-commit")
  system("chmod u+x .git/hooks/pre-commit")
end

task :precommit => :compile