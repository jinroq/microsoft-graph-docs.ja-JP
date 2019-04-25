---
title: teamsTemplate リソースの種類
description: teamsTemplate エンティティについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583173"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="b2eff-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2eff-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b2eff-104">チームテンプレートは、Microsoft Teams で[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="b2eff-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="b2eff-105">テンプレートでは、テンプレートを使用して作成された新しいチームでプロビジョニングする必要がある構造、設定、およびコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="b2eff-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="b2eff-106">Microsoft は基本テンプレートのセットを提供しており、お客様は独自のカスタムテンプレートを保存することができます。</span><span class="sxs-lookup"><span data-stu-id="b2eff-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="b2eff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2eff-107">Properties</span></span>

| <span data-ttu-id="b2eff-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2eff-108">Property</span></span>            | <span data-ttu-id="b2eff-109">型</span><span class="sxs-lookup"><span data-stu-id="b2eff-109">Type</span></span>     | <span data-ttu-id="b2eff-110">説明</span><span class="sxs-lookup"><span data-stu-id="b2eff-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="b2eff-111">id</span><span class="sxs-lookup"><span data-stu-id="b2eff-111">id</span></span>                  | <span data-ttu-id="b2eff-112">String</span><span class="sxs-lookup"><span data-stu-id="b2eff-112">String</span></span>   | <span data-ttu-id="b2eff-113">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b2eff-113">Unique identifier of the template.</span></span> <span data-ttu-id="b2eff-114">null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b2eff-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b2eff-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2eff-115">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsTemplate",
  "baseType": "microsoft.graph.entity"
}-->

```json
{
  "id": "string"
}
```

# <a name="see-also"></a><span data-ttu-id="b2eff-116">関連項目</span><span class="sxs-lookup"><span data-stu-id="b2eff-116">See also</span></span>

- [<span data-ttu-id="b2eff-117">team</span><span class="sxs-lookup"><span data-stu-id="b2eff-117">team</span></span>](team.md)

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
