require 'rake-jekyll'

Rake::Jekyll::GitDeployTask.new(:deploy) do |t|
    # Description of the rake task.
    t.description = 'Generate the site and push changes to remote repository'

    # Run this command to build the site.
    t.build_script = ->(dest_dir) {
        puts "\nRunning Jekyll..."
        sh "bundle exec jekyll build"
    }
end
