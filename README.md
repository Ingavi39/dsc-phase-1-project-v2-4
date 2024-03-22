# Phase one project

## Overview  

Microsoft is considering entry into the movie industry, driven by observations of thriving ventures within the sector. Seeking guidance, they aim to discern the optimal film attributes conducive to box office success. Leveraging comprehensive movie data encompassing worldwide and domestic box office revenue, production budget, genre classification, and runtime, our objective is to elucidate correlations among these variables and cinematic success metrics. This analytical endeavor aims to furnish Microsoft with actionable insights, guiding informed decision-making processes toward crafting high-earning cinematic endeavors.

## Business Understanding
Microsoft's venture into the realm of cinema will undoubtedly be facilitated by addressing crucial inquiries such as:

1. **Genre Prioritization**: Identifying the genres that resonate most with audiences and align with Microsoft's brand ethos will streamline their entry strategy. By pinpointing the genres where they can offer unique perspectives or capitalize on existing strengths, Microsoft can effectively carve out its niche in the competitive landscape.

2. **Optimal Film Length**: Understanding the ideal duration for a movie is pivotal in captivating audience attention while ensuring narrative coherence. By exploring audience preferences and industry trends, Microsoft can tailor its productions to strike the perfect balance between engagement and storytelling depth.

3. **Budget Allocation and Performance**: Analyzing the correlation between budget allocation and movie performance is essential for maximizing returns on investment. While a substantial budget can afford top-notch production values and star talent, prudent resource allocation is key to achieving commercial success. Microsoft must assess whether higher investment translates to enhanced audience reception and critical acclaim.

4. **Competitive Landscape**: Identifying potential studio competitors is imperative for Microsoft to navigate the industry landscape effectively. By studying both emulation-worthy studios for best practices and potential direct competitors for differentiation strategies, Microsoft can position itself strategically in the market and capitalize on untapped opportunities.

Addressing these fundamental questions will not only streamline Microsoft's entry into the movie industry but also lay a robust foundation for sustainable growth and creative innovation in the cinematic domain.

# Data Understanding
Firstly, we begin by importing all important python libraries and files
Next, we need to get the size and information on each dataset. This is important because it will help us pick the datasets that can best fit our goal.

We can see that the 'movie_budgets', 'TMD_movies' and 'movie_info' are the top 3 while 'Bom_movies' comes last.
Now while the amount of data is important for reliability, what the data says is just as, if not more important as it will be easier to accomplish what we have set out to do.
So we must qualitatively decide which datasets to pick out

The best data sets to use will be:
- **'Movie_budgets'** as it gives use both domestic and worldwide gross, as well as the movie budget
- **'Movies_info'** as it gives use the runtime as well as the genre of the movie
- **'Bom_movies'** can be used to see which studio does best at the box office 
Though 'TMDB' HAD alot more data the was no highly distiguishing variable to measure a likely hood of success. It does not provide a genre, age rating, runtime, budget. Only the date, which I beleive is not strong enough of a reason to contribute to a films success.

# Data preparation 
In this section, we clean the data, removing rows with missing values, adding median values to a few missing rows, making any strings that are numerical into floats or integers

# Data Analysis
We will calculate the correlation between runtime and gross as well as budget to gross. We will use both Pearson and Spearman's correlation coefficient for a more reliable result

The correlations between runtime and gross are positive but not strong and therefore we can no with confidence say that runtime positively affects correlation as the relationship is very weak.
![alt text](image-2.png)
![alt text](image-3.png)

However the correlations between budget and gross are very strongly positive. This suggests movies with bigger budgets tend to earn more money.
![alt text](image-4.png)
![alt text](image-5.png)

From this analysis we can see that BV(Disney) is the highest earning studio by over a billion
![alt text](image-6.png)

We can also determine that Comedy is the genre that performs the best
![alt text](image-7.png)

# Conclusions
There are four key recommendations from analyizing the data:
1. **Microsoft's Flexibility Regarding Movie Length**:
   - Microsoft's involvement in the film industry offers a unique opportunity to explore different approaches to movie length without being constrained by traditional norms. Unlike traditional studios, Microsoft does not need to adhere to a specific movie length to ensure success. Whether a film is long or short may not significantly affect its overall growth or reception by audiences. This flexibility allows Microsoft to experiment with storytelling formats and cater to diverse audience preferences without the pressure of conforming to established conventions.

2. **Investment Strategy and Revenue Potential**:
   - To maximize revenue potential from their film ventures, Microsoft should adopt a strategic approach to investment, recognizing that higher-budget productions often yield greater returns. By investing substantially in film budgets, Microsoft can enhance production values, attract top talent, and create high-quality cinematic experiences that resonate with audiences worldwide. This willingness to invest significantly in their film projects can position Microsoft as a major player in the industry and pave the way for blockbuster successes.

3. **Emulating Successful Studios Like Disney**:
   - Microsoft can learn valuable lessons from successful studios like Disney, particularly in terms of brand building, content creation, and market dominance. Emulating Disney's strategies, such as recruiting experienced executives from the company or developing intellectual properties (IPs) with similar prestige and appeal, can bolster Microsoft's standing in the film industry. By leveraging Disney's proven formula for success, Microsoft can increase its market share and compete more effectively in an industry where Disney consistently outperforms its rivals by substantial margins.

4. **Focusing on High-Grossing Genres, Particularly Comedy**:
   - Analyzing trends in box office performance reveals that comedy films consistently rank among the highest-grossing genres. Recognizing this trend, Microsoft should prioritize the production of comedy films to capitalize on their commercial appeal and audience demand. By creating entertaining and humorous content that resonates with viewers, Microsoft can tap into a lucrative market segment and generate significant revenue streams. Moreover, comedy films often have broad demographic appeal, making them accessible to diverse audiences worldwide and enhancing Microsoft's global reach and profitability in the film industry.

   # Potential limitations 
- Correlation is not causation 
- Data does not take into account other factors contibuting to a films success such as a film's critical reception,   innovative marketing strategies and cultural relevance 
- Data excludes popular films that are streamed but not released in theatres (Netflix films)
There may be hidden costs that arent included in film budgets such as marketing