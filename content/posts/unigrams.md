---
title: "Text file dissection"
date: 2021-09-02
draft: true
---

This is one of the first C++ projects I have done that actually felt useful. The program takes a .txt file input, cleans it up, and counts unigrams and bigrams.

Throughout this post, I am going to break down some of the more interesting bits of code, or things I find interesting. If you want to skip that and just look at the code yourself, you can here[LINK TO GITHUB].

To start if you've never heard of unigrams or bigrams (like I hadn't). The concept comes from n-grams, basically just continuous "phrases" from some larger section of text. So unigram just being words in this case, and bigrams being strings of 2 words that appear next to each other.

If we were to have a string "that dog runs fast".

the unigrams would be:
  that
  dog
  runs
  fast

and the bigrams:
  that dog
  dog runs
  runs fast

Now into the fun parts of code!

TODO: readData
``` c++
int readData(string fileName, string  (&wordArray)[ARRAYSIZE], int &wordCount)
{
  ifstream textFile(fileName);
  if(textFile.is_open())
  {
    int i=0;
    while(textFile >> wordArray[i])
    {
      i++;
    }
    textFile.close();
    wordCount = i;
    cout << "Finished Reading " << wordCount << " words. Closing file" << endl;
  } else
  {
    cout << "File could not be opened" << endl;
    return 0;
  }
  return 1;
}
```

TODO: cleanUp
``` c++
  // your code here
```

TODO: generate Unigram/bigrams
``` c++
  // your code here
```

TODO: Other cool uses once its setup: getLongestWord, Search. Logging. In theory shortestWord, things that repeat x times
