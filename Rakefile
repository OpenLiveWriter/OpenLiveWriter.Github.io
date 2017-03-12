require "stringex"

# This rakefile will provide rake tasks to make it easier to manage a Jekyll blog

## -- Misc Configs -- ##
posts_dir    = "_posts"    # directory for blog files
new_post_ext = "md"  # default new post file extension when using the new_post task

desc "Generate the website using Jekyll"
task :generate do
  puts "## Generating site with Jekyll"
  system "jekyll build"
end

desc "Preview the generated website in a browser and keep watching for changes"
task :preview do
  puts "## Serving the generated site to localhost:4000 and watching for changes"
  jekyllPid = Process.spawn("jekyll serve")

  trap("INT") {
    Process.kill(9, jekyllPid) rescue Errno::ESRCH
    exit 0
  }

  Process.wait(jekyllPid)
end

desc "Begin a new blog post in /_posts. Use as rake new_news_item[title,author,file-extension]. In absence of any of those, the values will be asked for interactively."
task :new_blog_post, [:title, :author, :extension] do |t, args|
  if args.title
    title = args.title
  else
    puts("Enter a title for your post: ")
    title = STDIN.gets.chomp
  end

  if args.author
    author = args.author
  else
    puts("Enter your GitHub username: ")
    author = STDIN.gets.chomp
  end

  if args.extension
    new_post_ext = args.extension
  else
    puts("Enter the file extension you want to use: ")
    new_post_ext = STDIN.gets.chomp
  end

  filename = "#{posts_dir}/#{Time.now.strftime('%Y-%m-%d')}-#{title.to_url}.#{new_post_ext}"
  if File.exist?(filename)
    abort("rake aborted!") if ask("#{filename} already exists. Do you want to overwrite?", ['y', 'n']) == 'n'
  end
  puts "Creating new post: #{filename}"
  open(filename, 'w') do |post|
    post.puts "---"
    post.puts "layout: default"
    post.puts "title: \"#{title.gsub(/&/,'&amp;')}\""
    post.puts "date: #{Time.now.strftime('%Y-%m-%d %H:%M:%S %z')}"
    post.puts "categories: [blog]"
    post.puts "author: #{author}"
    post.puts "download: true"
    post.puts "---"
  end
end

desc "Begin a new news post in /_posts. Use as rake new_news_item[title,author,file-extension]. In absence of any of those, the values will be asked for interactively."
task :new_news_item, [:title, :author, :extension] do |t, args|
  if args.title
    title = args.title
  else
    puts("Enter a title for your post: ")
    title = STDIN.gets.chomp
  end

  if args.author
    author = args.author
  else
    puts("Enter your GitHub username: ")
    author = STDIN.gets.chomp
  end

  if args.extension
    new_post_ext = args.extension
  else
    puts("Enter the file extension you want to use: ")
    new_post_ext = STDIN.gets.chomp
  end

  filename = "#{posts_dir}/#{Time.now.strftime('%Y-%m-%d')}-#{title.to_url}.#{new_post_ext}"
  if File.exist?(filename)
    abort("rake aborted!") if ask("#{filename} already exists. Do you want to overwrite?", ['y', 'n']) == 'n'
  end
  puts "Creating new post: #{filename}"
  open(filename, 'w') do |post|
    post.puts "---"
    post.puts "layout: default"
    post.puts "title: \"#{title.gsub(/&/,'&amp;')}\""
    post.puts "date: #{Time.now.strftime('%Y-%m-%d %H:%M:%S %z')}"
    post.puts "categories: [news]"
    post.puts "author: #{author}"
    post.puts "download: true"
    post.puts "---"
  end
end

desc "Begin a new release post in /_posts. Use as rake new_release[version-number,author,file-extension]. In absence of any of those, the values will be asked for interactively. The fully formed title becomes 'Open Live Writer version-number is now available!'."
task :new_release, [:version, :author, :extension] do |t, args|
  if args.version
    version = args.version
  else
    puts("Enter the version number (The fully formed title becomes 'Open Live Writer version-number is now available!'): ")
    version = STDIN.gets.chomp
  end
  title = "Open Live Writer #{version} is now available!"

  if args.author
    author = args.author
  else
    puts("Enter your GitHub username: ")
    author = STDIN.gets.chomp
  end

  if args.extension
    new_post_ext = args.extension
  else
    puts("Enter the file extension you want to use: ")
    new_post_ext = STDIN.gets.chomp
  end

  filename = "#{posts_dir}/#{Time.now.strftime('%Y-%m-%d')}-#{title.to_url}.#{new_post_ext}"
  if File.exist?(filename)
    abort("rake aborted!") if ask("#{filename} already exists. Do you want to overwrite?", ['y', 'n']) == 'n'
  end
  puts "Creating new post: #{filename}"
  open(filename, 'w') do |post|
    post.puts "---"
    post.puts "layout: default"
    post.puts "title: \"#{title.gsub(/&/,'&amp;')}\""
    post.puts "date: #{Time.now.strftime('%Y-%m-%d %H:%M:%S %z')}"
    post.puts "categories: [news, release]"
    post.puts "author: #{author}"
    post.puts "download: true"
    post.puts "---"
  end
end
