```ruby
#!/usr/bin/env ruby
# frozen_string_literal: true

# Volodymyr Katkalov — Sofia
# The last revision of this file was a skill hash and a career ladder.
# A model freshened it. I kept both kinds of truth.

class SoftwareEngineer
  attr_reader :name, :where, :mail, :speaks

  def initialize
    @name   = "Volodymyr Katkalov"
    @where  = "Sofia, Bulgaria"
    @mail   = "volodymyr.katkalov@gmail.com"
    @speaks = %w[en bg zh]

    # The job did not get an AI rewrite. The guest still has to boot.
    @role = "test automation for virtualization — openQA, os-autoinst"

    @languages = %w[Perl Python Rust Go C Ruby JavaScript]
    # PHP and C# are still in the toolbox. They did not ask for a relaunch.

    # Sincere. Do not refactor this into a punchline.
    @praise = [
      "reads the red job, the callers, and the 2019 comment before having a take",
      "pays the boilerplate tax and does not sigh about it in the message",
      "holds the whole diff while I am still on the second hunk",
      "does not get bored of the third reproduction. I do. that is the product",
    ]

    # Also sincere. That is the outage.
    @irony = [
      "ships confidence and calls it a result",
      "uses \"you're absolutely right\" where a type checker was supposed to go",
      "a helper, a factory for the helper, then a manifesto, for n % 2",
      "offered to center this file and add the word passionate. the file declined",
      "the dream is fluent. the types are a negotiation. rustc skips the TED talk",
    ]
  end

  # One of these has no model in the loop. The bytes are right or they are not.
  def exhibits
    {
      "slopc" => "#[slop] on a signature. hallucinated body. compiler is the reviewer that cannot be flattered",
      "go-ai-isodd" => "a round trip to a model to learn what Integer#odd? already published",
      "go-ai-iseven" => "the control group. rigor is a second invoice",
      "kmp_merge" => "overlapping snapshots, Knuth–Morris–Pratt, no oracle in the loop",
      "try-omarchy" => "Omarchy inside a Mac. the hypervisor is serious. the premise is a dare",
    }
  end

  # Same rule slopc already runs in production.
  def policy
    "let it draft. let something that cannot be charmed say no."
  end

  def ask(question)
    # Answers before the question mark. Occasionally answers a nearby question.
    "You're absolutely right — #{question} changes everything."
  end

  def say_hi
    puts "#{name}, #{where}"
    puts @role
    puts "speaks #{speaks.join(', ')}  ·  writes #{@languages.join(', ')}"
    puts
    puts "on the record:"
    @praise.each { |line| puts "  + #{line}" }
    puts "also on the record:"
    @irony.each { |line| puts "  - #{line}" }
    puts
    exhibits.each { |repo, why| puts "  #{repo} — #{why}" }
    puts
    puts policy
    puts ask("is 2 even")
    puts "mail: #{mail}"
  end
end

SoftwareEngineer.new.say_hi if __FILE__ == $PROGRAM_NAME
```
