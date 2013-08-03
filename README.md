def procnew
new_proc = Proc.new { return "I got here..." }
new_proc.call
return "...but not here."
end
def lambdaproc
new_proc = lambda { return "You get here..." }
new_proc.call
return "And I got here!"
end
puts lambdaproc
→
And I got here!
puts procnew
→
I got here...

