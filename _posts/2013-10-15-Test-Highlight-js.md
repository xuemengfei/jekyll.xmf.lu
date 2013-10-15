---
layout: post
date: 2013-10-15 14:25:00
title: Test highlight.js
category: test
---

### Descriptions

Seeing people's actual work is just as important as what they say. Seeing people work their through exercises live might be even more important. These are some exercises that aren't particularly difficult and anybody with CSS experience should be able to do. Watching/listening to them do it could be invaluable. Collab Mode on CodePen is kinda perfect for that (just saying).

Accessible and semantic image replacement has been a CSS topic for a lot of years and the "best way" has morphed over the years. Asking them to show you how it could be done a number of ways would be a way to get insight into how long they've really been working with CSS. Not only is it directly an important thing to know how to do, knowing how to do it multiple ways demonstrates the depth of their internal toolbox.

### Javascript

```javascript
  var lang = {
    'en': {
      confirm: 'Are you sure?',
      loading: 'Loading...'
    },
    'zh_cn': {
      confirm: '确定删除？',
      loading: '提交中...'
    }
  }
```

<!-- more -->

### CSS

```css
  * {
    margin: 0;
    padding: 0;
    -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
  }

  html {
    overflow-y: scroll;
    -webkit-overflow-scrolling: touch;
    -webkit-text-size-adjust: 100%;
  }

  body {
    color: #333333;
    font: 14px/1.5 "Helvetica Neue", Helvetica, Arial, sans-serif;
  }

  a {
    color: #0088cc;
    text-decoration: none;
  }
  a:hover {
    color: #005580;
    text-decoration: underline;
  }

  button, input, select, textarea {
    font: inherit;
    font-size: 100%;
    vertical-align: baseline;
  }

  button {
    *overflow: visible;
  }
  button::-moz-focus-inner {
    padding: 0;
    border: 0;
  }

```

### Ruby

```ruby
  class DocsController < BaseController
    require 'format_transformation/flash_tool'
    include FilesHelper

    skip_before_filter :app_login, :only => [:preview_html5]

    def new
      @file = DbFile.new(:filetype => :document)
      @title = t('files.document')
      choose_folder
    end
  end
```
