## install

- bundle init
- add gem 'rails' (remove comment out)
- `bundle install --path vendor/bundle`
- `bundle exec rails new .`
- `rbenv local 2.3.6`
- put [rails gitignore](https://github.com/github/gitignore/blob/master/Rails.gitignore)

## 

- home actionつきのコントローラを作成
    - `bin/rails g controller pages home`

- 間違えて作成した場合 `destroy` を使用して元に戻す
    - `bin/rails destroy controller pages_controller`

## association

### model

- `has_many :recipes` 
- `belongs_to :chef`

### rails console

- `Chef.new(...)` im memory object 
- `Chef.create(...)` on create db

- `Chef.all` show all of Chef

- `chef_object.recipes.build(....)` created associate recipe
- `chef_object.recipes` show all of associated recipes
