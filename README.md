```ruby
#!/usr/bin/env ruby

class SoftwareEngineer
  attr_reader :name, :roles, :languages, :email, :skills
  
  def initialize
    @name = "Volodymyr Katkalov"
    @roles = [
      "Frontend Developer",
      "Backend Developer",
      "Fullstack Developer",
      "DevOps Engineer",
      "Test Automation Developer (current)"
    ]
    @languages = ["en_US", "bg_BG", "zh_CN"]
    @skills = {
      programming_languages: ["Perl", "Python", "PHP", "Ruby", "C#", "JavaScript"],
      testing: ["Selenium", "Cypress", "PyTest", "OpenQA"],
      devops: ["Linux", "Docker", "Kubernetes", "OpenShift"],
      databases: ["PostgreSQL", "MongoDB", "Redis"]
    }
    @email = "volodymyr.katkalov@gmail.com"
  end

  def say_hi
    puts "Thanks for dropping by, hope you find some of my work interesting."
    puts "Roles: #{roles.join(' → ')}"
    puts "Skills:"
    skills.each do |category, items|
      puts "  #{category.to_s.split('_').map(&:capitalize).join(' ')}: #{items.join(', ')}"
    end
    puts "In case you want to contact me feel free to drop me a line to #{email}"
  end
end

me = SoftwareEngineer.new
me.say_hi
```
