---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1aa3b528ec966c88859dfa8244a245c72047449f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889435"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Conversation conversation = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").conversations("AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=")
    .buildRequest()
    .get();

```