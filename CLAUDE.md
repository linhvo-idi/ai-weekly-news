This folder is a GitHub repository for the AI for Development newsletter.

When I give you a zip file containing newsletter HTML files to publish:

1. Extract and save the index.html newsletter content as `index.html` in the root (overwrite existing)

2. Save the dated copy to `archive'

3. Edit `archive.html` to add a new entry at the TOP of the <ul class="archive-list">, directly after the <!-- ADD NEW ISSUES HERE --> comment. Use this format:
   <li class="archive-item">
       <a href="archive/ai-newsletter-[START]-to-[END].html" class="archive-link">
           <span class="archive-date">[Human-readable date range, e.g., "Jan 27 – Feb 10, 2026"]</span>
           <span class="archive-meta"><span class="archive-count">[X] updates</span></span>
       </a>
   </li>

4. Remove the "empty state" <li> if it still exists (the one with 📭 emoji)

5. Run these commands in sequence:
   git add .
   git commit -m "Add newsletter: [date range]"
   git push

6. Confirm when done and provide the live URL