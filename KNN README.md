# Background

You just woke up. You think you heard your phone ringing, but you're just imagining things. The room looks kind of unfamiliar. All you remember is being out last night. "Whose apartment is this? What's with the overdone rustic look. They've kind of taken it too far. Did I go home with someone?" you ask, racking your brain super hard. Hmm... &#x1F914; You don't remember meeting anyone you were particularly attracted to. It's all a blur, except for that very old, lanky white man with the long beard and pointy hat. He used a staff just as tall as him to support his old frame. And why the heck was he in a robe. Meh, you brush the thought away and scan the room. Your eyes catch what looks like a ticket on a bedside stand. Apart from those items, yourself, and the bed there's nothing more in the room. 

Studying the ticket a second time, a few things stand out: "RMS Titanic". That's odd, is it a movie ticket? You remember your partner bawling their eyes out watching *Titanic* a few movie nights ago. You focus back on the ticket. Boarding pass, yadda yadda third class yadda yadda, "Date: 10th April 1912". Wait! Nooooo! It can't be!....



---
.

.

The RMS Titanic was a British passenger liner operated by the White Star Line that sank in the North Atlantic Ocean in the early morning hours of April 15, 1912, after striking an iceberg during her maiden voyage from Southampton to New York City. Of the estimated 2,224 passengers and crew aboard, more than 1,500 died, making the sinking one of modern history's deadliest peacetime commercial marine disasters.

### Defining the question

Using the provided data, Can we design a model that correctly categorizes passengers aboard the *Titanic* as either survivors, or deceased? 

### Metric for success

Heavy is the head that wears the crown. A gargantuan task lies before you. After reading the background section, surely the objective is clear. You want the model to tell which passengers have lowest chances of surviving so that you know where to focus your efforts when you time-travel back to 1912. **THESE ARE HUMAN LIVES**, so we want 100% accuracy. That's the bar. No room for error!

More realistically, we can shoot for **80 percent**

### Experimental design choices

We will use a the K Nearest neighbors classifier for this model, with varying test and train sizes and K values, to see how these changes affect our accuracy.

### Appropriateness of the data to answer our question

The total number of passengers on the ill-fated Titanic was 2,224. Of those, we had 1317 passengers. Our data comprises 891 records. It is important to note that our dataset does not capture accomodation and boarding details for any of the staff, so we can't predict their survival rates. The missing 60 percent of the data may drastically improve our model if added to our data.

However, we do have 67 percent of passenger data which is a pretty darn good sample size as far as predicting PASSENGER survival goes.
