Add your answers to the Algorithms exercises here.

## Exercise I




## Exercise II

I would start out by going to the half way point of the floors (`f/2`). I would then drop an egg. If they egg breaks then I know that the egg will break on every floor above `f/2`. I would drop the next egg at the half way point of the lower floors (`(f/2)/2`). If the egg broke at that height I now know that the egg will break after being dropped from anything above that floor. Next I would go to half of that floor so (`((f/2)/2)/2`) If the egg still broke I would continue halving the floors until I got an egg that didn't break. I would then go up half as may floors. If it doesn't break I would go up half again but if it does break I would go down half again. Until the egg doesn't break.

