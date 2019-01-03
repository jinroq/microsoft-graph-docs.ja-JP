---
title: Microsoft Graph で SharePoint サイトを開く
description: Microsoft Graph の SharePoint API は、以下の基本的なシナリオをサポートしています。
ms.openlocfilehash: e7150f5b437358b3ddb484640463b2f92d5416eb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073324"
---
# <a name="working-with-sharepoint-sites-in-microsoft-graph"></a><span data-ttu-id="25192-103">Microsoft Graph で SharePoint サイトを開く</span><span class="sxs-lookup"><span data-stu-id="25192-103">Working with SharePoint sites in Microsoft Graph</span></span>

<span data-ttu-id="25192-104">Microsoft Graph の SharePoint API は、以下の基本的なシナリオをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="25192-104">The SharePoint API in Microsoft Graph supports the following core scenarios:</span></span>

* <span data-ttu-id="25192-105">SharePoint **サイト**、**リスト**、および**ドライブ** (ドキュメント ライブラリ) へのアクセス</span><span class="sxs-lookup"><span data-stu-id="25192-105">Access to SharePoint **sites**, **lists**, and **drives** (document libraries)</span></span>
* <span data-ttu-id="25192-106">**サイト** リソースの読み取り専用サポート (新しいサイトは作成できません)</span><span class="sxs-lookup"><span data-stu-id="25192-106">Read-only support for **site** resources (no ability to create new sites)</span></span>
* <span data-ttu-id="25192-107">**リスト**、**listItem** および **driveItem** の読み取り/書き込みサポート</span><span class="sxs-lookup"><span data-stu-id="25192-107">Read-write support for **lists**, **listItems**, and **driveItems**</span></span>
* <span data-ttu-id="25192-108">SharePoint ID、URL、または相対パスでリソースを指定する</span><span class="sxs-lookup"><span data-stu-id="25192-108">Address resources by SharePoint ID, URL, or relative path</span></span>

<span data-ttu-id="25192-109">SharePoint API は、次の 3 つの主要なリソースの種類を公開します。</span><span class="sxs-lookup"><span data-stu-id="25192-109">The SharePoint API exposes three major resource types:</span></span>

* <span data-ttu-id="25192-110">[サイト](site.md) _(最上位のオブジェクト)_</span><span class="sxs-lookup"><span data-stu-id="25192-110">[Site](site.md) _(top-level object)_</span></span>
* [<span data-ttu-id="25192-111">リスト</span><span class="sxs-lookup"><span data-stu-id="25192-111">List</span></span>](list.md)
* [<span data-ttu-id="25192-112">ListItem</span><span class="sxs-lookup"><span data-stu-id="25192-112">ListItem</span></span>](listitem.md)

<span data-ttu-id="25192-113">次に、listItem リソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="25192-113">The following is an example of a listItem resource.</span></span>

```json
{
  "fields": {
    "Title": "Access card",
    "Employee": "Ryan Gregg",
    "EmployeeId": "10",
    "CardSerial": "01235492",
    "Alias": "RGregg",
    "ID": 1,
    "ContentType": "Item",
    "Modified": "2016-09-19T23:15:25-07:00",
    "Created": "2016-09-19T23:15:25-07:00"
  },
  "createdBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "createdDateTime": "2016-09-20T06:15:25Z",
  "eTag": "48e941c3-9515-4c48-9760-c07c90c79d48,1",
  "id": "4",
  "lastModifiedBy": {
    "user": {
      "id": "b757fdcb-0271-4807-b243-504139e4ba04",
      "displayName": "Ryan Gregg"
    }
  },
  "lastModifiedDateTime": "2016-09-20T06:15:25Z",
}
```

<span data-ttu-id="25192-114">リソースでは、次の異なる 3 つの方法でデータを公開します。</span><span class="sxs-lookup"><span data-stu-id="25192-114">Resources expose data in three different ways:</span></span>

* <span data-ttu-id="25192-115">_プロパティ_ (**id** や **name** など) は単純な値を公開します。</span><span class="sxs-lookup"><span data-stu-id="25192-115">_Properties_ (like **id** and **name**) expose simple values.</span></span>
* <span data-ttu-id="25192-116">_ファセット_(**フィールド** や **createdBy** など) は複雑な値を公開します。</span><span class="sxs-lookup"><span data-stu-id="25192-116">_Facets_ (like **fields** and **createdBy**) expose complex values.</span></span>
* <span data-ttu-id="25192-117">_参照_ (**items** など) はその他のリソースのコレクションを指します。</span><span class="sxs-lookup"><span data-stu-id="25192-117">_References_ (like **items**) point to collections of other resources.</span></span>

