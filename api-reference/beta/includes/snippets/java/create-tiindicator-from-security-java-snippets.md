---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12e5cbf9cd9db67be02712dd673ccb0435126d4a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868109"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.action = TiAction.ALERT;
LinkedList<String> activityGroupNamesList = new LinkedList<String>();
tiIndicator.activityGroupNames = activityGroupNamesList;
tiIndicator.confidence = 0;
tiIndicator.description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.";
tiIndicator.expirationDateTime = "2019-03-02T00:43:37.5031462+03:00";
tiIndicator.externalId = "Test--8586509942679764298MS501";
tiIndicator.fileHashType = FileHashType.SHA256;
tiIndicator.fileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313";
LinkedList<String> killChainList = new LinkedList<String>();
tiIndicator.killChain = killChainList;
LinkedList<String> malwareFamilyNamesList = new LinkedList<String>();
tiIndicator.malwareFamilyNames = malwareFamilyNamesList;
tiIndicator.severity = 0;
LinkedList<String> tagsList = new LinkedList<String>();
tiIndicator.tags = tagsList;
tiIndicator.targetProduct = "Azure Sentinel";
tiIndicator.threatType = "WatchList";
tiIndicator.tlpLevel = TlpLevel.GREEN;

graphClient.security().tiIndicators()
    .buildRequest()
    .post(tiIndicator);

```