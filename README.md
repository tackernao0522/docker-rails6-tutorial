# Section3 List3.5 hello ActionをApplicationコントローラに追加

```
class ApplicationController < ActionController::Base

  def hello
    render html: "hello, world"
  end
end
```

+ `src/config/routes.rb`を編集<br>

```
Rails.application.routes.draw do
  root 'application#hello'
end
```
