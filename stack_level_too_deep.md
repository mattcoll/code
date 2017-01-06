STACK LEVEL TOO DEEP

means something is repeating infinitely

what ever gem is not working

Go into bin/{gem} then remove

~ rm bin/rake

Then add it back

~ bundle binstubs rake


OR ---------


Remove all binstubs and reinstall

~ rm bin/*

~ bundle install --binstubs

________________________________________________________

link to help: https://github.com/rbenv/rbenv/wiki/Understanding-binstubs
