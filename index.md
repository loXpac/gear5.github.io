---
layout: home
title: Cinema's Golden Age
subtitle: Has there even ever been such a thing ?
cover-img: "/assets/img/nevjuice.jpg"
---

## Lights, Camera, and ... Action !
<div style="text-align: justify;">
  <p>
    Cinema has always been a mirror to society, showcasing both the highs and lows, being the canvas for the cultural statement and creating narratives that are worldwide, as well as more geographically inclined.
  </p>
  <p>
    The question of whether there is a "Golden Age" of cinema — a point in time of outstanding creativity, cultural impact, and economic success — still continues to be a passionate subject of exploration.
  </p>
  <p>
    Let's dive into different snapshots of the industry, through various datasets, in order to assess if a metric can be defined to quantify the success of a specific genre, or the industry as a whole. This, will then allow us to identify significant eras, and predict trends that may shape the industry's future.
  </p>
  
  <p>
    You might wonder where one would even start and know what defines a successful movie ? Is it it's box office revenue, is it how known it is, how popular it is with critics and fans ? How many languages it has been translated to or how many countries it has been distributed in ?  
  </p>

  <p>
    Worry not, as we have found the Industry's Secret 11 herbs and Spices, let's look at them together, and see if you can also figure it with us ! 
  </p>

  <p>
  The first question you might ask yourself probably relates to what will be cooking with ? What different ingredients do we have at disposition, what about the genres that are comprised within the huge coop that is the global movie industry.  
  </p>
</div>
<div style = "display: flex; justify-content: center;">
 <iframe src="assets/plots/genre_piechart.html" style="width: 100%; height: 620px; border: none;"></iframe>
</div>

