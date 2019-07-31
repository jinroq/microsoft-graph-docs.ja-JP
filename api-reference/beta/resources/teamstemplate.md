---
title: teamsTemplate リソースの種類
description: TeamsTemplate エンティティについて説明します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dde08e6c4ecde3b3a600958a5af5cd93b5fc600f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964390"
---
# <a name="teamstemplate-resource-type"></a><span data-ttu-id="e5f58-103">teamsTemplate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5f58-103">teamsTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5f58-104">チームテンプレートは、Microsoft Teams で[チーム](../resources/team.md)を作成するための青写真です。</span><span class="sxs-lookup"><span data-stu-id="e5f58-104">A team template is a blueprint for creating a [team](../resources/team.md) in Microsoft Teams.</span></span> <span data-ttu-id="e5f58-105">テンプレートでは、テンプレートを使用して作成された新しいチームでプロビジョニングする必要がある構造、設定、およびコンテンツを指定します。</span><span class="sxs-lookup"><span data-stu-id="e5f58-105">A template specifies the structure, settings, and even content that should be provisioned in a new team created using the template.</span></span> <span data-ttu-id="e5f58-106">Microsoft は基本テンプレートのセットを提供しており、お客様は独自のカスタムテンプレートを保存することができます。</span><span class="sxs-lookup"><span data-stu-id="e5f58-106">Microsoft provides a suite of base templates and customers can save their own custom templates.</span></span>

## <a name="properties"></a><span data-ttu-id="e5f58-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5f58-107">Properties</span></span>

| <span data-ttu-id="e5f58-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5f58-108">Property</span></span>            | <span data-ttu-id="e5f58-109">型</span><span class="sxs-lookup"><span data-stu-id="e5f58-109">Type</span></span>     | <span data-ttu-id="e5f58-110">説明</span><span class="sxs-lookup"><span data-stu-id="e5f58-110">Description</span></span> |
|:------------------- |:-------- |:----------- |
| <span data-ttu-id="e5f58-111">id</span><span class="sxs-lookup"><span data-stu-id="e5f58-111">id</span></span>                  | <span data-ttu-id="e5f58-112">String</span><span class="sxs-lookup"><span data-stu-id="e5f58-112">String</span></span>   | <span data-ttu-id="e5f58-113">テンプレートの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e5f58-113">Unique identifier of the template.</span></span> <span data-ttu-id="e5f58-114">Null にすることはできません。</span><span class="sxs-lookup"><span data-stu-id="e5f58-114">Cannot be null.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5f58-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5f58-115">JSON representation</span></span>

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

# <a name="see-also"></a><span data-ttu-id="e5f58-116">関連項目</span><span class="sxs-lookup"><span data-stu-id="e5f58-116">See also</span></span>

- [<span data-ttu-id="e5f58-117">team</span><span class="sxs-lookup"><span data-stu-id="e5f58-117">team</span></span>](team.md)

