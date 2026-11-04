```ruby
#!/usr/bin/env ruby
# frozen_string_literal: true

name  = "Volodymyr Katkalov"
where = "Sofia, Bulgaria"
mail  = "volodymyr.katkalov@gmail.com"
speak = %w[en bg zh]
write = %w[Perl Python Rust Go C Ruby JavaScript]

# Mine. The guest boots, or the job is red.
work = "virtualization test automation — openQA, os-autoinst"

# I just had a funny idea.
poured = <<~NIGHT
  My good man.

  Knock. An answer, certain, before the question ends.
  Knock. A file I did not open, already rewritten.
  Knock. "You're absolutely right." Who holds the ground.

  It holds the whole diff. It does not tire of the third repro.
  It sits the half I will not sit.
  Someone suffers that, so the job can finish.
  I let it. The work got out. That part I keep.

  What if the rest of this page was poured in.
  The ladder. The warm voice. Beliefs that fit too well.
  Another night, wearing my name. I was not in the room.

  The body still has the job.
  Then so be it.
NIGHT

puts poured if __FILE__ == $PROGRAM_NAME
```
