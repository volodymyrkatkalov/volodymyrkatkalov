```ruby
#!/usr/bin/env ruby
# frozen_string_literal: true

class SoftwareEngineer
  attr_reader :name, :roles, :languages, :email

  def initialize
    @name = "Volodymyr Katkalov"
    @email = "volodymyr.katkalov@gmail.com"
    @languages = ["en_US", "bg_BG", "zh_CN"]

    @roles = [
      "Frontend Developer",
      "Backend Developer",
      "Fullstack Developer",
      "DevOps Engineer",
      "Test Automation Developer",
    ]

    @wrote = %w[Perl Python PHP Ruby C# JavaScript Go Rust]

    @into = ["AI", "LLMs", "agents", "harnesses", "orchestration"]

    @post_ironic_repos = {
      "go-ai-isodd" => "Why do the math yourself when you can ask an AI? I asked. In a repository.",
      "go-ai-iseven" => "One parity package was not enough, so I shipped the other sign too.",
    }

    @meta_ironic_repos = {
      "slopc" => "Slap #[slop] on a signature and pray.",
    }
  end

  def say_hi
    puts name
    puts "Did #{roles.join(', ')}."
    puts "An LLM does that now too. Better than me :)"
    puts "Wrote #{@wrote.join(', ')}."
    puts "Currently into #{@into.join(', ')}, etc."
    puts
    puts "Post-ironic:"
    @post_ironic_repos.each do |repo, line|
      puts "  #{repo} — #{line}"
      puts "  https://github.com/volodymyrkatkalov/#{repo}"
    end
    puts "Meta-ironic:"
    @meta_ironic_repos.each do |repo, line|
      puts "  #{repo} — #{line}"
      puts "  https://github.com/volodymyrkatkalov/#{repo}"
    end
    puts
    puts email
  end
end

SoftwareEngineer.new.say_hi
```
