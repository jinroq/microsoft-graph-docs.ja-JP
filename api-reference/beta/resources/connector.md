---
title: コネクタ リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 98fa998a37b01ad64e556b229912932f4d1cfc75
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884624"
---
# <a name="connector-resource-type"></a><span data-ttu-id="1195f-103">コネクタ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1195f-103">connector resource type</span></span>

> <span data-ttu-id="1195f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1195f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1195f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1195f-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="1195f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1195f-106">Methods</span></span>

| <span data-ttu-id="1195f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1195f-107">Method</span></span>           | <span data-ttu-id="1195f-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1195f-108">Return Type</span></span>    |<span data-ttu-id="1195f-109">説明</span><span class="sxs-lookup"><span data-stu-id="1195f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1195f-110">コネクタを取得します。</span><span class="sxs-lookup"><span data-stu-id="1195f-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="1195f-111">コネクタ</span><span class="sxs-lookup"><span data-stu-id="1195f-111">connector</span></span>](connector.md) |<span data-ttu-id="1195f-112">コネクタ オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1195f-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="1195f-113">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1195f-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="1195f-114">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1195f-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="1195f-115">コネクタに関連付けられている connectorGroup オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1195f-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="1195f-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1195f-116">Properties</span></span>
| <span data-ttu-id="1195f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1195f-117">Property</span></span>     | <span data-ttu-id="1195f-118">種類</span><span class="sxs-lookup"><span data-stu-id="1195f-118">Type</span></span>   |<span data-ttu-id="1195f-119">説明</span><span class="sxs-lookup"><span data-stu-id="1195f-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1195f-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="1195f-120">externalIp</span></span>|<span data-ttu-id="1195f-121">String</span><span class="sxs-lookup"><span data-stu-id="1195f-121">String</span></span>|<span data-ttu-id="1195f-122">コネクタ コンピューターのサービスによって検出されたと外部の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1195f-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="1195f-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1195f-123">Read-only</span></span>|
|<span data-ttu-id="1195f-124">id</span><span class="sxs-lookup"><span data-stu-id="1195f-124">id</span></span>|<span data-ttu-id="1195f-125">String</span><span class="sxs-lookup"><span data-stu-id="1195f-125">String</span></span>| <span data-ttu-id="1195f-126">コネクタのオブジェクト id です。</span><span class="sxs-lookup"><span data-stu-id="1195f-126">The object id of the connector.</span></span> <BR><span data-ttu-id="1195f-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1195f-127">Read-only.</span></span>|
|<span data-ttu-id="1195f-128">マシン名</span><span class="sxs-lookup"><span data-stu-id="1195f-128">machineName</span></span>|<span data-ttu-id="1195f-129">String</span><span class="sxs-lookup"><span data-stu-id="1195f-129">String</span></span>| <span data-ttu-id="1195f-130">コネクタが実行されているマシンの名前です。</span><span class="sxs-lookup"><span data-stu-id="1195f-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="1195f-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1195f-131">Read-only</span></span>|
|<span data-ttu-id="1195f-132">status</span><span class="sxs-lookup"><span data-stu-id="1195f-132">status</span></span>|<span data-ttu-id="1195f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1195f-133">string</span></span>| <span data-ttu-id="1195f-134">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="1195f-134">Indicates the status of the connector.</span></span> <span data-ttu-id="1195f-135">使用可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="1195f-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="1195f-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1195f-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="1195f-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1195f-137">Relationships</span></span>
| <span data-ttu-id="1195f-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1195f-138">Relationship</span></span> | <span data-ttu-id="1195f-139">型</span><span class="sxs-lookup"><span data-stu-id="1195f-139">Type</span></span>   |<span data-ttu-id="1195f-140">説明</span><span class="sxs-lookup"><span data-stu-id="1195f-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1195f-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="1195f-141">memberOf</span></span>|<span data-ttu-id="1195f-142">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1195f-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="1195f-143">接続がのメンバーである connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="1195f-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="1195f-144">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1195f-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1195f-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1195f-145">JSON representation</span></span>

<span data-ttu-id="1195f-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1195f-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "connector resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