<div style = "text-align: justify;">
  <p>
    The first conclusion from this lovely distribution is that this lovely industry is quite a complex mix of genres. <br/> <br/>
    Drama is the big winner, and by far, with a choke hold on nearly 14 % of the movies in our data (one might say ever, but let's not get too much ahead of ourselves). Comedy comes in, in a not so close second at about half of drama movies produced, with Romance rounding up the podium. <br/>
    Only the top 20 movies were shown, as the 366 different genres would result in quite crowded donut... <br/> <br/>
    The top 20 movies genres are still within the answers one would think about when trying to figure a genre, however there are some slightly more obscure ones further down the distribution. It might be better not to focus on the 2 movies on the Netherlands in World War II genre, so we will mostly focus on those better top 15 genres throughout the showdown. 
  </p>

  <p>
    Now, let's see what features one would need to chose to get a good recipe for a success metric !
  </p>

</div>

<div style = "display: flex; justify-content: center;">
 <iframe src="assets/plots/movie_metrics_all_genres.html" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

<div style="text-align: justify;">
  Well, well, well, what do we have here ? <br/> <br/>
  Let us begin by looking at the Number of movies by genre over time.<br/>
  The first thing to notice is that for nearly every genre, the production rate as massively increased since the beginning of movie production, bar a few exceptions.<br/>
  Let's first start with the number of movies throughout the past century; there are few trends emerging already... <br/> <br/>
  
<ol>
  <li>
  The most common trend is the simple exponential increase in movie production throughout the years, with representative genres like Drama or World Cinema. One can also see the small step-like plateaus in the increase, maybe implying small saturations every decade or so.
  </li>

  <li>
    The next interesting shape is how the Indie Genre underwent a rebirth, with many movies produced from the 1910s to 1930s, then a pseudo-death of the medium until a new life was instilled in the genre by the 60s. Could that be the transition from independent movie producers to big studio conglomerates, until the return of the amateur as technology got more accessible ?
  </li>

  <li>
    Finally, on a sadder note, some genres simply did not survive or just fell off. Yes, we're talking about you Mr. Black & White, or Ms. Silent. They simply weren't the same after the 60s and 30s respectively.
  </li>
</ol>

<p>
  What about a more common way of defining success, such as box office revenue, adjusted for inflation of course ! <br/>
  Here we can see the same trend emerging as before, with a slight mix up in the main players. With Drama, Action and Adventure now the highest grossing genres, Short Films and Musicals once earned some serious money, but those days are long gone.
</p>

<p>
  The next feature that one would need to analyze would be the popularity of a movie. This is pulled from the IMDB website and dataset, and calculated based on how a movie is perceived by the the online audience compared to the rest of the movies available, see it as a nice and friendly contest which rewards heavily popular movies, thus putting an emphasis on movies that are currently enjoyed as well as all time great movies. <br/>
  Here, we can see a few trends appear out of our delicious data :
  <ol>
    <li>
      An increase in popularity, in more recent movies for genres such as Action, Adventure or even Crime Fiction. 
    </li>

  <li>
      A stable popular view for Genres like World Cinema, which seems to be enjoyed for any of its movies equally.
  </li>

  <li>
    And a more appreciative view of old movies and more recent ones with a gap in the middle for genres like Black & White, or Indie.
  </li>
  </ol>
  One must note the lack of popularity score for some genres, either irregularly or before a set time, due to the data acquisition from this shared dataset, as well as how the score itself is given with a vast majority of low popularity scores, with some ultra popular scorers. Yes, Adventure we can see that peak.
</p>

<p>
  For the next feature, we wanted to be nice and chew up the work a bit for you, we thus collected a big chunk of reviews online, fed them through a RoBERTa Sentiment Analysis (SA)pipeline, and thus obtained a score from -1 (highly negative review) to 1(most certainly a great time) that we added for each year of a genre thus giving the mean SA score for that year. <br/>
  Hence, the very nature of this score is dependant on the availability of reviews for this movie, big gaps may occur...
  A general trend though is that the mean SA score is at least slightly positive with greater variation on years not in the 90s to 2010s (where a consensus was seemingly reached, or reviews simply started to be boringly similar).
</p>

<p>
  Last, but not least the Average Rating was obtained and is similar in nature to the SA Score in how it portrays our data, with coming from the same dataset a lack of data points. It also possesses the same 20 year quirk with this weird consensus...
</p>

<p>
  Great ! We now have collected all the Secret Ingredients for a Killer Recipe ! <br/>
  What comes next is to assemble the Avengers, and save Marvel and the Movie Industry from making boring movies for the rest of our lives... Hard task, but heroes must be brave. <br/> <br/>
  Let's see how our success metric can be assembled to have a coherent view on the industry.
</p>
</div>

## Act I : A New Metric Awakens

<div style="display: flex; justify-content: center;">
 <img src="assets/plots/success_metric_histogram.png" style="width: 50%;"/>
 <img src="assets/plots/movie_success_hexbin.png" style="width: 50%;"/>
</div>

<div style="text-align: justify;">
  Voluptate deserunt elit ad officia enim voluptate duis nostrud culpa sint do laborum ad. Cupidatat amet enim aliqua esse eiusmod amet. Ut enim elit ad nostrud do eu sit sint tempor culpa ea dolor. Nisi exercitation elit id Lorem commodo culpa. Eiusmod irure velit ea id incididunt labore sint deserunt tempor. Eiusmod commodo voluptate ut exercitation et ipsum nulla.
</div>

<div style="text-align: center;">
 <iframe src="assets/plots/bubble_plot.html" style="width: 100%; height: 620px; border: none;"></iframe>
</div>

<div style="text-align: center;">
 <iframe src="assets/plots/success_score_distribution.html" style="width: 100%; height: 620px; border: none;"></iframe>
</div>

<div style="text-align: center;">
 <iframe src="assets/plots/top_movies_vertical_radiobuttons.html" style="width: 100%; height: 620px; border: none;"></iframe>
</div>

<div style="text-align: center;">
<iframe src="assets/plots/precomputed_choropleth_fixed_colorbar.html" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

<div style="text-align: center;">
<iframe src="assets/plots/horbar.html" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

## Act II : Tell Me More

<div style="text-align: justify;">
  Duis laborum pariatur sint culpa duis amet exercitation. Veniam consequat tempor labore consequat reprehenderit amet irure pariatur dolore proident occaecat pariatur voluptate. Aliquip eu velit magna laboris fugiat veniam sint officia eiusmod minim deserunt magna.
</div>

## Act III : I Can Now See the Way

<div style="text-align: justify;">
For the final act of our grand data journey, we gazed into the crystal ball and predicted future trends in the movie industry. To do this, we combined the data of our success metric for each genre and projected their influence on the movie industry. This allowed us to compare the impact of each genre over time. When calculating the impact, we focused on two main points:
</div>

- Scaling: More successful movies have more of an impact. Makes sense right?
- Causality: No time travelling in this movie! We do not want the success of a movie to have an impact before it's release.

<div style="text-align: justify;">
Also, to keep the graphs visually pleasing, we are only going to keep genres with more than 3000 movies. This represents a total of 19 genres!
</div>

<div style="text-align: center;">
<iframe src="assets/plots/StackedImpactOverTime.png" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

<div style="text-align: justify;">
We can check if these impact timeseries are in agreement with the golden ages we found in the previous parts. To better visualize this, we can normalize the impact for each genre and plot them over time to find the following plot:
</div>

<div style="text-align: center;">
<iframe src="assets/plots/NormalizedGenreImpact.png" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

<div style="text-align: justify;">
From these graphs, one thing is clear: The movie industry is thriving! We can see a real explosion of the impact over the recent years. This can in part be explained by our dataset having more data about recent movies. 
</div>

<div style="text-align: justify;">
Another interesting thing to note is that eventhough all genres seem to be experiencing a golden age in recent year, there are two outliers: Black-and-White movies and Silent films. They experienced their golden age in the 40's and in the 30's respectively. 
</div>

<div style="text-align: justify;">
Finally, even before gazing into the crystal ball, we can see that Comedy films have experienced a sudden growth in recent years. This may indicate a future golden age for this genre in the future. However, this remains to be seen from our predictions. 
</div> 

<div style="text-align: justify;">
One last thing we can do before looking at the prediction is evaluating the relative impact of each genre for different time periods.
</div> 

<div style="text-align: center;">
<iframe src="assets/plots/relativeImpactRadar.html" style="width: 100%; height: 500px; border: none;"></iframe>
</div>

<div style="text-align: justify;">
We can see from this graph the slow decline of the Black-and-White movies who once represented more than 35% of the impact. This domination has been replaced by the Dramas throughout the 60's until the 2010's. However, this domination seems to be slowing down, with new genres emerging such as Thrillers, Action movies and Comedies. But enough said about the past. Let's now look into the future!
</div>



## As The Curtains Close

<div style="text-align: justify;">
  Excepteur pariatur qui reprehenderit mollit aliqua voluptate. Voluptate nisi amet ex ea esse velit laboris deserunt Lorem aute. Laborum pariatur elit magna qui. Cillum et irure adipisicing officia. Duis laborum pariatur sint culpa duis amet exercitation. Veniam consequat tempor labore consequat reprehenderit amet irure pariatur dolore proident occaecat pariatur voluptate. Aliquip eu velit magna laboris fugiat veniam sint officia eiusmod minim deserunt magna.
</div>