<span data-ttu-id="25192-118">`?expand=fields` などの _expand_ クエリ パラメーターで、URL 内の参照を展開することができます。</span><span class="sxs-lookup"><span data-stu-id="25192-118">You can expand references in your URL with the _expand_ query parameter; for example, `?expand=fields`.</span></span>
<span data-ttu-id="25192-119">`?select=id,name` などの _select_ クエリ パラメーターで、特定のプロパティやファセットを要求することができます。</span><span class="sxs-lookup"><span data-stu-id="25192-119">You can request specific properties and facets with the _select_ query parameter; for example, `?select=id,name`.</span></span>
<span data-ttu-id="25192-120">既定では、プロパティとファセットはほとんどが返されるのに対し、参照はいずれも表示されません。</span><span class="sxs-lookup"><span data-stu-id="25192-120">By default, most properties and facets are returned while all references are hidden.</span></span>
<span data-ttu-id="25192-121">効率を高めるには、注目すべきデータだけに _select_ と _expand_ を返すことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="25192-121">For efficiency, we recommend that you specify _select_ and _expand_ to only return the data you care about.</span></span>

## <a name="sharepoint-api-root-resources"></a><span data-ttu-id="25192-122">SharePoint API のルート リソース</span><span class="sxs-lookup"><span data-stu-id="25192-122">SharePoint API root resources</span></span>

<span data-ttu-id="25192-123">以下は、`https://graph.microsoft.com/beta` に関する例です。</span><span class="sxs-lookup"><span data-stu-id="25192-123">The following examples are relative to `https://graph.microsoft.com/beta`.</span></span>

| <span data-ttu-id="25192-124">パス</span><span class="sxs-lookup"><span data-stu-id="25192-124">Path</span></span>                                   | <span data-ttu-id="25192-125">説明</span><span class="sxs-lookup"><span data-stu-id="25192-125">Description</span></span>
|:---------------------------------------|:------------------------------------
| <span data-ttu-id="25192-126">/sites/root</span><span class="sxs-lookup"><span data-stu-id="25192-126">/sites/root</span></span>                            | <span data-ttu-id="25192-127">組織の既定の[サイト][]</span><span class="sxs-lookup"><span data-stu-id="25192-127">Organization's default [site][].</span></span>
| <span data-ttu-id="25192-128">/sites/{site-id}</span><span class="sxs-lookup"><span data-stu-id="25192-128">/sites/{site-id}</span></span>                       | <span data-ttu-id="25192-129">ID を使って特定の[サイト][]にアクセスする</span><span class="sxs-lookup"><span data-stu-id="25192-129">Access a specific [site][] by its ID.</span></span>
| <span data-ttu-id="25192-130">/sites/{site-id}/drive</span><span class="sxs-lookup"><span data-stu-id="25192-130">/sites/{site-id}/drive</span></span>                 | <span data-ttu-id="25192-131">指定した[サイト][]の既定の[ドライブ](drive.md) (ドキュメント ライブラリ) にアクセスする</span><span class="sxs-lookup"><span data-stu-id="25192-131">Access the default [drive](drive.md) (document library) for the given [site][].</span></span>
| <span data-ttu-id="25192-132">/sites/{site-id}/drives</span><span class="sxs-lookup"><span data-stu-id="25192-132">/sites/{site-id}/drives</span></span>                | <span data-ttu-id="25192-133">[サイト][]の下にある[ドライブ](drive.md) (ドキュメント ライブラリ) を列挙する。</span><span class="sxs-lookup"><span data-stu-id="25192-133">Enumerate the [drives](drive.md) (document libraries) under the [site][].</span></span>
| <span data-ttu-id="25192-134">/sites/{site-id}/sites</span><span class="sxs-lookup"><span data-stu-id="25192-134">/sites/{site-id}/sites</span></span>                 | <span data-ttu-id="25192-135">[サイト][]の下のサブサイトを列挙する。</span><span class="sxs-lookup"><span data-stu-id="25192-135">Enumerate the sub-sites under the [site][].</span></span>
| <span data-ttu-id="25192-136">/sites/{site-id}/lists</span><span class="sxs-lookup"><span data-stu-id="25192-136">/sites/{site-id}/lists</span></span>                 | <span data-ttu-id="25192-137">[サイト](site.md)の下の[リスト](list.md)を列挙する。</span><span class="sxs-lookup"><span data-stu-id="25192-137">Enumerate the [lists](list.md) under the [site](site.md).</span></span>
| <span data-ttu-id="25192-138">/sites/{site-id}/lists/{list-id}/items</span><span class="sxs-lookup"><span data-stu-id="25192-138">/sites/{site-id}/lists/{list-id}/items</span></span> | <span data-ttu-id="25192-139">[リスト](list.md)の下の [listItem](listitem.md) を列挙する。</span><span class="sxs-lookup"><span data-stu-id="25192-139">Enumerate the [listItems](listitem.md) under the [list](list.md).</span></span>
| <span data-ttu-id="25192-140">/groups/{group-id}/sites/root</span><span class="sxs-lookup"><span data-stu-id="25192-140">/groups/{group-id}/sites/root</span></span>          | <span data-ttu-id="25192-141">グループのチーム [サイト][]にアクセスする</span><span class="sxs-lookup"><span data-stu-id="25192-141">Access a group's team [site][].</span></span>

