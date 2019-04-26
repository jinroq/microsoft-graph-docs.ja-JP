---
title: コネクタリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 5467d2a4625ad3813ff2777838db87be3ca5b713
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341220"
---
# <a name="connector-resource-type"></a><span data-ttu-id="6718d-103">コネクタリソースの種類</span><span class="sxs-lookup"><span data-stu-id="6718d-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="6718d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="6718d-104">Methods</span></span>

| <span data-ttu-id="6718d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6718d-105">Method</span></span>           | <span data-ttu-id="6718d-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6718d-106">Return Type</span></span>    |<span data-ttu-id="6718d-107">説明</span><span class="sxs-lookup"><span data-stu-id="6718d-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6718d-108">コネクタの取得</span><span class="sxs-lookup"><span data-stu-id="6718d-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="6718d-109">コネクター</span><span class="sxs-lookup"><span data-stu-id="6718d-109">connector</span></span>](connector.md) |<span data-ttu-id="6718d-110">コネクタオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6718d-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="6718d-111">List memberOf</span><span class="sxs-lookup"><span data-stu-id="6718d-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="6718d-112">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6718d-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="6718d-113">コネクタに関連付けられているコネクタグループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="6718d-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="6718d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6718d-114">Properties</span></span>
| <span data-ttu-id="6718d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6718d-115">Property</span></span>     | <span data-ttu-id="6718d-116">型</span><span class="sxs-lookup"><span data-stu-id="6718d-116">Type</span></span>   |<span data-ttu-id="6718d-117">説明</span><span class="sxs-lookup"><span data-stu-id="6718d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6718d-118">externalip</span><span class="sxs-lookup"><span data-stu-id="6718d-118">externalIp</span></span>|<span data-ttu-id="6718d-119">String</span><span class="sxs-lookup"><span data-stu-id="6718d-119">String</span></span>|<span data-ttu-id="6718d-120">コネクタコンピューターのサービスによって検出された外部 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="6718d-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="6718d-121">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="6718d-121">Read-only</span></span>|
|<span data-ttu-id="6718d-122">id</span><span class="sxs-lookup"><span data-stu-id="6718d-122">id</span></span>|<span data-ttu-id="6718d-123">String</span><span class="sxs-lookup"><span data-stu-id="6718d-123">String</span></span>| <span data-ttu-id="6718d-124">コネクタのオブジェクト id。</span><span class="sxs-lookup"><span data-stu-id="6718d-124">The object id of the connector.</span></span> <BR><span data-ttu-id="6718d-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6718d-125">Read-only.</span></span>|
|<span data-ttu-id="6718d-126">マシン</span><span class="sxs-lookup"><span data-stu-id="6718d-126">machineName</span></span>|<span data-ttu-id="6718d-127">String</span><span class="sxs-lookup"><span data-stu-id="6718d-127">String</span></span>| <span data-ttu-id="6718d-128">コネクタが実行されているコンピューターの名前。</span><span class="sxs-lookup"><span data-stu-id="6718d-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="6718d-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="6718d-129">Read-only</span></span>|
|<span data-ttu-id="6718d-130">status</span><span class="sxs-lookup"><span data-stu-id="6718d-130">status</span></span>|<span data-ttu-id="6718d-131">string</span><span class="sxs-lookup"><span data-stu-id="6718d-131">string</span></span>| <span data-ttu-id="6718d-132">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6718d-132">Indicates the status of the connector.</span></span> <span data-ttu-id="6718d-133">可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="6718d-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="6718d-134">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="6718d-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="6718d-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6718d-135">Relationships</span></span>
| <span data-ttu-id="6718d-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6718d-136">Relationship</span></span> | <span data-ttu-id="6718d-137">型</span><span class="sxs-lookup"><span data-stu-id="6718d-137">Type</span></span>   |<span data-ttu-id="6718d-138">説明</span><span class="sxs-lookup"><span data-stu-id="6718d-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6718d-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="6718d-139">memberOf</span></span>|<span data-ttu-id="6718d-140">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6718d-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="6718d-141">接続がメンバーであるコネクタグループ。</span><span class="sxs-lookup"><span data-stu-id="6718d-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="6718d-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6718d-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6718d-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6718d-143">JSON representation</span></span>

<span data-ttu-id="6718d-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6718d-144">Here is a JSON representation of the resource.</span></span>

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
