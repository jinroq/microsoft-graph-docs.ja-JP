---
title: コネクタリソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: eed936c808e920f35a741a836a1fab64b2754bf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535537"
---
# <a name="connector-resource-type"></a><span data-ttu-id="0fcd8-103">コネクタリソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fcd8-103">connector resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="0fcd8-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fcd8-104">Methods</span></span>

| <span data-ttu-id="0fcd8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0fcd8-105">Method</span></span>           | <span data-ttu-id="0fcd8-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0fcd8-106">Return Type</span></span>    |<span data-ttu-id="0fcd8-107">説明</span><span class="sxs-lookup"><span data-stu-id="0fcd8-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0fcd8-108">コネクタの取得</span><span class="sxs-lookup"><span data-stu-id="0fcd8-108">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="0fcd8-109">コネクター</span><span class="sxs-lookup"><span data-stu-id="0fcd8-109">connector</span></span>](connector.md) |<span data-ttu-id="0fcd8-110">コネクタオブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-110">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="0fcd8-111">List memberOf</span><span class="sxs-lookup"><span data-stu-id="0fcd8-111">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="0fcd8-112">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fcd8-112">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="0fcd8-113">コネクタに関連付けられているコネクタグループオブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-113">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="0fcd8-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fcd8-114">Properties</span></span>
| <span data-ttu-id="0fcd8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fcd8-115">Property</span></span>     | <span data-ttu-id="0fcd8-116">型</span><span class="sxs-lookup"><span data-stu-id="0fcd8-116">Type</span></span>   |<span data-ttu-id="0fcd8-117">説明</span><span class="sxs-lookup"><span data-stu-id="0fcd8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fcd8-118">externalip</span><span class="sxs-lookup"><span data-stu-id="0fcd8-118">externalIp</span></span>|<span data-ttu-id="0fcd8-119">String</span><span class="sxs-lookup"><span data-stu-id="0fcd8-119">String</span></span>|<span data-ttu-id="0fcd8-120">コネクタコンピューターのサービスによって検出された外部 IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-120">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="0fcd8-121">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0fcd8-121">Read-only</span></span>|
|<span data-ttu-id="0fcd8-122">id</span><span class="sxs-lookup"><span data-stu-id="0fcd8-122">id</span></span>|<span data-ttu-id="0fcd8-123">String</span><span class="sxs-lookup"><span data-stu-id="0fcd8-123">String</span></span>| <span data-ttu-id="0fcd8-124">コネクタのオブジェクト id。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-124">The object id of the connector.</span></span> <BR><span data-ttu-id="0fcd8-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-125">Read-only.</span></span>|
|<span data-ttu-id="0fcd8-126">マシン</span><span class="sxs-lookup"><span data-stu-id="0fcd8-126">machineName</span></span>|<span data-ttu-id="0fcd8-127">String</span><span class="sxs-lookup"><span data-stu-id="0fcd8-127">String</span></span>| <span data-ttu-id="0fcd8-128">コネクタが実行されているコンピューターの名前。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-128">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="0fcd8-129">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0fcd8-129">Read-only</span></span>|
|<span data-ttu-id="0fcd8-130">status</span><span class="sxs-lookup"><span data-stu-id="0fcd8-130">status</span></span>|<span data-ttu-id="0fcd8-131">string</span><span class="sxs-lookup"><span data-stu-id="0fcd8-131">string</span></span>| <span data-ttu-id="0fcd8-132">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-132">Indicates the status of the connector.</span></span> <span data-ttu-id="0fcd8-133">可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-133">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="0fcd8-134">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="0fcd8-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="0fcd8-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0fcd8-135">Relationships</span></span>
| <span data-ttu-id="0fcd8-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0fcd8-136">Relationship</span></span> | <span data-ttu-id="0fcd8-137">型</span><span class="sxs-lookup"><span data-stu-id="0fcd8-137">Type</span></span>   |<span data-ttu-id="0fcd8-138">説明</span><span class="sxs-lookup"><span data-stu-id="0fcd8-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0fcd8-139">memberOf</span><span class="sxs-lookup"><span data-stu-id="0fcd8-139">memberOf</span></span>|<span data-ttu-id="0fcd8-140">[コネクタグループ](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0fcd8-140">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="0fcd8-141">接続がメンバーであるコネクタグループ。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-141">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="0fcd8-142">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-142">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0fcd8-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fcd8-143">JSON representation</span></span>

<span data-ttu-id="0fcd8-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fcd8-144">Here is a JSON representation of the resource.</span></span>

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