<span data-ttu-id="25192-p102">サイトは、SharePoint のホスト名の後にコロンとサイトへの相対パスを入れる形で指定できます。最後にコロン (:) を入れるとリソースモデル指定画面に戻れます (オプション)。</span><span class="sxs-lookup"><span data-stu-id="25192-p102">Sites can also be addressed by path by using the SharePoint hostname, followed by a colon and the relative path to the site. You can optionally transition back to addressing the resource model by putting another colon at the end.</span></span>

| <span data-ttu-id="25192-144">パス</span><span class="sxs-lookup"><span data-stu-id="25192-144">Path</span></span>                                           | <span data-ttu-id="25192-145">説明</span><span class="sxs-lookup"><span data-stu-id="25192-145">Description</span></span>
|:-----------------------------------------------|:-----------------------------------
| <span data-ttu-id="25192-146">/sites/contoso.sharepoint.com:/teams/hr</span><span class="sxs-lookup"><span data-stu-id="25192-146">/sites/contoso.sharepoint.com:/teams/hr</span></span>        | <span data-ttu-id="25192-147">関連付けられているサイトhttps://contoso.sharepoint.com/teams/hr</span><span class="sxs-lookup"><span data-stu-id="25192-147">The site associated with https://contoso.sharepoint.com/teams/hr</span></span>
| <span data-ttu-id="25192-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span><span class="sxs-lookup"><span data-stu-id="25192-148">/sites/contoso.sharepoint.com:/teams/hr:/drive</span></span> | <span data-ttu-id="25192-149">このサイトの既定の[ドライブ](drive.md)にアクセスする</span><span class="sxs-lookup"><span data-stu-id="25192-149">Access the default [drive](drive.md) for this site.</span></span>

## <a name="note-for-existing-sharepoint-developers"></a><span data-ttu-id="25192-150">既存の SharePoint 開発者向けのメモ</span><span class="sxs-lookup"><span data-stu-id="25192-150">Note for existing SharePoint developers</span></span>

<span data-ttu-id="25192-p103">Microsoft Graph の SharePoint API は、CSOM API と大きく異なる点がいくつかあります。[サイト][]のリソースは `SPWeb` にマッピングされます。サイト コレクションのルート[サイト][] (`SPWeb`) には、`SPSite` に関する情報を含む [siteCollection](sitecollection.md) ファセットが含まれています。サイトの ID はそのサイト コレクション内でのみ一意であり、ID でサイトを指定する場合、サイト コレクション識別子とサイト識別子の両方を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="25192-p103">The Microsoft Graph SharePoint API has a few key differences with the CSOM APIs. The [site][] resource maps to `SPWeb`. The root [site][] (`SPWeb`) in a site collection has a [siteCollection](sitecollection.md) facet, which contains information about the `SPSite`. Because IDs for sites are only unique within their site collection, addressing a site by ID requires providing both the site collection identifier and the site identifier.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id},{spweb-id}/
```
<span data-ttu-id="25192-155">ホスト名のみで作成された URL は、既定のサイト コレクションのルート サイト (`SPWeb`) をポイントします。</span><span class="sxs-lookup"><span data-stu-id="25192-155">A URL constructed with only the hostname will point to the root site (`SPWeb`) in the default site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname}
```

<span data-ttu-id="25192-156">ホスト名と siteCollection (`SPSite`) ID のみで作成された URL は、指定したサイト コレクションのルート サイト (`SPWeb`) をポイントします。</span><span class="sxs-lookup"><span data-stu-id="25192-156">A URL constructed with only the hostname and siteCollection (`SPSite`) ID will point to the root site (`SPWeb`) in the given site collection.</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{hostname},{spsite-id}
```

[site]: site.md
[list]: list.md
[drive]: drive.md
[siteCollection]: sitecollection.md

<!-- {
  "type": "#page.annotation",
  "description": "Getting started programming with the SharePoint API",
  "keywords": "getting started sharepoint rest api programming C# ios android rest http",
  "section": "documentation",
  "tocPath": "Getting Started",
  "tocIndex": -100
} -->