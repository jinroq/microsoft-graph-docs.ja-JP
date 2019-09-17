---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8e0f3abab7eac1507dd60a20657d3c1a66fefc5
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36846134"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    ReceivedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    HasAttachments = true,
    From = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    Sender = new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    },
    ConversationThreadId = "conversationThreadId-value",
    NewParticipants = new List<Recipient>()
    {
        new Recipient
        {
            EmailAddress = new EmailAddress
            {
                Name = "name-value",
                Address = "address-value"
            }
        }
    },
    ConversationId = "conversationId-value",
    CreatedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    ChangeKey = "changeKey-value",
    Categories = new List<String>()
    {
        "categories-value"
    },
    Id = "id-value",
    InReplyTo = new Post
    {
    },
    Attachments = new List<Attachment>()
    {
        new Attachment
        {
            LastModifiedDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
            Name = "name-value",
            ContentType = "contentType-value",
            Size = 99,
            IsInline = true,
            Id = "id-value"
        }
    }
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```