---
title: スケジュールを取得する
description: '**Schedule**オブジェクトのプロパティとリレーションシップを取得します。'
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40e796700df1013825ed5267712619ab59803b4d
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638999"
---
# <a name="get-schedule"></a><span data-ttu-id="d38ff-103">スケジュールを取得する</span><span class="sxs-lookup"><span data-stu-id="d38ff-103">Get schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38ff-104">[Schedule](../resources/schedule.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="d38ff-104">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="d38ff-105">スケジュール作成プロセスは、[リソースベースの長時間実行操作 (RELO) に関する1つの API ガイドライン](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)に準拠しています。</span><span class="sxs-lookup"><span data-stu-id="d38ff-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="d38ff-106">クライアントが[PUT メソッド](team-put-schedule.md)を使用すると、スケジュールが準備されている場合、操作によってスケジュールが更新されます。それ以外の場合、操作はバックグラウンドでスケジュールプロビジョニングプロセスを開始します。</span><span class="sxs-lookup"><span data-stu-id="d38ff-106">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="d38ff-107">スケジュールの準備中に、クライアントは GET メソッドを使用してスケジュールを取得し`provisionStatus` 、プロパティでプロビジョニングの現在の状態を確認できます。</span><span class="sxs-lookup"><span data-stu-id="d38ff-107">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="d38ff-108">プロビジョニングが失敗した場合、クライアントは`provisionStatusCode`プロパティから追加情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="d38ff-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="d38ff-109">クライアントは、スケジュールの構成を検査することもできます。</span><span class="sxs-lookup"><span data-stu-id="d38ff-109">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="d38ff-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d38ff-110">Permissions</span></span>

<span data-ttu-id="d38ff-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d38ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d38ff-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d38ff-113">Permission type</span></span>      | <span data-ttu-id="d38ff-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d38ff-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d38ff-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d38ff-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d38ff-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d38ff-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d38ff-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d38ff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d38ff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d38ff-118">Not supported.</span></span>    |
|<span data-ttu-id="d38ff-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d38ff-119">Application</span></span> | <span data-ttu-id="d38ff-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d38ff-120">Not supported.</span></span> |

> <span data-ttu-id="d38ff-121">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d38ff-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d38ff-122">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d38ff-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d38ff-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d38ff-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="d38ff-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d38ff-124">Request headers</span></span>

| <span data-ttu-id="d38ff-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d38ff-125">Header</span></span>       | <span data-ttu-id="d38ff-126">値</span><span class="sxs-lookup"><span data-stu-id="d38ff-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d38ff-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d38ff-127">Authorization</span></span>  | <span data-ttu-id="d38ff-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d38ff-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d38ff-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d38ff-130">Content-Type</span></span>  | <span data-ttu-id="d38ff-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d38ff-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d38ff-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="d38ff-132">Request body</span></span>
<span data-ttu-id="d38ff-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d38ff-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d38ff-134">応答</span><span class="sxs-lookup"><span data-stu-id="d38ff-134">Response</span></span>

<span data-ttu-id="d38ff-135">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schedule](../resources/schedule.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d38ff-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d38ff-136">例</span><span class="sxs-lookup"><span data-stu-id="d38ff-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d38ff-137">要求</span><span class="sxs-lookup"><span data-stu-id="d38ff-137">Request</span></span>

<span data-ttu-id="d38ff-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d38ff-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```

#### <a name="response"></a><span data-ttu-id="d38ff-139">応答</span><span class="sxs-lookup"><span data-stu-id="d38ff-139">Response</span></span>

<span data-ttu-id="d38ff-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d38ff-140">The following is an example of the response.</span></span> 

><span data-ttu-id="d38ff-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d38ff-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d38ff-143">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="d38ff-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d38ff-144">Visual</span><span class="sxs-lookup"><span data-stu-id="d38ff-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d38ff-145">Java</span><span class="sxs-lookup"><span data-stu-id="d38ff-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
