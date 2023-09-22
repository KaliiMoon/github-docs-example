# Writing Good Documentation

## Step 1 - Using Codeblocks.

Codeblocks in markdown make it *very easy* for tech people to __copy, paste, share code__.
A good __Cloud Engineer__ uses Codeblocks whenever possible.

Because it allows others to copy and paste their code to replicate of research issues.

```ruby
class Person
  attr_accessor :name, :age

  def initialize(name, age)
    @name = name
    @age = age
  end

  def introduce
    puts "Hi, I'm #{@name}, and I'm #{@age} years old."
  end

  def celebrate_birthday
    @age += 1
    puts "#{@name} is now #{@age} years old! Happy Birthday!"
  end
end

# Create two person objects
person1 = Person.new("Alice", 30)
person2 = Person.new("Bob", 25)

# Introduce the people
person1.introduce
person2.introduce

# Celebrate their birthdays
person1.celebrate_birthday
person2.celebrate_birthday
```


- When you can you should attempt to apply syntax highlighting to your codeblocks.

<img width="200px" src="https://github.com/KaliiMoon/github-docs-example/assets/132712673/262f8913-65b9-424d-9690-ecbc3885d28b" />

Good Cloud Engineers use codeblocks for both Code and Errors that appear in the console.

```bash
def divide(a, b)
  result = a / b
  return result
end

begin
  result = divide(5, 0)
rescue ZeroDivisionError => e
  puts "Error: #{e.message}"
  puts e.backtrace
end
```

> Here is an example of using a codeblock for an error that appears in bash.

## Step 3 - Use Github Flavoured Markdown Task Lists

Github extends Markdown to have a list where you can check off items. [<sup>[2]</sup>](#external-references)

- [x] Finish Step 1
- [ ] Finish Step 2
- [x] Finish Step 3

# Step 4 - Use Emojis (Optional)

Github Flavored Markdown (GFM) supports emoji shortcodes.
Here are some examples:

| Name | Shortcode | Emoji |
| --- | --- | --- |
| flower | `:sunflower:` | 🌻: |
| cresent moon | `:crescent_moon:` | :crescent_moon: |

# Step 5 - how to create a table

You can use the following markdown format to create tables:

```md
| Name | Shortcode | Emoji |
| --- | --- | --- |
| flower | `:sunflower:` | 🌻: |
| cresent moon | `:crescent_moon:` | :crescent_moon: |
```

Github extends the functionality of Markdown tables to provide more alignment and table cell formatting options. [<sup>[1]</sup>](#external-references)


 ## External References

 - [GH Doc Examples](https://github.com/KaliiMoon/github-docs-example/edit/main/README.md) 
 - [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
 - [GFM - (Tables with ext)](https://github.github.com/gfm/#tables-extension-) <sup>[1]</sup>
 - [GFM - Emoji CheatSheet](https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)
 - [GFM - Task Lists](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#task-lists) <sup>[2]</sup>

 
 
