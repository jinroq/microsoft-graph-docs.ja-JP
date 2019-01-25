---
title: コネクタ リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525732"
---
# <a name="connector-resource-type"></a><span data-ttu-id="b3dcf-103">コネクタ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3dcf-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="b3dcf-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3dcf-104">Methods</span></span>

| <span data-ttu-id="b3dcf-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3dcf-105">Method</span></span>           | <span data-ttu-id="b3dcf-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b3dcf-106">Return Type</span></span>    |<span data-ttu-id="b3dcf-107">説明</span><span class="sxs-lookup"><span data-stu-id="b3dcf-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3dcf-108">コネクタを取得します。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="b3dcf-109">Connector</span><span class="sxs-lookup"><span data-stu-id="b3dcf-109">connector</span></span>](connector.md) |<span data-ttu-id="b3dcf-110">コネクタ オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="b3dcf-111">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b3dcf-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="b3dcf-112">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dcf-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="b3dcf-113">コネクタに関連付けられている connectorGroup オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3dcf-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dcf-114">Properties</span></span>
| <span data-ttu-id="b3dcf-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dcf-115">Property</span></span>     | <span data-ttu-id="b3dcf-116">型</span><span class="sxs-lookup"><span data-stu-id="b3dcf-116">Type</span></span>   |<span data-ttu-id="b3dcf-117">説明</span><span class="sxs-lookup"><span data-stu-id="b3dcf-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3dcf-118">externalIp</span><span class="sxs-lookup"><span data-stu-id="b3dcf-118">externalIp</span></span>|<span data-ttu-id="b3dcf-119">String</span><span class="sxs-lookup"><span data-stu-id="b3dcf-119">String</span></span>|<span data-ttu-id="b3dcf-120">コネクタ コンピューターのサービスによって検出されたと外部の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="b3dcf-121">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="b3dcf-121">Read-only</span></span>|
|<span data-ttu-id="b3dcf-122">id</span><span class="sxs-lookup"><span data-stu-id="b3dcf-122">id</span></span>|<span data-ttu-id="b3dcf-123">String</span><span class="sxs-lookup"><span data-stu-id="b3dcf-123">String</span></span>| <span data-ttu-id="b3dcf-124">コネクタのオブジェクト id です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-124">The object id of the connector.</span></span> <BR><span data-ttu-id="b3dcf-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-125">Read-only.</span></span>|
|<span data-ttu-id="b3dcf-126">マシン名</span><span class="sxs-lookup"><span data-stu-id="b3dcf-126">machineName</span></span>|<span data-ttu-id="b3dcf-127">String</span><span class="sxs-lookup"><span data-stu-id="b3dcf-127">String</span></span>| <span data-ttu-id="b3dcf-128">コネクタが実行されているマシンの名前です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="b3dcf-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="b3dcf-129">Read-only</span></span>|
|<span data-ttu-id="b3dcf-130">status</span><span class="sxs-lookup"><span data-stu-id="b3dcf-130">status</span></span>|<span data-ttu-id="b3dcf-131">string</span><span class="sxs-lookup"><span data-stu-id="b3dcf-131">string</span></span>| <span data-ttu-id="b3dcf-132">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-132">Indicates the status of the connector.</span></span> <span data-ttu-id="b3dcf-133">使用可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="b3dcf-134">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="b3dcf-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="b3dcf-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3dcf-135">Relationships</span></span>
| <span data-ttu-id="b3dcf-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3dcf-136">Relationship</span></span> | <span data-ttu-id="b3dcf-137">型</span><span class="sxs-lookup"><span data-stu-id="b3dcf-137">Type</span></span>   |<span data-ttu-id="b3dcf-138">説明</span><span class="sxs-lookup"><span data-stu-id="b3dcf-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3dcf-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="b3dcf-139">memberOf</span></span>|<span data-ttu-id="b3dcf-140">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b3dcf-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="b3dcf-141">接続がのメンバーである connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="b3dcf-142">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3dcf-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3dcf-143">JSON representation</span></span>

<span data-ttu-id="b3dcf-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3dcf-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/connector.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
