# bell_rss_feed_section

**Bell RSS HTML Section**

Easily integrate the latest RSS feeds from Bell Network into your website with our simple HTML snippet. Customize the appearance and behavior of the feed to suit your needs, and get real-time updates by using a straightforward URL.

**HTML Structure:**

    <!-- RSS Feed Section -->
    <section class="container mt-5 card bell-card-back-main">
        <!-- RSS Feed Container with Data Attributes -->
        <div id="rss-feed-container" 
             data-company="bell_games" 
             data-sort="newest" 
             data-max="4" 
             data-news_type="all" 
             data-row="3" 
             data-light="dark" 
             data-bg-card="true" 
             data-bg-card-bg-color="dark" 
             data-bg-card-bg-row-color="black" 
             data-bg-card-bg-border="true" 
             data-bg-card-bg-border-color="danger">
            <!-- RSS Feed List will be injected here -->
            <ul id="rss-feed-list"></ul>
        </div>
        <!-- Load the RSS JavaScript file from the CDN -->
        <script async src="https://cdn.bellnetwork.eu/cdn/bell_network_front/get_rss.js"></script>
    </section>

**Description of Attributes:**

**data-company:**
  Specifies the company or source for the RSS feed.
  Example: 
    
    data-company="bell_games"
  
**data-sort:**
  Determines the sorting order of the news items.
  Options: newest, highup, highdown.
  Example: 
  
    data-sort="newest".

**data-max:**
  Limits the maximum number of news items displayed.
  Example: (shows up to 4 news items)

    data-max="4"

**data-news_type:**
  Filters the news based on type.
  Options: news, updates, gupdates, rss, all
  Example: (shows all news types)

    data-news_type="all"

**data-row:**
  Sets the number of news items per row.
  Example: (3 items per row).

    data-row="3"

**data-light:**
  Determines the color theme (light or dark mode).
  Options: light, dark.
  Example: (applies dark theme)

    data-light="dark"

**data-bg-card:**
  Enables or disables the background card for the feed container.
  Options: true, false.
  Example: (enables background card)

    data-bg-card="true"

**data-bg-card-bg-color:**
  Sets the background color of the main card.
  Options: light, dark, primary, etc.
  Example: (dark background)

    data-bg-card-bg-color="dark"

**data-bg-card-bg-row-color:**
  Sets the background color for each row of news items.
  Options: light, dark, primary, etc.
  Example:

    data-bg-card-bg-row-color="black"

**data-bg-card-bg-border:**
  Enables or disables a border around the feed container.
  Options: true, false.
  Example:

    data-bg-card-bg-border="true"

**data-bg-card-bg-border-color:**
  Sets the border color if data-bg-card-bg-border is true.
  Options: primary, danger, info, etc.
  Example: (red border)

    data-bg-card-bg-border-color="danger"

**Example Usage:**
  **In the provided example:**

  The RSS feed is configured for the bell group eu.
  It sorts the news by the newest first.
  A maximum of 4 news items will be displayed.
  The layout will use 3 items per row.
  The display uses a dark theme with a dark background for the main card and a black background for rows.
  This configuration ensures that the feed is customized according to the specified design and preferences.
  
  Background Card Enabled: The data-bg-card="true" attribute enables a styled background card around the RSS feed container.
  Background and Border Styling:
  To adjust the background card ensure data-bg-card-bg-border is set to true.
  Background Color: The card's background color is set to dark (data-bg-card-bg-color="dark").
  Row Background Color: Each row of news items has a black background (data-bg-card-bg-row-color="black").
  Border: A red border is applied around the card (data-bg-card-bg-border-color="danger").
  This setup ensures a customized appearance for the RSS feed with a clear and styled presentation based on the specified attributes.

**Direct RSS Feed URL**
 If you prefer a direct URL to fetch the RSS feed, you can use the following structure:

    https://rss.bellnetwork.eu/rss/<company>/feed

Replace <company> with a valid value. For example, to get the feed for bell_games:

     https://rss.bellnetwork.eu/rss/bell_games/feed

You can find a full list with all available projects for rss on https://rss.bellnetwork.eu

This README description provides a clear and comprehensive guide for integrating and customizing the Bell RSS feed section, making it easier for users to implement it on their websites.
