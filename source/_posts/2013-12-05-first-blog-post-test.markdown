---
layout: post
title: "First Blog Post Test"
date: 2013-12-05 21:07:19 -0500
comments: true
categories: Sitecore
---

hello? is this thing on?

```csharp
public string CalculateMD5Hash(string input)
{
  // step 1, calculate MD5 hash from input
  MD5 md5 = System.Security.Cryptography.MD5.Create();
  byte[] inputBytes = System.Text.Encoding.ASCII.GetBytes(input);
  byte[] hash = md5.ComputeHash(inputBytes);

  // step 2, convert byte array to hex string
  StringBuilder sb = new StringBuilder();
  for (int i = 0; i < hash.Length; i++)
  {
    sb.Append(hash[i].ToString("X2"));
  }
  return sb.ToString();
}
```

more text is here and doing stuff that is cool la la la


{% gist 7817481 %}