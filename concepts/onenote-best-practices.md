---
title: Microsoft Graph で OneNote API を使用する場合のベスト プラクティス
description: この記事では、Microsoft Graph で OneNote API を使用するための推奨事項を提供します。 これらの推奨事項は、Stack Overflow と Twitter でよく寄せられる質問への回答に基づいています。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 95c135ec405764a53f06fed2f9ac2dde6b4138bd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560915"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a><span data-ttu-id="9f249-104">Microsoft Graph で OneNote API を使用する場合の推奨事項</span><span class="sxs-lookup"><span data-stu-id="9f249-104">Best practices for working with the OneNote API in Microsoft Graph</span></span>

<span data-ttu-id="9f249-105">この記事では、Microsoft Graph で OneNote API を使用するための推奨事項を提供します。</span><span class="sxs-lookup"><span data-stu-id="9f249-105">This article provides recommendations for working with the OneNote APIs in Microsoft Graph.</span></span> <span data-ttu-id="9f249-106">これらの推奨事項は、Stack Overflow と Twitter でよく寄せられる質問への回答に基づいています。</span><span class="sxs-lookup"><span data-stu-id="9f249-106">These recommendations are based on answers to common questions on Stack Overflow and Twitter.</span></span>

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a><span data-ttu-id="9f249-107">$Select を使用して、必要なプロパティの最小限のセットを選択する</span><span class="sxs-lookup"><span data-stu-id="9f249-107">Use $select to select the minimum set of properties you need</span></span>

<span data-ttu-id="9f249-108">リソース (たとえば、ノートブック内のセクション) のクエリを実行するときには、次のような要求を行います。</span><span class="sxs-lookup"><span data-stu-id="9f249-108">When you query for a resource (for example, sections inside a notebook), you make a request similar to the following.</span></span>

```http
GET ~/notebooks/{id}/sections
```

<span data-ttu-id="9f249-109">これは、セクションのすべてのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="9f249-109">This retrieves all the properties of the sections.</span></span> <span data-ttu-id="9f249-110">ただし、すべてのプロパティが必要とは限りません。</span><span class="sxs-lookup"><span data-stu-id="9f249-110">However, you might not need all properties.</span></span> <span data-ttu-id="9f249-111">次の例のように、`$select` クエリ パラメーターを使用して、必要なプロパティだけを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="9f249-111">You can use the `$select` query parameter to return just the properties that you want, as shown in the following example.</span></span>

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

<span data-ttu-id="9f249-112">同じアプローチは、他の OneNote API に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9f249-112">The same approach applies to other OneNote APIs.</span></span>

## <a name="use-expand-instead-of-making-multiple-api-calls"></a><span data-ttu-id="9f249-113">複数の API 呼び出しを実行するのではなく、$expand を使用します。</span><span class="sxs-lookup"><span data-stu-id="9f249-113">Use $expand instead of making multiple API calls</span></span>

<span data-ttu-id="9f249-114">ユーザーのノートブック、セクション、およびセクション グループのすべてを階層的なビューで取得します。</span><span class="sxs-lookup"><span data-stu-id="9f249-114">Suppose you want to retrieve all of the user’s notebooks, sections, and section groups in a hierarchical view.</span></span> <span data-ttu-id="9f249-115">次の方法でこれを行います。</span><span class="sxs-lookup"><span data-stu-id="9f249-115">You might accomplish that by doing the following:</span></span>

* <span data-ttu-id="9f249-116">`GET ~/notebooks` を呼び出して、ノートブックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f249-116">Call `GET ~/notebooks` to get the list of notebooks.</span></span>

* <span data-ttu-id="9f249-117">取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sections` を呼び出してセクションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f249-117">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sections` to retrieve the list of sections.</span></span>

* <span data-ttu-id="9f249-118">取得したすべてのノートブックについて、`GET ~/notebooks/{notebookId}/sectionGroups` を呼び出してセクション グループの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="9f249-118">For every retrieved notebook, call `GET ~/notebooks/{notebookId}/sectionGroups` to retrieve the list of section groups.</span></span>

* <span data-ttu-id="9f249-119">必要に応じて、セクション グループを再帰的に反復処理できます。</span><span class="sxs-lookup"><span data-stu-id="9f249-119">Optionally recursively iterate through section groups.</span></span>

<span data-ttu-id="9f249-120">この方法 (サービスへ何回かの連続した余分なラウンドトリップを実行) でも可能ですが、より優れたアプローチは、`$expand` クエリ パラメーターを使用することです。</span><span class="sxs-lookup"><span data-stu-id="9f249-120">While this will work (with a few extra sequential roundtrips to the service), a better approach is to use the `$expand` query parameter.</span></span> 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

<span data-ttu-id="9f249-121">これにより、1 回のネットワーク ラウンドトリップで同じ結果が得られ、より良いパフォーマンスが得られます。</span><span class="sxs-lookup"><span data-stu-id="9f249-121">This will yield the same results in one network roundtrip, with better performance.</span></span>

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a><span data-ttu-id="9f249-122">ユーザーに対してすべてのページを取得する場合は、セクションごとに個別に行ってください。</span><span class="sxs-lookup"><span data-stu-id="9f249-122">When getting all pages for a user, do so for each section separately</span></span>

<span data-ttu-id="9f249-123">Microsoft Graph はすべてのページを取得するためにエンドポイントを公開しますが、これはユーザーがアクセス権を持っているすべてのページを取得する最良の方法ではありません。</span><span class="sxs-lookup"><span data-stu-id="9f249-123">While Microsoft Graph exposes an endpoint to retrieve all pages, this isn't the best way to get all the pages the user has access to.</span></span> <span data-ttu-id="9f249-124">ユーザーが持つセクションが多すぎると、これによりタイムアウトやパフォーマンスの低下を招きます。</span><span class="sxs-lookup"><span data-stu-id="9f249-124">When the user has too many sections, this can lead to timeouts or bad performance.</span></span> <span data-ttu-id="9f249-125">各セクションを反復処理して、個別にそれぞれのページを取得することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9f249-125">It is better to iterate each section, getting pages for each one separately.</span></span>

<span data-ttu-id="9f249-126">たとえば、この呼び出しを使用する代わりに、(この API はページ化されているので、すべてのページを一度にフェッチすることはできません):</span><span class="sxs-lookup"><span data-stu-id="9f249-126">For example, instead of using this call (this API is paged, so you won't be able to fetch the pages all at once):</span></span>

```http
GET ~/pages
```

<span data-ttu-id="9f249-127">(特にすべてのセクションが必要ない場合は) 次の呼び出しを何回か使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9f249-127">It is better to use the following call several times (especially if you don't need all sections):</span></span>

```http
GET ~/sections/{id}/pages
```

<span data-ttu-id="9f249-128">ページのメタデータを取得するには、既定値 `lastModifiedDateTime` の順序付けを上書きします。</span><span class="sxs-lookup"><span data-stu-id="9f249-128">When getting page metadata, override the default `lastModifiedDateTime` ordering.</span></span> <span data-ttu-id="9f249-129">それらを `lastModifiedDateTime` で並べ替える必要がないときには、より速くページを取得できます。</span><span class="sxs-lookup"><span data-stu-id="9f249-129">It is faster to get pages when you don't have to sort them by `lastModifiedDateTime`.</span></span> <span data-ttu-id="9f249-130">これを行うには、たとえば他の任意のプロパティで並べ替えることができます。</span><span class="sxs-lookup"><span data-stu-id="9f249-130">To do this, you can sort by any other property; for example:</span></span>

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
