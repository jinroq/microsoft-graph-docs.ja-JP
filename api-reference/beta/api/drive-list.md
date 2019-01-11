---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ドライブを一覧表示する
localization_priority: Normal
ms.openlocfilehash: 81b5221e9c2823ac9729310d002f755e1c63e061
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843408"
---
# <a name="list-available-drives"></a><span data-ttu-id="291c9-102">利用可能なドライブの一覧表示</span><span class="sxs-lookup"><span data-stu-id="291c9-102">List available drives</span></span>

> <span data-ttu-id="291c9-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="291c9-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="291c9-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="291c9-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="291c9-105">ターゲットとなる User、Group、または [Site](../resources/site.md) が利用可能な [Drive](../resources/drive.md) リソースの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="291c9-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="291c9-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="291c9-106">Permissions</span></span>

<span data-ttu-id="291c9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="291c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="291c9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="291c9-109">Permission type</span></span>      | <span data-ttu-id="291c9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="291c9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="291c9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="291c9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="291c9-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="291c9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="291c9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="291c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="291c9-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="291c9-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="291c9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="291c9-115">Application</span></span> | <span data-ttu-id="291c9-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="291c9-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="291c9-117">グループのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="291c9-117">List a group's drives</span></span>

<span data-ttu-id="291c9-118">グループのドキュメント ライブラリを一覧表示するために、アプリが Group の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="291c9-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="291c9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="291c9-119">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a><span data-ttu-id="291c9-120">サイトのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="291c9-120">List a site's drives</span></span>

<span data-ttu-id="291c9-121">サイトのドキュメント ライブラリを一覧表示するために、アプリは Site の **drives** リレーションシップを要求します。</span><span class="sxs-lookup"><span data-stu-id="291c9-121">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a><span data-ttu-id="291c9-122">ユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="291c9-122">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a><span data-ttu-id="291c9-123">現在のユーザーのドライブを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="291c9-123">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="291c9-124">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="291c9-124">Optional query parameters</span></span>

<span data-ttu-id="291c9-125">このメソッドは、応答をカスタマイズするための `$expand`、`$select`、`$skipToken`、`$top`、`$orderby` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="291c9-125">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="291c9-126">応答</span><span class="sxs-lookup"><span data-stu-id="291c9-126">Response</span></span>

<span data-ttu-id="291c9-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [Drive](../resources/drive.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="291c9-127">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="291c9-128">備考</span><span class="sxs-lookup"><span data-stu-id="291c9-128">Remarks</span></span>

<span data-ttu-id="291c9-129">ほとんどのユーザーには、ドライブ リソースが 1 つしかありません。</span><span class="sxs-lookup"><span data-stu-id="291c9-129">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="291c9-130">Group と Site には、複数の Drive リソースが利用可能である場合があります。</span><span class="sxs-lookup"><span data-stu-id="291c9-130">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="291c9-131">[system][] ファセットのあるドライブは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="291c9-131">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="291c9-132">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="291c9-132">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
