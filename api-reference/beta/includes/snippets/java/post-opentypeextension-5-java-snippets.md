---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bf7762aad6ba53d1571b6e4fd28420c38cc46866
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878430"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = new Conversation();
conversation.Topic = "Does anyone have a second?";
LinkedList<ConversationThread> ThreadsList = new LinkedList<ConversationThread>();
ConversationThread Threads = new ConversationThread();
LinkedList<Post> PostsList = new LinkedList<Post>();
Post Posts = new Post();
ItemBody Body = new ItemBody();
Body.ContentType = BodyType.HTML;
Body.Content = "This is urgent!";
Posts.Body = Body;
LinkedList<Extension> ExtensionsList = new LinkedList<Extension>();
Extension Extensions = new Extension();
Extensions.additionalDataManager().put("@odata.type", new JsonPrimitive("microsoft.graph.openTypeExtension"));
Extensions.extensionName = "Com.Contoso.Benefits";
Extensions.companyName = "Contoso";
Extensions.expirationDate = "2016-08-03T11:00:00Z";
LinkedList<String> topPicksList = new LinkedList<String>();
topPicksList.add("Employees only");
topPicksList.add("Add spouse or guest");
topPicksList.add("Add family");
Extensions.topPicks = topPicksList;
ExtensionsList.add(Extensions);
Posts.Extensions = ExtensionsList;
PostsList.add(Posts);
Threads.Posts = PostsList;
ThreadsList.add(Threads);
conversation.Threads = ThreadsList;

graphClient.groups("37df2ff0-0de0-4c33-8aee-75289364aef6").conversations()
    .buildRequest()
    .post(conversation);

```