# terminal_talk


### print skull and crossbones using UTF-8 
```term
 $ echo -e "\xE2\x98\xA0" 
```

- in one terminal 

```term
 $ nc -l 1234
```
    
- then in irb
```ruby
require 'socket' s = TCPSocket.new 'localhost',1234
s.write "Hello Terminal"
s.write "\nput\nme\non\na\nnew\nline".encode(Encoding::ASCII)
```
## Questions to answer
- What kind of bytes am i sending with this mehtod by default?
  - It seems to be unicode (UTF-8?)
  - But I can force ASCII for escapes
  - What about unicode escapes?
-builtins std utils and core UNIX programs
Add user 

