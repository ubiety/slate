---
title: Ubiety XMPP Documentation

language_tabs:
  - csharp: C#
  - vb: VB.NET

toc_footers:
  - <a href='http://github.com/tripit/slate'>Documentation Powered by Slate</a>

search: true
---

# Introduction

Welcome to the Ubiety XMPP Documentation. This is a .NET implementation of the XMPP protocol used for chat applications.

# Connecting

```csharp
using Ubiety;

class Main {
  public void Main(string[] args) {
    Xmpp xmpp = new Xmpp();
    xmpp.Settings.Username = "test@testing.com";
    xmpp.Settings.Password = "testpass";

    xmpp.Connect();
  }
}
```

```vb
Imports Ubiety

Class Main
    Public Sub Main(ByVal args() As String)
        Dim xmpp As Xmpp = New Xmpp
        xmpp.Settings.Username = "test@testing.com"
        xmpp.Settings.Password = "testpass"
        xmpp.Connect
    End Sub
End Class
```

To connect to a server you must set the username and password. The username must be a valid JID as we will determine which server to connect to from it.
