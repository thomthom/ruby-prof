# ruby_prof for SketchUp 2017+

This fork is a dirty hack to get RubyProf operating under SketchUp 2017+.
RubyProf used to work within SketchUp out of the box, but with SketchUp 2017 it
started working properly. It's not clear if it's due to upgrading to Ruby 2.2
or something else. (Maybe Chromiums processes or message pump is
interfering... ?)

[See more detailed comment `in ruby_prof.c`](ext/ruby_prof/ruby_prof.c#L137)

## Building

1. Install the matching standalone version of Ruby.
2. Install DevKit for Ruby
3. Open a console window with Ruby DevKit enabled. (`C:\RubyDevKit\x64\devkitvars.bat`)
4. `cd ext/ruby_prof`
5. `ruby extconf.rb`
6. `make`

I have not been able to
