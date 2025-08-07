+++
title = 'Montréal - Houston by Train'
"blog/tags" = [ "Travel"]
date = "2025-06-08"
draft=false
+++

# That Time I Travelled Montréal - Houston by Train

In April 2025, I had to travel from Montréal in Québec to Houston, Texas to attend the ISBI25 conference. 
Of course the cheapest, and fastest, option was the plane with a direct flight of 4 hours.
But, concerned about the environmental impact of such a trip, I asked friends researching Life Cycle Analysis (LCA) and Carbon Accounting to help me compare between plane and train for this trip.

For this, I first had to determine what route I would take. As train is quite bad in North America, you need some tricks to find a train-only itinerary without too many changes. I asked a friend of mine who did a similar trip before, he gave me a helpful piece of advice : "Go to Chicago, from there you can go anywhere" (paraphrased).

Playing with the Amtrak website for a few days, I ended up with two possible itineraries :
- Montréal -> New York -> Chicago -> Houston : a trip of 74 hours with 54 hours spent in the train
- Montréal -> New York -> New Orleans -> Houston : 79 hours with 52 in the train

Clearly, it's a commitment. For the round trip, I would have to spend 7 to 8 days travelling. All this to go to a 4 days conference. On the other hand, taking the plane for a just 4 days could be considered a waste of resources if the plane option really emitted more carbon than the train one.

Now that we have the options, let's see the results ! Here is what my friends gave me :

<style type="text/css">
table {
    width: fit-content;
    align-self: center;
}
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px 0px;
  overflow:hidden;padding:10px 10px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:2px 0px;
 overflow:hidden;padding:10px 10px;word-break:normal;}
.tg .tg-cly1{text-align:left;vertical-align:middle; border-width:0px 0px 2px 0px;}
.tg .tg-lboi{border-color:inherit;text-align:left;vertical-align:middle}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
.tg .tg-0lax{text-align:left;vertical-align:top}
.tg .tg-end{text-align:left;vertical-align:top; border-width:0px 0px 2px 0px;}
</style>
<table class="tg"><thead>
  <tr>
    <th class="tg-0pky"></th>
    <th class="tg-0pky">Itinerary</th>
    <th class="tg-0pky">Multiplicative <br> Factor</th>
    <th class="tg-0pky">Two Way Emissions<br> (kgCO2eq)</th>
    <th class="tg-0pky">Saved Emissions <br>   (kgCO2eq) </th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-lboi" rowspan="2">Plane</td>
    <td class="tg-lboi" rowspan="2">Montréal -&gt; Houston</td>
    <td class="tg-0pky">2</td>
    <td class="tg-0pky">825</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">3</td>
    <td class="tg-0pky">1237</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-cly1" rowspan="2">Train</td>
    <td class="tg-0lax">Montréal -&gt; NY -&gt; <br>
     Chicago -&gt; Houston</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">581</td>
    <td class="tg-0lax">244 to 656</td>
  </tr>
  <tr>
    <td class="tg-end">Montréal -&gt; NY -&gt; <br>
     New Orleans -&gt; Houston</td>
    <td class="tg-end"></td>
    <td class="tg-end">568</td>
    <td class="tg-end">257 to 669</td>
  </tr>
</tbody>
<caption> Emissions Estimation for a Round Trip</caption>
</table>

Some details about the method :
- Emissions per passenger:
  -  Airplane: \(emissions = d \times FE_{\text{airplane}} \times M\)
        -  \(d\) : distance (mile)
        -  \(FE_{\text{airplane}}\): emission factor for a medium-haul airplane (kgCO2eq.passenger \(^{-1}\).mile \(^{-1}\)))
        -   \(M\): multiplier representing potential non-CO2 effects (2 or 3 according to the literature)
    -   Train: \(emissions = d \times FE_{\text{train}} \times M\)
- Emission factors, calculated from the emission factors of the [US EPA](https://www.epa.gov/climateleadership/ghg-emission-factors-hub) (2025) and the [GWP100 of the AR6](https://ghgprotocol.org/sites/default/files/2024-08/Global-Warming-Potential-Values%20%28August%202024%29.pdf)
  -  Airplane: 0.13 kgCO2eq.passenger \(^{-1}\).mile \(^{-1}\)
  -  Train: 0.15 kgCO2eq.passenger \(^{-1}\).mile \(^{-1}\) (“Intercity Rail - Other Routes (other than Northeast Corridor)”)
        - Diesel train very likely

In my case, taking the train would avoid up to half a ton of CO2eq which is a quarter of the 2 tons per person per year that we need to reach by 2050. It is not a negligible gain.

Once cleared by my supervisor, I took my tickets. All of them in coach, obviously, the price for a bed being way too high for anyone to justify in an expense report. Quite happily, Amtrak's seats are wide with ample leg space. Quite sadly, the train is not a popular option in the US, so you will most likely have the second seat to lie down and rest. 

Now let's talk about the reason that made me write this : **it was so cool** ! 

First, the train is comfortable and calm and I found it weirdly relaxing. In the superliners, you will find observation deck which are so enjoyable. Being able to spend hours looking at the country through the panoramic windows is one of the best things I experienced in this trip. 

Secondly, I worked on my master's thesis and on an article for most of the trip to Houston. The absence of a space for a second screen and the lack of powerful enough Wi-Fi made it impossible to watch a video while working (very bad work habit) and, in general, to be distracted. I just had enough connection to go on Overleaf and check some results on my lab computer through SSH. This made me so focused that I wrote the entire article and most of my thesis in these 3 days !

The blend between being able to deeply focus while enjoying the scenery made me realize how overstimulated I was back in my normal life. This experience changed me, I try to spend less time watching content as a background noise to avoid being bored. Doing creative things, such as writing this probably poor blog post, make me much more happy and involved than any content I have watched. 

I am a strong defender of the idea that we need to rethink how we live our lives. I think travel is a good example of such thing. At the beginning, I took this decision to avoid carbon emission, expecting the travel to be more of a trial of my commitment than a pleasure. Now, I want to choose the slower way for any travel. I hope that, in a very near future, this approach to travel will be the default one, fast travel being saved for real emergencies.

As researchers, a capital part of our work is to discuss and diffuse our research. But we are not a class of citizen above the rest, we can not expect others to stop travelling by plane so that we can continue to do it. I think promoting slower travel in academia can be an efficient way to fight this problem. (Splitting conferences in multiple venues is also a very good idea ! See [EurIPS](https://www.eurips.cc/))

I hope this was an interesting post and that my English is good enough to convey my ideas!