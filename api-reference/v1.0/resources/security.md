---
title: セキュリティリソースの種類
description: セキュリティリソースは、セキュリティオブジェクトモデルのエントリポイントです。 単一のセキュリティリソースを返します。 使用可能なプロパティは含まれていません。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7bf3f279e50efb451188426d030e356d55ad6be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579213"
---
# <a name="security-resource-type"></a><span data-ttu-id="58106-105">セキュリティリソースの種類</span><span class="sxs-lookup"><span data-stu-id="58106-105">security resource type</span></span>

<span data-ttu-id="58106-106">セキュリティリソースは、セキュリティオブジェクトモデルのエントリポイントです。</span><span class="sxs-lookup"><span data-stu-id="58106-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="58106-107">単一のセキュリティリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="58106-107">It returns a singleton security resource.</span></span> <span data-ttu-id="58106-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="58106-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="58106-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="58106-109">Methods</span></span>

| <span data-ttu-id="58106-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="58106-110">Method</span></span>       | <span data-ttu-id="58106-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58106-111">Return Type</span></span> | <span data-ttu-id="58106-112">説明</span><span class="sxs-lookup"><span data-stu-id="58106-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="58106-113">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="58106-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="58106-114">[alert](alert.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58106-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="58106-115">通知オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="58106-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="58106-116">通知を取得する</span><span class="sxs-lookup"><span data-stu-id="58106-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="58106-117">[alert](alert.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58106-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="58106-118">通知オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="58106-118">Get a alert object.</span></span> |
| [<span data-ttu-id="58106-119">アラートを更新する</span><span class="sxs-lookup"><span data-stu-id="58106-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="58106-120">[alert](alert.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58106-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="58106-121">通知オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="58106-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="58106-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58106-122">Properties</span></span>
<span data-ttu-id="58106-123">なし</span><span class="sxs-lookup"><span data-stu-id="58106-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="58106-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58106-124">Relationships</span></span>
| <span data-ttu-id="58106-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58106-125">Relationship</span></span> | <span data-ttu-id="58106-126">型</span><span class="sxs-lookup"><span data-stu-id="58106-126">Type</span></span>        | <span data-ttu-id="58106-127">説明</span><span class="sxs-lookup"><span data-stu-id="58106-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58106-128">アラート</span><span class="sxs-lookup"><span data-stu-id="58106-128">alerts</span></span>|<span data-ttu-id="58106-129">[alert](alert.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58106-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="58106-p103">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="58106-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="58106-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58106-132">JSON representation</span></span>
<span data-ttu-id="58106-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58106-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="58106-134">例</span><span class="sxs-lookup"><span data-stu-id="58106-134">Example</span></span>

<span data-ttu-id="58106-135">**セキュリティ**リソースは、グラフのルートで使用できます。</span><span class="sxs-lookup"><span data-stu-id="58106-135">The **security** resource is available at the root of the graph.</span></span>

<!--{
  "blockType": "request"
}-->
```http
GET https://graph.microsoft.com/v1.0/security
```

<!--{
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security"
}-->
```json
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "security resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
