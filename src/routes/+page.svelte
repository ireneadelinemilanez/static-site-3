<!--
  This is you page!
-->
<script>
  // Import all the news furniture components
  import ArticleHeader from '$lib/components/ArticleHeader.svelte';
  import ArticleBody from '$lib/components/ArticleBody.svelte';
  import ImageWithCaption from '$lib/components/ImageWithCaption.svelte';
  import RelatedLinks from '$lib/components/RelatedLinks.svelte';

  // Article metadata
  let headline = 'Bed-Stuy Mutual Aid Groups Rally to Feed Neighbors';
  let byline = 'Irene Adeline Milanez';
  let pubDate = '2025-12-16';

  // Related stories
  const relatedStories = [
    { headline: 'How America\'s top news organizations escape rigid publishing systems to design beautiful data-driven stories on deadline.', href: 'https://palewi.re/docs/coding-the-news/' },
    { headline: 'How to install, configure and use Visual Studio Code, GitHub and Copilot', href: 'https://palewi.re/docs/coding-the-news/scripts/week-1/' },
  ];
</script>

<!-- This sets the page title in the browser tab -->
<svelte:head>
  <title>{headline} | NYCity News Service</title>
  <meta name="description" content="At the Craig Newmark Graduate School of Journalism at the City University of New York, change is in our DNA. That comes of being born in 2006, as the digital revolution was transforming our profession in ways none of us could have imagined." />
</svelte:head>

<!-- Your page content goes here -->
<div class="container">
  
  <!-- Article Header: Headline, byline, and publication date -->
  <ArticleHeader
    {headline}
    {byline}
    {pubDate}
  />

  <!-- Lead Image: CUNY Journalism School building -->
  <ImageWithCaption
    src="/snap.jpg"
    alt="The Craig Newmark Graduate School of Journalism is at 219 West 40th Street in Midtown Manhattan."
    caption="Bed-Stuy residents bundled in puffer jackets line up for Bed-Stuy Strong’s food distribution at Herbert Von King Park in Bed-Stuy, Brooklyn on Tuesday, November 11, 2025."
    credit="Craig Newmark Graduate School of Journalism"
  />

  <!-- Article Body: The main story text with proper typography -->
  <ArticleBody>
    <p>
      Snow sprinkled as volunteers from mutual aid network Bed-Stuy Strong organized crates of milk, eggs, kale and apples at Herbert Von King Park on Nov. 11. Bundled in puffer jackets, area residents formed a line that followed hand-drawn signs welcoming all to collect free groceries.
    </p>

    <p>
Jackson Fratesi, volunteer with Bed-Stuy Strong since the COVID-19 pandemic, said the group planned the distribution after learning that November SNAP benefits would be delayed because of the government shutdown. 

    </p>

    <p>
“Bed-Stuy Strong sprung up in response to the pandemic when people were really in need,” he said. “This is just another time, but neither of these, unfortunately, are totally unique. It’s the responsibility of communities to take care of each other.”

    </p>

    <p>
Over at Restoration Plaza on Fulton St., City Council Member Chi Ossé distributed Thanksgiving baskets organized by volunteers from Exalt Youth and Muna Social Services. In groups of ten at a time, mostly elderly Bed-Stuy residents received bags of pantry staples, produce and meat. 

    </p>

    <p>
“We’re hearing the calls to our district office,” Ossé said.“This was a president who said that he ran on affordability and making America great, but he’s letting innocent people starve.”

    </p>

    <p>
According to city data, more than 40,000 Bed-Stuy residents who rely on SNAP benefits saw their monthly grocery budgets shrink at the start of November. With food pantries strained and underresourced, mutual aid groups, local government and community-led efforts continue to fill the gaps left by SNAP. 

    </p>

    <p>
Although food stamp payments have been restored, some SNAP recipients will now have to work or be in approved job training for at least 80 hours a month. The new law now includes work requirements for adults up to 64 years old, raised from 54 years old, and ended exemptions for homeless people, veterans and former foster youth. Many non-citizens who previously qualified, including refugees and asylum-seekers, will lose SNAP eligibility. Most recipients will see these changes applied at their next recertification. 

    </p>

    <p>
Ossé said his office has held weekly food distributions for the past four years, but has seen an influx of both recipients and volunteers since the beginning of November.

    </p>

    <p>
“In this time of a dangerous, threatening and hostile government, it’s really amazing to see the community take care of each other to keep us safe,” he said.

    </p>
  </ArticleBody>

  <!-- Related Stories: Links to other articles -->
  <RelatedLinks
    title="Related Stories"
    links={relatedStories}
  />

</div>

<style>
  /* Styles here only apply to this page */
  .container {
    padding: var(--spacing-lg) var(--spacing-md);
  }
</style>