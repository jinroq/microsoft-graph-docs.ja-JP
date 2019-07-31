---
title: 同期エラーリソースの種類
description: 同期処理中に発生したエラーを表します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2be415a127f7bcef030407be737bb9b48c8a116f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964670"
---
# <a name="synchronizationerror-resource-type"></a><span data-ttu-id="f1c5a-103">同期エラーリソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1c5a-103">synchronizationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1c5a-104">同期処理中に発生したエラーを表します。</span><span class="sxs-lookup"><span data-stu-id="f1c5a-104">Represents an error that occurred during the synchronization process.</span></span>

## <a name="properties"></a><span data-ttu-id="f1c5a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c5a-105">Properties</span></span>

<!-- Add descriptions for the properties. -->
| <span data-ttu-id="f1c5a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1c5a-106">Property</span></span>     | <span data-ttu-id="f1c5a-107">型</span><span class="sxs-lookup"><span data-stu-id="f1c5a-107">Type</span></span>   |<span data-ttu-id="f1c5a-108">説明</span><span class="sxs-lookup"><span data-stu-id="f1c5a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1c5a-109">code</span><span class="sxs-lookup"><span data-stu-id="f1c5a-109">code</span></span>|<span data-ttu-id="f1c5a-110">String</span><span class="sxs-lookup"><span data-stu-id="f1c5a-110">String</span></span>||
|<span data-ttu-id="f1c5a-111">message</span><span class="sxs-lookup"><span data-stu-id="f1c5a-111">message</span></span>|<span data-ttu-id="f1c5a-112">String</span><span class="sxs-lookup"><span data-stu-id="f1c5a-112">String</span></span>||
|<span data-ttu-id="f1c5a-113">tenantActionable 可能</span><span class="sxs-lookup"><span data-stu-id="f1c5a-113">tenantActionable</span></span>|<span data-ttu-id="f1c5a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="f1c5a-114">Boolean</span></span>||

## <a name="json-representation"></a><span data-ttu-id="f1c5a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1c5a-115">JSON representation</span></span>

<span data-ttu-id="f1c5a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f1c5a-116">The following is a JSON representation of the resource.</span></span>

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
