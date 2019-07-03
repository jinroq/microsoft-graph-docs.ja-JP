---
title: スケジュールを作成または置換する
description: '**Schedule**オブジェクトを作成または置換します。'
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 94a8249f8a11f74d0266a417454c892052e4176a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458426"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="a9057-103">スケジュールを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="a9057-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9057-104">[Schedule](../resources/schedule.md)オブジェクトを作成または置換します。</span><span class="sxs-lookup"><span data-stu-id="a9057-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="a9057-105">スケジュール作成プロセスは、[リソースベースの長時間実行操作 (RELO) に関する1つの API ガイドライン](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)に準拠しています。</span><span class="sxs-lookup"><span data-stu-id="a9057-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="a9057-106">クライアントが PUT メソッドを使用する場合、スケジュールが準備されていると、この操作によってスケジュールが置き換えられます。それ以外の場合、操作はバックグラウンドでスケジュールプロビジョニングプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="a9057-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="a9057-107">スケジュールの準備中に、クライアントは[get メソッド](schedule-get.md)を使用してスケジュールを取得し`provisionStatus` 、プロパティでプロビジョニングの現在の状態を確認できます。</span><span class="sxs-lookup"><span data-stu-id="a9057-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="a9057-108">プロビジョニングが失敗した場合、クライアントは`provisionStatusCode`プロパティから追加情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="a9057-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="a9057-109">クライアントは、スケジュールの構成を検査することもできます。</span><span class="sxs-lookup"><span data-stu-id="a9057-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="a9057-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a9057-110">Permissions</span></span>

<span data-ttu-id="a9057-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9057-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9057-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9057-113">Permission type</span></span>      | <span data-ttu-id="a9057-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9057-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a9057-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9057-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a9057-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9057-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a9057-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9057-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9057-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9057-118">Not supported.</span></span>    |
|<span data-ttu-id="a9057-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9057-119">Application</span></span> | <span data-ttu-id="a9057-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9057-120">Not supported.</span></span> |

> <span data-ttu-id="a9057-121">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a9057-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a9057-122">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="a9057-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a9057-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9057-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="a9057-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9057-124">Request headers</span></span>

| <span data-ttu-id="a9057-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9057-125">Header</span></span>       | <span data-ttu-id="a9057-126">値</span><span class="sxs-lookup"><span data-stu-id="a9057-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a9057-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9057-127">Authorization</span></span>  | <span data-ttu-id="a9057-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a9057-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a9057-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a9057-130">Content-Type</span></span>  | <span data-ttu-id="a9057-131">application/json</span><span class="sxs-lookup"><span data-stu-id="a9057-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a9057-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9057-132">Request body</span></span>

<span data-ttu-id="a9057-133">要求本文で、 [schedule](../resources/schedule.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9057-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a9057-134">応答</span><span class="sxs-lookup"><span data-stu-id="a9057-134">Response</span></span>

<span data-ttu-id="a9057-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schedule](../resources/schedule.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9057-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9057-136">例</span><span class="sxs-lookup"><span data-stu-id="a9057-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a9057-137">要求</span><span class="sxs-lookup"><span data-stu-id="a9057-137">Request</span></span>

<span data-ttu-id="a9057-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9057-138">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a9057-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="a9057-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9057-140">C#</span><span class="sxs-lookup"><span data-stu-id="a9057-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/team-put-schedule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9057-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="a9057-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/team-put-schedule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9057-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="a9057-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/team-put-schedule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9057-143">応答</span><span class="sxs-lookup"><span data-stu-id="a9057-143">Response</span></span>

<span data-ttu-id="a9057-144">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a9057-144">The following is an example of the response.</span></span> 

><span data-ttu-id="a9057-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="a9057-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
