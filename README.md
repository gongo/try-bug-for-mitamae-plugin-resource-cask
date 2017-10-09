Test
==============================

```console
$ curl -LO https://github.com/itamae-kitchen/mitamae/releases/download/v1.5.1/mitamae-x86_64-darwin
$ chmod +x mitamae-x86_64-darwin

$ mkdir plugins
$ cd plugins/
$ git clone https://github.com/k0kubun/itamae-plugin-resource-cask.git
$ cd ../

$ ./mitamae-x86_64-darwin local roles/mac.rb

 INFO : Starting MItamae...
trace:
	[1] /home/mruby/code/mrblib/mitamae.rb:2:in __main__
	[2] /home/mruby/code/mrblib/mitamae/cli.rb:4:in start
	[3] /home/mruby/code/mrblib/mitamae/cli.rb:17:in run
	[4] /home/mruby/code/mrblib/mitamae/cli/local.rb:33:in run
	[5] /home/mruby/code/mrblib/mitamae/recipe_loader.rb:17:in load
	[6] /home/mruby/code/mruby/mrblib/enum.rb:61:in map
	[7] /home/mruby/code/mruby/mrblib/array.rb:17:in each
	[8] /home/mruby/code/mruby/mrblib/enum.rb:61:in map
	[9] /home/mruby/code/mrblib/mitamae/recipe_loader.rb:18:in load
	[10] /home/mruby/code/mrblib/mitamae/recipe.rb:9:in load
	[11] /home/mruby/code/mruby/mrbgems/mruby-object-ext/mrblib/object.rb:16:in tap
	[12] /home/mruby/code/mrblib/mitamae/recipe.rb:11:in load
	[13] /Users/gongo/Workspaces/src/github.com/gongo/try-bug-for-mitamae-plugin-resource-cask/roles/mac.rb:1:in instance_eval
	[14] /home/mruby/code/mrblib/mitamae/recipe_context.rb:123:in include_recipe
	[15] /home/mruby/code/mruby/mrbgems/mruby-object-ext/mrblib/object.rb:16:in tap
	[16] /home/mruby/code/mrblib/mitamae/recipe_context.rb:124:in include_recipe
	[17] /Users/gongo/Workspaces/src/github.com/gongo/try-bug-for-mitamae-plugin-resource-cask/cookbooks/cask/default.rb:1:in instance_eval
/Users/gongo/Workspaces/src/github.com/gongo/try-bug-for-mitamae-plugin-resource-cask/cookbooks/cask/default.rb:1:undefined method 'cask' for #<MItamae::RecipeContext:0x10085bd88> (NoMethodError)
```
