# Writing a Ruby on Rails application without using a database model

-----------------
-----------------
This is an approach

In **app/models/tableless.rb**:

```
class Tableless < ActiveRecord::Base
  def self.columns
    @columns ||= [];
  end

  def self.column(name, sql_type = nil, default = nil, null = true)
    columns << ActiveRecord::ConnectionAdapters::Column.new(name.to_s, default,
      sql_type.to_s, null)
  end

  # Override the save method to prevent exceptions.
  def save(validate = true)
    validate ? valid? : true
  end
end
```

In **app/models/foo.rb**:

```
class Foo < Tableless
  column :bar, :string  
  validates_presence_of :bar
end
```

In **script/console**:

Loading development environment (Rails 2.2.2)

```
>> foo = Foo.new
=> #<Foo bar: nil>
>> foo.valid?
=> false
>> foo.errors
=> #<ActiveRecord::Errors:0x235b270 @errors={"bar"=>["can't be blank"]}, @base=#<Foo bar: nil>>
```

-----------------
-----------------
The other method:
https://github.com/remiprev/her

