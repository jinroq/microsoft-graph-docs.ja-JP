---
title: outlookUser リソースの種類
description: ユーザーが利用できる Outlook サービスを表します。
author: angelgolfer-ms
ms.openlocfilehash: 3a65206c74d16f7943d986e38b520ef388803c22
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314743"
---
# <a name="outlookuser-resource-type"></a><span data-ttu-id="21471-103">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21471-103">outlookUser resource type</span></span>


<span data-ttu-id="21471-104">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="21471-104">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="21471-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="21471-105">Methods</span></span>

| <span data-ttu-id="21471-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="21471-106">Method</span></span>           | <span data-ttu-id="21471-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21471-107">Return Type</span></span>    |<span data-ttu-id="21471-108">説明</span><span class="sxs-lookup"><span data-stu-id="21471-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="21471-109">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="21471-109">Create category</span></span>](../api/outlookuser-post-mastercategories.md) | [<span data-ttu-id="21471-110">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="21471-110">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="21471-111">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="21471-111">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="21471-112">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="21471-112">List categories</span></span>](../api/outlookuser-list-mastercategories.md) | <span data-ttu-id="21471-113">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21471-113">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="21471-114">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="21471-114">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="21471-115">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="21471-115">supportedLanguages</span></span>](../api/outlookuser-supportedlanguages.md) | <span data-ttu-id="21471-116">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21471-116">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="21471-117">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="21471-117">Get the list of locales and languages that is supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="21471-118">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="21471-118">supportedTimeZones</span></span>](../api/outlookuser-supportedtimezones.md) | <span data-ttu-id="21471-119">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21471-119">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="21471-120">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="21471-120">Get the list of time zones that is supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="21471-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21471-121">Properties</span></span>
<span data-ttu-id="21471-122">なし</span><span class="sxs-lookup"><span data-stu-id="21471-122">None</span></span>

## <a name="relationships"></a><span data-ttu-id="21471-123">関係</span><span class="sxs-lookup"><span data-stu-id="21471-123">Relationships</span></span>
| <span data-ttu-id="21471-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21471-124">Relationship</span></span> | <span data-ttu-id="21471-125">型</span><span class="sxs-lookup"><span data-stu-id="21471-125">Type</span></span>   |<span data-ttu-id="21471-126">説明</span><span class="sxs-lookup"><span data-stu-id="21471-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21471-127">masterCategories</span><span class="sxs-lookup"><span data-stu-id="21471-127">masterCategories</span></span>|<span data-ttu-id="21471-128">[outlookCategory](../resources/outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="21471-128">[outlookCategory](../resources/outlookcategory.md) collection</span></span>| <span data-ttu-id="21471-129">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="21471-129">A list of categories defined for the user.</span></span> | 

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