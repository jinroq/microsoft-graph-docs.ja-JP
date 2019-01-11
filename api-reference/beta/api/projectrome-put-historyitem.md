---
title: 作成するか、historyItem を置き換える
description: 新規作成または既存のユーザー アクティビティの既存の履歴項目を置換します。
localization_priority: Normal
ms.openlocfilehash: 008e4bc8470ffddce4f60f71bdff68ca13ad39c5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807890"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="00cdb-103">作成するか、historyItem を置き換える</span><span class="sxs-lookup"><span data-stu-id="00cdb-103">Create or replace a historyItem</span></span>

> <span data-ttu-id="00cdb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="00cdb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00cdb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cdb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00cdb-106">新規作成または既存のユーザー アクティビティの既存の履歴項目を置換します。</span><span class="sxs-lookup"><span data-stu-id="00cdb-106">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="00cdb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="00cdb-107">Permissions</span></span>

<span data-ttu-id="00cdb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00cdb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="00cdb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00cdb-110">Permission type</span></span>      | <span data-ttu-id="00cdb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="00cdb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00cdb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00cdb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="00cdb-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="00cdb-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="00cdb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00cdb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00cdb-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="00cdb-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="00cdb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00cdb-116">Application</span></span> | <span data-ttu-id="00cdb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cdb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="00cdb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00cdb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="00cdb-119">Id は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="00cdb-119">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00cdb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00cdb-120">Request headers</span></span>

|<span data-ttu-id="00cdb-121">名前</span><span class="sxs-lookup"><span data-stu-id="00cdb-121">Name</span></span> | <span data-ttu-id="00cdb-122">種類</span><span class="sxs-lookup"><span data-stu-id="00cdb-122">Type</span></span> | <span data-ttu-id="00cdb-123">説明</span><span class="sxs-lookup"><span data-stu-id="00cdb-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="00cdb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="00cdb-124">Authorization</span></span> | <span data-ttu-id="00cdb-125">string</span><span class="sxs-lookup"><span data-stu-id="00cdb-125">string</span></span> | <span data-ttu-id="00cdb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="00cdb-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00cdb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="00cdb-128">Request body</span></span>

<span data-ttu-id="00cdb-129">要求の本文には、 [historyItem](../resources/projectrome-historyitem.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="00cdb-129">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="00cdb-130">応答</span><span class="sxs-lookup"><span data-stu-id="00cdb-130">Response</span></span>

<span data-ttu-id="00cdb-131">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、historyItem が作成されている場合、応答コードまたは`200 OK`、historyItem を交換した場合。</span><span class="sxs-lookup"><span data-stu-id="00cdb-131">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="00cdb-132">例</span><span class="sxs-lookup"><span data-stu-id="00cdb-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="00cdb-133">要求</span><span class="sxs-lookup"><span data-stu-id="00cdb-133">Request</span></span>

<span data-ttu-id="00cdb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00cdb-134">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="00cdb-135">応答</span><span class="sxs-lookup"><span data-stu-id="00cdb-135">Response</span></span>

<span data-ttu-id="00cdb-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="00cdb-136">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.historyItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
    "status": "updated",
    "userTimezone": "Africa/Casablanca",
    "createdDateTime": "2018-02-26T20:28:22.14Z",
    "lastModifiedDateTime": "2018-02-26T20:28:22.155Z",
    "id": "9d0b74e4-4b41-43ea-b34d-f9c1bf9f809c",
    "startedDateTime": "2018-02-26T20:54:04.345Z",
    "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
    "expirationDateTime": "2018-03-28T20:28:22.14Z",
    "activeDurationSeconds": 20
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
