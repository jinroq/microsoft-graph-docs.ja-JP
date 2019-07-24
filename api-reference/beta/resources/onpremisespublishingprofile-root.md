---
title: オンプレミスの発行プロファイル
description: さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b0e975d932226adfa2c455baaa396c1d580f6ff
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841333"
---
# <a name="on-premises-publishing-profiles"></a>オンプレミスの発行プロファイル

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

さまざまな Azure サービス (たとえば、Azue Active Directory Connect パススルー認証、Workday to Azure AD ユーザープロビジョニング) は、企業ネットワークの外部からさまざまな社内リソースへの条件付きアクセスを許可します。 テナント管理者によってインストールされた[社内エージェント](onpremisesagent.md)は、発行された特定の[リソース](publishedresource.md)への要求にアクセスしたり、処理したりするように構成できます。
[エージェントグループ](onpremisesagentgroup.md)を使用すると、テナント管理者は特定のエージェントを割り当てて、発行された特定の社内リソースを提供できます。 テナント管理者は、複数のエージェントをまとめてグループ化し、発行された各リソースをグループに割り当てることができます。 同じオンプレミスの発行タイプのエンティティセット全体が[onPremisesPublishingProfile](onpremisespublishingprofile.md)によって表されます。

テナント管理者は、各**onPremisesPublishingProfile**に対して、エージェントが更新を受信したり、エージェントに対して更新プログラムを適用したりできる[時間枠](updatewindow.md)を構成できます。 **OnPremisesPublishingProfile**に指定された[updater 構成](hybridagentupdaterconfiguration.md)は、その**onPremisesPublishingProfile**内のすべてのエージェントに適用されます。

## <a name="see-also"></a>関連項目

- [オンプレミスのエージェント](onpremisesagent.md)
- [オンプレミスエージェントグループ](onpremisesagentgroup.md)
- [オンプレミスの発行プロファイル](onpremisespublishingprofile.md)
- [発行済みリソース](publishedresource.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
