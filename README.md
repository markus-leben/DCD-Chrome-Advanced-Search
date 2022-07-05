# DCD-Chrome-Advanced-Search
A tool for extending Google Chrome's address bar search to work on Diamond Comics Distributions internal search, including advanced search terms.

# HowTo:
1. In google chrome settings under site search, add a new search with the url https://retailerservices.diamondcomics.com/Reorder/Reorder?&start=tabContentItemSearch?tmpayload=%s
2. Install Tampermonkey
3. Create a new script and copy the paste of DCDSearch.js or import it from greasyfork.

# Search Syntax
Searches are formatted like "dcd category:payload", with spaces separating each. So, for example, you might type "dcd artist:staples batch:feb22". 

The default category is title, so if you type "dcd saga" it will search for every book with 'saga' in its title. You might have to narrow that search down a fair bit.

Artists, writers, and cover artists are entered into the 'creator name 1', 'creator name 2', and 'creator name 3' fields respectively. Be aware that this leads to some weird edge cases on books that have one creator in multiple roles or multiple creators in the same role. If you're trying to search for a book that has two writers, you should probably input "dcd writer:[writer 1 here] artist:[writer 2 here]" for best results. This is a weird workaround, but the best I have so far.

Currently, you are allowed to type multiple of the same category in. So "dcd saga category:comics category:tps" would give you all Saga trades and single issues. 

Quote support is currently on my todo.
