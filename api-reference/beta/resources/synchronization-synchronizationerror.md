---
title: 同期エラーリソースの種類
description: 同期処理中に発生したエラーを表します。
localization_priority: Normal
ms.openlocfilehash: 7f678cdbd48a3d5f013c22120d01c28bb61738e6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324747"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="67d6e-103">同期エラーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="67d6e-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67d6e-104">同期処理中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="67d6e-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="67d6e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67d6e-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="67d6e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67d6e-106">Property</span></span>     | <span data-ttu-id="67d6e-107">型</span><span class="sxs-lookup"><span data-stu-id="67d6e-107">Type</span></span>   |<span data-ttu-id="67d6e-108">説明</span><span class="sxs-lookup"><span data-stu-id="67d6e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="67d6e-109">code</span><span class="sxs-lookup"><span data-stu-id="67d6e-109">code</span></span>|<span data-ttu-id="67d6e-110">String</span><span class="sxs-lookup"><span data-stu-id="67d6e-110">String</span></span>||
|<span data-ttu-id="67d6e-111">message</span><span class="sxs-lookup"><span data-stu-id="67d6e-111">message</span></span>|<span data-ttu-id="67d6e-112">String</span><span class="sxs-lookup"><span data-stu-id="67d6e-112">String</span></span>||
|<span data-ttu-id="67d6e-113">tenantactionable 可能</span><span class="sxs-lookup"><span data-stu-id="67d6e-113">tenantActionable</span></span>|<span data-ttu-id="67d6e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="67d6e-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="67d6e-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="67d6e-115">JSON representation</span></span>

<span data-ttu-id="67d6e-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="67d6e-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationError"
}-->

```json
{
  "code": "String",
  "message": "String",
  "tenantActionable": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
