---
title: コネクタ リソースの種類
description: 以下は、リソースの JSON 表記です。
ms.openlocfilehash: 6d4cb7e5ca1a5384dbb6c8be92e7ce4eb107388a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072932"
---
# <a name="connector-resource-type"></a><span data-ttu-id="3dd4d-103">コネクタ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3dd4d-103">connector resource type</span></span>

> <span data-ttu-id="3dd4d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3dd4d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-105">Use of these APIs in production applications is not supported.</span></span>

<!-- Not supported items
|[Create connectorGroup](../api/connector-post-memberof.md) |[connectorGroup](connectorgroup.md)| Associate a connector with a new connectorGroup by posting to the memberOf collection.|
|[Update](../api/connector-update.md) | [connector](connector.md)   | Connectors are created when they are registed with the tenant. |
|[Delete](../api/connector-delete.md) | None |Delete connector object. |

-->

## <a name="methods"></a><span data-ttu-id="3dd4d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3dd4d-106">Methods</span></span>

| <span data-ttu-id="3dd4d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3dd4d-107">Method</span></span>           | <span data-ttu-id="3dd4d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3dd4d-108">Return Type</span></span>    |<span data-ttu-id="3dd4d-109">説明</span><span class="sxs-lookup"><span data-stu-id="3dd4d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3dd4d-110">コネクタを取得します。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-110">Get connector</span></span>](../api/connector-get.md) | [<span data-ttu-id="3dd4d-111">コネクタ</span><span class="sxs-lookup"><span data-stu-id="3dd4d-111">connector</span></span>](connector.md) |<span data-ttu-id="3dd4d-112">コネクタ オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-112">Read properties and relationships of connector object.</span></span>|
|[<span data-ttu-id="3dd4d-113">memberOf を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="3dd4d-113">List memberOf</span></span>](../api/connector-list-memberof.md) |<span data-ttu-id="3dd4d-114">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3dd4d-114">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="3dd4d-115">コネクタに関連付けられている connectorGroup オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-115">Get the connectorGroup object associated with the connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="3dd4d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd4d-116">Properties</span></span>
| <span data-ttu-id="3dd4d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dd4d-117">Property</span></span>     | <span data-ttu-id="3dd4d-118">型</span><span class="sxs-lookup"><span data-stu-id="3dd4d-118">Type</span></span>   |<span data-ttu-id="3dd4d-119">説明</span><span class="sxs-lookup"><span data-stu-id="3dd4d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dd4d-120">externalIp</span><span class="sxs-lookup"><span data-stu-id="3dd4d-120">externalIp</span></span>|<span data-ttu-id="3dd4d-121">String</span><span class="sxs-lookup"><span data-stu-id="3dd4d-121">String</span></span>|<span data-ttu-id="3dd4d-122">コネクタ コンピューターのサービスによって検出されたと外部の IP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-122">The external IP address as detected by the service for the connector machine.</span></span> <span data-ttu-id="3dd4d-123">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="3dd4d-123">Read-only</span></span>|
|<span data-ttu-id="3dd4d-124">id</span><span class="sxs-lookup"><span data-stu-id="3dd4d-124">id</span></span>|<span data-ttu-id="3dd4d-125">String</span><span class="sxs-lookup"><span data-stu-id="3dd4d-125">String</span></span>| <span data-ttu-id="3dd4d-126">コネクタのオブジェクト id です。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-126">The object id of the connector.</span></span> <BR><span data-ttu-id="3dd4d-127">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-127">Read-only.</span></span>|
|<span data-ttu-id="3dd4d-128">マシン名</span><span class="sxs-lookup"><span data-stu-id="3dd4d-128">machineName</span></span>|<span data-ttu-id="3dd4d-129">String</span><span class="sxs-lookup"><span data-stu-id="3dd4d-129">String</span></span>| <span data-ttu-id="3dd4d-130">コネクタが実行されているマシンの名前です。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-130">The name of the machine that the connector is running on.</span></span> <BR><span data-ttu-id="3dd4d-131">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="3dd4d-131">Read-only</span></span>|
|<span data-ttu-id="3dd4d-132">status</span><span class="sxs-lookup"><span data-stu-id="3dd4d-132">status</span></span>|<span data-ttu-id="3dd4d-133">文字列</span><span class="sxs-lookup"><span data-stu-id="3dd4d-133">string</span></span>| <span data-ttu-id="3dd4d-134">コネクタの状態を示します。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-134">Indicates the status of the connector.</span></span> <span data-ttu-id="3dd4d-135">使用可能な値は、`active`、`inactive` です。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-135">Possible values are: `active`, `inactive`.</span></span> <span data-ttu-id="3dd4d-136">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="3dd4d-136">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="3dd4d-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3dd4d-137">Relationships</span></span>
| <span data-ttu-id="3dd4d-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3dd4d-138">Relationship</span></span> | <span data-ttu-id="3dd4d-139">型</span><span class="sxs-lookup"><span data-stu-id="3dd4d-139">Type</span></span>   |<span data-ttu-id="3dd4d-140">説明</span><span class="sxs-lookup"><span data-stu-id="3dd4d-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dd4d-141">memberOf</span><span class="sxs-lookup"><span data-stu-id="3dd4d-141">memberOf</span></span>|<span data-ttu-id="3dd4d-142">[connectorGroup](connectorgroup.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3dd4d-142">[connectorGroup](connectorgroup.md) collection</span></span>| <span data-ttu-id="3dd4d-143">接続がのメンバーである connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-143">The connectorGroup that the connect is a member of.</span></span><br><span data-ttu-id="3dd4d-144">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-144">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3dd4d-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dd4d-145">JSON representation</span></span>

<span data-ttu-id="3dd4d-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3dd4d-146">Here is a JSON representation of the resource.</span></span>

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
