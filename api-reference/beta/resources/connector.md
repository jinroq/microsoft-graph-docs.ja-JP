---
title: コネクタリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ec4d3fdb415533d5b3f2effc72688fe912551bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012878"
---
# <a name="connector-resource-type"></a><span data-ttu-id="19111-103">コネクタリソースの種類</span><span class="sxs-lookup"><span data-stu-id="19111-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="19111-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="19111-104">Methods</span></span>

| <span data-ttu-id="19111-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="19111-105">Method</span></span>           | <span data-ttu-id="19111-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="19111-106">Return Type</span></span>    |<span data-ttu-id="19111-107">説明</span><span class="sxs-lookup"><span data-stu-id="19111-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="19111-108">コネクタの取得</span><span class="sxs-lookup"><span data-stu-id="19111-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="19111-109">コネクター</span><span class="sxs-lookup"><span data-stu-id="19111-109">connector</span></span>](connector.md) |<span data-ttu-id="19111-110">コネクタオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="19111-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="19111-111">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="19111-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="19111-112">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="19111-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="19111-113">コネクタに関連付けられているコネクタグループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="19111-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="19111-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19111-114">Properties</span></span>
| <span data-ttu-id="19111-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19111-115">Property</span></span>     | <span data-ttu-id="19111-116">型</span><span class="sxs-lookup"><span data-stu-id="19111-116">Type</span></span>   |<span data-ttu-id="19111-117">説明</span><span class="sxs-lookup"><span data-stu-id="19111-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19111-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="19111-118">externalIp</span></span>|<span data-ttu-id="19111-119">String</span><span class="sxs-lookup"><span data-stu-id="19111-119">String</span></span>|<span data-ttu-id="19111-120">コネクタコンピューターのサービスによって検出された外部 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="19111-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="19111-121">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="19111-121">Read-only</span></span>|
|<span data-ttu-id="19111-122">id</span><span class="sxs-lookup"><span data-stu-id="19111-122">id</span></span>|<span data-ttu-id="19111-123">文字列</span><span class="sxs-lookup"><span data-stu-id="19111-123">String</span></span>| <span data-ttu-id="19111-124">コネクタのオブジェクト id。</span><span class="sxs-lookup"><span data-stu-id="19111-124">The object id of the connector.</span></span> <BR><span data-ttu-id="19111-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19111-125">Read-only.</span></span>|
|<span data-ttu-id="19111-126">マシン</span><span class="sxs-lookup"><span data-stu-id="19111-126">machineName</span></span>|<span data-ttu-id="19111-127">String</span><span class="sxs-lookup"><span data-stu-id="19111-127">String</span></span>| <span data-ttu-id="19111-128">コネクタが実行されているコンピューターの名前。</span><span class="sxs-lookup"><span data-stu-id="19111-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="19111-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="19111-129">Read-only</span></span>|
|<span data-ttu-id="19111-130">status</span><span class="sxs-lookup"><span data-stu-id="19111-130">status</span></span>|<span data-ttu-id="19111-131">string</span><span class="sxs-lookup"><span data-stu-id="19111-131">string</span></span>| <span data-ttu-id="19111-132">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="19111-132">Indicates the status of the connector.</span></span> <span data-ttu-id="19111-133">可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="19111-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="19111-134">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="19111-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="19111-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19111-135">Relationships</span></span>
| <span data-ttu-id="19111-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19111-136">Relationship</span></span> | <span data-ttu-id="19111-137">型</span><span class="sxs-lookup"><span data-stu-id="19111-137">Type</span></span>   |<span data-ttu-id="19111-138">説明</span><span class="sxs-lookup"><span data-stu-id="19111-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19111-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="19111-139">memberOf</span></span>|<span data-ttu-id="19111-140">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="19111-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="19111-141">接続がメンバーであるコネクタグループ。</span><span class="sxs-lookup"><span data-stu-id="19111-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="19111-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="19111-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="19111-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19111-143">JSON representation</span></span>

<span data-ttu-id="19111-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="19111-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connector"
}-->

```json
{
  "externalIp": "String",
  "id": "String (identifier)",
  "machineName": "String",
  "status": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
