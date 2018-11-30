---
title: セキュリティ リソースの種類
description: セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。 シングルトンのセキュリティ リソースを返します。 使用可能なプロパティが含まれていません。
ms.openlocfilehash: ddf00e46135733ef18c18918c0c365134138671f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021140"
---
# <a name="security-resource-type"></a><span data-ttu-id="d095b-105">セキュリティ リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d095b-105">security resource type</span></span>

<span data-ttu-id="d095b-106">セキュリティ リソースは、セキュリティ オブジェクト モデルのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="d095b-106">The security resource is the entry point for the Security object model.</span></span> <span data-ttu-id="d095b-107">シングルトンのセキュリティ リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="d095b-107">It returns a singleton security resource.</span></span> <span data-ttu-id="d095b-108">使用可能なプロパティが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="d095b-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="d095b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d095b-109">Methods</span></span>

| <span data-ttu-id="d095b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d095b-110">Method</span></span>       | <span data-ttu-id="d095b-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d095b-111">Return Type</span></span> | <span data-ttu-id="d095b-112">説明</span><span class="sxs-lookup"><span data-stu-id="d095b-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d095b-113">警告の一覧表示</span><span class="sxs-lookup"><span data-stu-id="d095b-113">List alerts</span></span>](../api/alert-list.md) | <span data-ttu-id="d095b-114">[アラート](alert.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d095b-114">[alert](alert.md) collection</span></span> | <span data-ttu-id="d095b-115">Alert オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d095b-115">Get a alert object collection.</span></span> |
| [<span data-ttu-id="d095b-116">アラートを取得します。</span><span class="sxs-lookup"><span data-stu-id="d095b-116">get alerts</span></span>](../api/alert-get.md) | <span data-ttu-id="d095b-117">[アラート](alert.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d095b-117">[alert](alert.md) collection</span></span> | <span data-ttu-id="d095b-118">Alert オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d095b-118">Get a alert object.</span></span> |
| [<span data-ttu-id="d095b-119">アラートを更新します。</span><span class="sxs-lookup"><span data-stu-id="d095b-119">Update alerts</span></span>](../api/alert-update.md) | <span data-ttu-id="d095b-120">[アラート](alert.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d095b-120">[alert](alert.md) collection</span></span> | <span data-ttu-id="d095b-121">Alert オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="d095b-121">Get a alert object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d095b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d095b-122">Properties</span></span>
<span data-ttu-id="d095b-123">なし</span><span class="sxs-lookup"><span data-stu-id="d095b-123">None</span></span>

## <a name="relationships"></a><span data-ttu-id="d095b-124">関係</span><span class="sxs-lookup"><span data-stu-id="d095b-124">Relationships</span></span>
| <span data-ttu-id="d095b-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d095b-125">Relationship</span></span> | <span data-ttu-id="d095b-126">型</span><span class="sxs-lookup"><span data-stu-id="d095b-126">Type</span></span>        | <span data-ttu-id="d095b-127">説明</span><span class="sxs-lookup"><span data-stu-id="d095b-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d095b-128">alerts</span><span class="sxs-lookup"><span data-stu-id="d095b-128">alerts</span></span>|<span data-ttu-id="d095b-129">[アラート](alert.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="d095b-129">[alert](alert.md) collection</span></span>| <span data-ttu-id="d095b-p103">読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d095b-p103">Read-only. Nullable.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="d095b-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d095b-132">JSON representation</span></span>
<span data-ttu-id="d095b-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d095b-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.security"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="d095b-134">使用例</span><span class="sxs-lookup"><span data-stu-id="d095b-134">Example</span></span>

<span data-ttu-id="d095b-135">**セキュリティ**リソースは、グラフのルートに使用できます。</span><span class="sxs-lookup"><span data-stu-id="d095b-135">The **security** resource is available at the root of the graph.</span></span>

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