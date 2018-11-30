---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
ms.openlocfilehash: 63bbabccc540046961d31c91fe7b1fb9afaaf4f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023521"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="ff6cb-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff6cb-103">outlookUser resource type</span></span>


<span data-ttu-id="ff6cb-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="ff6cb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff6cb-105">Methods</span></span>

| <span data-ttu-id="ff6cb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff6cb-106">Method</span></span>           | <span data-ttu-id="ff6cb-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ff6cb-107">Return Type</span></span>    |<span data-ttu-id="ff6cb-108">説明</span><span class="sxs-lookup"><span data-stu-id="ff6cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff6cb-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="ff6cb-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="ff6cb-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="ff6cb-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="ff6cb-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="ff6cb-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="ff6cb-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="ff6cb-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff6cb-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="ff6cb-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="ff6cb-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="ff6cb-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="ff6cb-116">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff6cb-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="ff6cb-117">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="ff6cb-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="ff6cb-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="ff6cb-119">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff6cb-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="ff6cb-120">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="ff6cb-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff6cb-121">Properties</span></span>
<span data-ttu-id="ff6cb-122">なし</span><span class="sxs-lookup"><span data-stu-id="ff6cb-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ff6cb-123">関係</span><span class="sxs-lookup"><span data-stu-id="ff6cb-123">Relationships</span></span>
| <span data-ttu-id="ff6cb-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff6cb-124">Relationship</span></span> | <span data-ttu-id="ff6cb-125">型</span><span class="sxs-lookup"><span data-stu-id="ff6cb-125">Type</span></span>   |<span data-ttu-id="ff6cb-126">説明</span><span class="sxs-lookup"><span data-stu-id="ff6cb-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff6cb-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="ff6cb-127">masterCategories</span></span>|<span data-ttu-id="ff6cb-128">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ff6cb-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="ff6cb-129">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="ff6cb-129">A list of categories defined for the user.</span></span> | 

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.outlookUser",
  "@odata.annotations": [
    {
      "property": "masterCategories",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->