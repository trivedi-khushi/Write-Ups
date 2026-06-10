---
title: "Three Key Engineering Lessons with Agents "

---

Three Key Engineering Lessons with Agents Kesh closes with three critical lessons learned:

1.  Don't just throw the problem at the LLM You can't just prompt "migrate this codebase" and expect consistent output. The output will differ every time — and that's dangerous. Solution: use a parser first to create a structured view of the codebase, then hand that to the LLM.
    
2.  Context window compression kills accuracy Throwing 700 functions into one prompt causes the LLM to summarize/compress the input to save context space — and then it makes decisions based on the summarized (incomplete) version, not the real code. Solution: partition work into multiple sub-agents, each getting its own full, uncompressed context window for higher accuracy.
    
3.  Architecture thinking has changed LLMs can write code extremely well. So the problems engineers now need to think about are different:
    

How do you compose agents? How do you handle conflict resolution between agents? How do you verify accuracy? Where in the software cycle should humans spend their time — designing code or designing architecture?