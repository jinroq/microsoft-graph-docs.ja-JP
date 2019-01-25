---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティをについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e75b3d8df318b116d5d908a40d4f756d9ee70864
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513047"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="27308-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27308-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27308-104">チーム テンプレートは、マイクロソフトのチームで[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="27308-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="27308-105">テンプレートは、テンプレートを使用して作成された新しいチームの構造、設定、および準備する必要があるものコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="27308-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="27308-106">マイクロソフトは、基本テンプレートのスイートを提供していて、お客様が独自のカスタム テンプレートを保存できます。</span><span class="sxs-lookup"><span data-stu-id="27308-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="27308-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27308-107">Properties</span></span>

| <span data-ttu-id="27308-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27308-108">Property</span></span>            | <span data-ttu-id="27308-109">型</span><span class="sxs-lookup"><span data-stu-id="27308-109">Type</span></span>     | <span data-ttu-id="27308-110">説明</span><span class="sxs-lookup"><span data-stu-id="27308-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="27308-111">id</span><span class="sxs-lookup"><span data-stu-id="27308-111">id</span></span>                  | <span data-ttu-id="27308-112">String</span><span class="sxs-lookup"><span data-stu-id="27308-112">String</span></span>   | <span data-ttu-id="27308-113">テンプレートの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="27308-113">Unique identifier of the template.</span></span> <span data-ttu-id="27308-114">Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="27308-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="27308-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27308-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="27308-116">関連項目</span><span class="sxs-lookup"><span data-stu-id="27308-116">See also</span></span>

- <span data-ttu-id="27308-117">Team</span><span class="sxs-lookup"><span data-stu-id="27308-117">[team](team.md)</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamstemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
