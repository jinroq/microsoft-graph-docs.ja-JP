---
title: 'スケジュール: 共有'
description: スケジュールの時間範囲をスケジュールのメンバーと共有します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e2d4678434fdaa546aaab3d8bb5557db365eb1ee
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264898"
---
# <a name="schedule-share"></a><span data-ttu-id="e9e5e-103">スケジュール: 共有</span><span class="sxs-lookup"><span data-stu-id="e9e5e-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9e5e-104">スケジュールの[](../resources/schedule.md)時間範囲をスケジュールのメンバーと共有します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="e9e5e-105">指定されたチームメンバーによって表示可能な[スケジュール](../resources/schedule.md)の指定された時間範囲で、 [Shift](../resources/shift.md)と[timeoff](../resources/timeoff.md)の各アイテムのコレクションを作成します (従業員とマネージャーを含む)。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="e9e5e-106">[スケジュール](../resources/schedule.md)内の各[シフト](../resources/shift.md)および[timeoff](../resources/timeoff.md)インスタンスでは、アイテムの下書きバージョンと共有バージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="e9e5e-107">下書きバージョンは、管理者のみが表示でき、共有バージョンは従業員とマネージャーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="e9e5e-108">指定した時間範囲の各[シフト](../resources/shift.md)と[timeoff](../resources/timeoff.md)のインスタンスについては、共有アクションは下書きバージョンの共有バージョンを更新するので、マネージャーに加えて、アイテムに関する最新情報を表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="e9e5e-109">**Notifyteam**パラメーターは、アイテムを表示できる従業員をさらに指定します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="e9e5e-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e9e5e-110">Permissions</span></span>

<span data-ttu-id="e9e5e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e9e5e-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e9e5e-113">Permission type</span></span>      | <span data-ttu-id="e9e5e-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e9e5e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e9e5e-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e9e5e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e9e5e-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9e5e-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e9e5e-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e9e5e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e9e5e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-118">Not supported.</span></span>    |
|<span data-ttu-id="e9e5e-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e9e5e-119">Application</span></span> | <span data-ttu-id="e9e5e-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-120">Not supported.</span></span> |

> <span data-ttu-id="e9e5e-121">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e9e5e-122">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e9e5e-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e9e5e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="e9e5e-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9e5e-124">Request headers</span></span>

| <span data-ttu-id="e9e5e-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e9e5e-125">Header</span></span>       | <span data-ttu-id="e9e5e-126">値</span><span class="sxs-lookup"><span data-stu-id="e9e5e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e9e5e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e9e5e-127">Authorization</span></span>  | <span data-ttu-id="e9e5e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e9e5e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e9e5e-130">Content-Type</span></span>  | <span data-ttu-id="e9e5e-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e9e5e-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e9e5e-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="e9e5e-132">Request body</span></span>

<span data-ttu-id="e9e5e-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="e9e5e-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e9e5e-134">Parameter</span></span>                   |<span data-ttu-id="e9e5e-135">型</span><span class="sxs-lookup"><span data-stu-id="e9e5e-135">Type</span></span>           |<span data-ttu-id="e9e5e-136">説明</span><span class="sxs-lookup"><span data-stu-id="e9e5e-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="e9e5e-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="e9e5e-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="e9e5e-138">チーム全体がこのアクションの通知を表示するかどうかを指定します。または、共有されていた交代が割り当てられた従業員のみを取得します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="e9e5e-139">必須です。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-139">Required.</span></span>       |
| <span data-ttu-id="e9e5e-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e5e-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="e9e5e-141">スケジュールの開始時刻を開始する時刻。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="e9e5e-142">必須です。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-142">Required.</span></span>   |
| <span data-ttu-id="e9e5e-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e9e5e-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="e9e5e-144">スケジュールによる移動を終了するまでの終了時刻。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="e9e5e-145">応答</span><span class="sxs-lookup"><span data-stu-id="e9e5e-145">Response</span></span>

<span data-ttu-id="e9e5e-p107">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9e5e-148">例</span><span class="sxs-lookup"><span data-stu-id="e9e5e-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="e9e5e-149">要求</span><span class="sxs-lookup"><span data-stu-id="e9e5e-149">Request</span></span>

<span data-ttu-id="e9e5e-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```

#### <a name="response"></a><span data-ttu-id="e9e5e-151">応答</span><span class="sxs-lookup"><span data-stu-id="e9e5e-151">Response</span></span>

<span data-ttu-id="e9e5e-152">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9e5e-152">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e9e5e-153">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e9e5e-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e9e5e-154">C#</span><span class="sxs-lookup"><span data-stu-id="e9e5e-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-share-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e9e5e-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="e9e5e-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-share-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e9e5e-156">目的-C</span><span class="sxs-lookup"><span data-stu-id="e9e5e-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-share-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
