---
title: 作成するか、historyItem を置き換える
description: 新規作成または既存のユーザー アクティビティの既存の履歴項目を置換します。
ms.openlocfilehash: a33c5cb295ce0cd954c37154bc85eac0322937e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023808"
---
# <a name="create-or-replace-a-historyitem"></a><span data-ttu-id="5bb98-103">作成するか、historyItem を置き換える</span><span class="sxs-lookup"><span data-stu-id="5bb98-103">Create or replace a historyItem</span></span>

<span data-ttu-id="5bb98-104">新規作成または既存のユーザー アクティビティの既存の履歴項目を置換します。</span><span class="sxs-lookup"><span data-stu-id="5bb98-104">Create a new or replace an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bb98-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5bb98-105">Permissions</span></span>

<span data-ttu-id="5bb98-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bb98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bb98-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bb98-108">Permission type</span></span>      | <span data-ttu-id="5bb98-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bb98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bb98-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5bb98-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5bb98-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5bb98-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bb98-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="5bb98-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="5bb98-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bb98-114">Application</span></span> | <span data-ttu-id="5bb98-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bb98-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bb98-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bb98-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{id}/historyItems/{id}
```

<span data-ttu-id="5bb98-117">Id は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bb98-117">Id needs to be a GUID.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bb98-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bb98-118">Request headers</span></span>

|<span data-ttu-id="5bb98-119">名前</span><span class="sxs-lookup"><span data-stu-id="5bb98-119">Name</span></span> | <span data-ttu-id="5bb98-120">型</span><span class="sxs-lookup"><span data-stu-id="5bb98-120">Type</span></span> | <span data-ttu-id="5bb98-121">説明</span><span class="sxs-lookup"><span data-stu-id="5bb98-121">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="5bb98-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb98-122">Authorization</span></span> | <span data-ttu-id="5bb98-123">string</span><span class="sxs-lookup"><span data-stu-id="5bb98-123">string</span></span> | <span data-ttu-id="5bb98-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5bb98-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb98-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bb98-126">Request body</span></span>

<span data-ttu-id="5bb98-127">要求の本文には、 [historyItem](../resources/projectrome-historyitem.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="5bb98-127">In the request body, supply a JSON representation of a [historyItem](../resources/projectrome-historyitem.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5bb98-128">応答</span><span class="sxs-lookup"><span data-stu-id="5bb98-128">Response</span></span>

<span data-ttu-id="5bb98-129">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、historyItem が作成されている場合、応答コードまたは`200 OK`、historyItem を交換した場合。</span><span class="sxs-lookup"><span data-stu-id="5bb98-129">If successful, this method returns the `201 Created` response code if the historyItem was created or `200 OK` if the historyItem was replaced.</span></span>

## <a name="example"></a><span data-ttu-id="5bb98-130">例</span><span class="sxs-lookup"><span data-stu-id="5bb98-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5bb98-131">要求</span><span class="sxs-lookup"><span data-stu-id="5bb98-131">Request</span></span>

<span data-ttu-id="5bb98-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bb98-132">Here is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_historyItem"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/{activity-id}/historyItems/{item-id}
Content-type: application/json
Content-length: 364

{
    "startedDateTime": "2015-02-11T20:54:04.3457274+00:00",
    "userTimezone": "Africa/Casablanca",
    "lastActiveDateTime": "2015-02-11T20:54:04.3457274+00:00"
}
```

#### <a name="response"></a><span data-ttu-id="5bb98-133">応答</span><span class="sxs-lookup"><span data-stu-id="5bb98-133">Response</span></span>

<span data-ttu-id="5bb98-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="5bb98-134">Here is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activityHistoryItem"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('user%40contoso.com')/activities('13881113971988980728')/historyItems/$entity",
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