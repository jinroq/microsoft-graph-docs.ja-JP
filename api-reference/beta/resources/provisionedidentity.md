---
title: provisionedIdentity リソースの種類
description: プロビジョニングオブジェクトの概要イベントに関連付けられている id を記述します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fb535bbba827f93b597c5e41efb128f2ad610ef2
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349411"
---
# <a name="provisionedidentity-resource-type"></a><span data-ttu-id="92117-103">provisionedIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92117-103">provisionedIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92117-104">プロビジョニングオブジェクトの概要イベントに関連付けられている id を記述します。</span><span class="sxs-lookup"><span data-stu-id="92117-104">Describes the identity associated with the provisioning object summary event.</span></span> 

## <a name="properties"></a><span data-ttu-id="92117-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92117-105">Properties</span></span>

| <span data-ttu-id="92117-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92117-106">Property</span></span>     | <span data-ttu-id="92117-107">型</span><span class="sxs-lookup"><span data-stu-id="92117-107">Type</span></span>        | <span data-ttu-id="92117-108">説明</span><span class="sxs-lookup"><span data-stu-id="92117-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="92117-109">詳細</span><span class="sxs-lookup"><span data-stu-id="92117-109">details</span></span>|[<span data-ttu-id="92117-110">詳細情報</span><span class="sxs-lookup"><span data-stu-id="92117-110">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="92117-111">Id の詳細。</span><span class="sxs-lookup"><span data-stu-id="92117-111">Details of the identity.</span></span>|
|<span data-ttu-id="92117-112">displayName</span><span class="sxs-lookup"><span data-stu-id="92117-112">displayName</span></span>|<span data-ttu-id="92117-113">String</span><span class="sxs-lookup"><span data-stu-id="92117-113">String</span></span>|<span data-ttu-id="92117-114">Id の表示名。</span><span class="sxs-lookup"><span data-stu-id="92117-114">Display name of the identity.</span></span> |
|<span data-ttu-id="92117-115">id</span><span class="sxs-lookup"><span data-stu-id="92117-115">id</span></span>|<span data-ttu-id="92117-116">文字列</span><span class="sxs-lookup"><span data-stu-id="92117-116">String</span></span>|<span data-ttu-id="92117-117">Id を一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="92117-117">Uniquely identifies the identity.</span></span>|
|<span data-ttu-id="92117-118">identityType</span><span class="sxs-lookup"><span data-stu-id="92117-118">identityType</span></span>|<span data-ttu-id="92117-119">String</span><span class="sxs-lookup"><span data-stu-id="92117-119">String</span></span>|<span data-ttu-id="92117-120">プロビジョニングされた id の種類 (' user '、' group ' など)。</span><span class="sxs-lookup"><span data-stu-id="92117-120">Type of identity that has been provisioned, such as 'user' or 'group'.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="92117-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92117-121">JSON representation</span></span>

<span data-ttu-id="92117-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92117-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedIdentity",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String",
  "identityType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
