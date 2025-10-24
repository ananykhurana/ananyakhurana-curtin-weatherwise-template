# ✍️ Project Reflection

## AI Tools Used

For this project, I primarily used Claude AI (via Cursor IDE) as my development assistant. The AI helped me in multiple ways: brainstorming implementation approaches, generating initial code structures, explaining complex concepts, and refining solutions through iterative prompting. Rather than simply accepting AI-generated code, I used it as a collaborative tool - asking questions, challenging suggestions, and requesting improvements until the code met professional standards.

## Prompting Techniques

Throughout this project, I applied several intentional prompting strategies:

1. **Pseudocode First**: Before requesting any implementation, I asked for pseudocode to understand the logic flow, ensuring I comprehended the approach before diving into syntax.

2. **Restating Problems**: I began conversations by restating requirements in my own words, which helped clarify my understanding and led to more targeted AI responses.

3. **Challenging Edge Cases**: Rather than accepting initial implementations, I actively questioned "What if?" scenarios - invalid locations, missing data, API failures - which led to much more robust error handling.

4. **Iterative Refinement**: I made multiple passes on each component, first getting basic functionality, then requesting specific improvements (better colors, error messages, additional features).

5. **Requesting Explanations**: I consistently asked the AI to explain *why* certain approaches were chosen, which deepened my understanding and helped me make informed decisions about trade-offs.

These techniques transformed AI from a code generator into a teaching tool that enhanced my learning.

## What Worked Well

I'm particularly proud of the natural language processing component. Initially, parsing user questions seemed daunting - how do you extract meaning from unstructured text? By breaking the problem into manageable pieces (extracting location, time, attribute) and using keyword matching with regex patterns, I created a system that handles many question variations naturally. The function successfully parses questions like "Will it rain in Sydney tomorrow?" or "What's the temperature in Perth this week?" and generates appropriate natural language responses. This demonstrates that complex-seeming problems can be solved with thoughtful design and systematic implementation.

The visualization component also exceeded my expectations. The temperature chart with filled areas between max and min temps, combined with the two-subplot precipitation display, creates professional-looking outputs that genuinely help users understand weather trends. The iterative prompting process - starting with basic charts and progressively adding features like annotations, better colors, and value labels - resulted in visualizations I'm genuinely proud to show.

## What Would You Do Differently

If I had more time, I would implement caching for API calls to improve performance during testing and reduce load on the weather service. Currently, each request hits the API, which works fine but isn't optimal. A simple time-based cache (storing results for 5-10 minutes) would make the application more responsive when users query the same location multiple times.

I would also enhance the location parsing to handle a wider variety of input formats. Currently, locations need to be capitalized for the regex pattern to match. Adding a database of known cities or fuzzy matching would make the system more forgiving of user input variations. However, I made a conscious decision to focus on core requirements rather than these optimizations, which reflects good project prioritization.

Additionally, I could add more visualization types - perhaps a combined view showing temperature and precipitation together, or a weekly summary dashboard. The modular structure I created would make adding these features straightforward.

## Final Thoughts

This project transformed my understanding of both software development and AI-assisted programming. I learned that AI tools are most valuable not as code generators, but as collaborative partners in problem-solving. The key is asking the right questions, challenging initial responses, and iteratively refining solutions.

The process of documenting AI conversations revealed how much my prompting improved throughout the project. Early conversations were vaguer, while later ones were more precise and strategic. This metacognitive awareness - understanding how I think and learn - is perhaps the most valuable outcome of this assignment.

I also gained confidence in tackling complex projects. By breaking the weather advisor into modular components (data retrieval, visualization, NLP, UI), what initially seemed overwhelming became manageable. This systematic approach to complexity is a skill I'll carry into future projects.

Finally, I appreciate how the assignment balanced technical requirements with process documentation. Showing my work through AI conversations felt more authentic than traditional assignments where only the final product matters. In the real world, the thinking process and problem-solving approach are just as important as the code itself, and this assignment reflected that reality.
