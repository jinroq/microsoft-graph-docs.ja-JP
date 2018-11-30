---
title: licenseUnitsDetail リソースの種類
description: subscribedSku エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。
ms.openlocfilehash: 5f3d62c39248739746923195945efbc3322d5686
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066540"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="ca30d-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca30d-103">licenseUnitsDetail resource type</span></span>

> <span data-ttu-id="ca30d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca30d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca30d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca30d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca30d-106">[subscribedSku](subscribedsku.md) エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="ca30d-106">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="ca30d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca30d-107">Properties</span></span>
| <span data-ttu-id="ca30d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca30d-108">Property</span></span>     | <span data-ttu-id="ca30d-109">型</span><span class="sxs-lookup"><span data-stu-id="ca30d-109">Type</span></span>   |<span data-ttu-id="ca30d-110">説明</span><span class="sxs-lookup"><span data-stu-id="ca30d-110">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="ca30d-111">enabled</span><span class="sxs-lookup"><span data-stu-id="ca30d-111">enabled</span></span>|<span data-ttu-id="ca30d-112">Int32</span><span class="sxs-lookup"><span data-stu-id="ca30d-112">Int32</span></span>| <span data-ttu-id="ca30d-113">有効になっている単位の数です。</span><span class="sxs-lookup"><span data-stu-id="ca30d-113">The number of units that are enabled.</span></span> |
|<span data-ttu-id="ca30d-114">suspended</span><span class="sxs-lookup"><span data-stu-id="ca30d-114">suspended</span></span>|<span data-ttu-id="ca30d-115">Int32</span><span class="sxs-lookup"><span data-stu-id="ca30d-115">Int32</span></span>| <span data-ttu-id="ca30d-116">利用停止中の単位の数です。</span><span class="sxs-lookup"><span data-stu-id="ca30d-116">The number of units that are suspended.</span></span> |
|<span data-ttu-id="ca30d-117">warning</span><span class="sxs-lookup"><span data-stu-id="ca30d-117">warning</span></span>|<span data-ttu-id="ca30d-118">Int32</span><span class="sxs-lookup"><span data-stu-id="ca30d-118">Int32</span></span>| <span data-ttu-id="ca30d-119">警告ステータスのユニットの数です。</span><span class="sxs-lookup"><span data-stu-id="ca30d-119">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ca30d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca30d-120">JSON representation</span></span>

<span data-ttu-id="ca30d-121">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ca30d-121">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
