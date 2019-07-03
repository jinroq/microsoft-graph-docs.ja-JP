---
title: 'スケジュール: 共有'
description: スケジュールの時間範囲をスケジュールのメンバーと共有します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d28ecff0f83487e9040bfb7a0336648e27b20196
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457549"
---
# <a name="schedule-share"></a><span data-ttu-id="6a508-103">スケジュール: 共有</span><span class="sxs-lookup"><span data-stu-id="6a508-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a508-104">スケジュールの[](../resources/schedule.md)時間範囲をスケジュールのメンバーと共有します。</span><span class="sxs-lookup"><span data-stu-id="6a508-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="6a508-105">指定されたチームメンバーによって表示可能な[スケジュール](../resources/schedule.md)の指定された時間範囲で、 [Shift](../resources/shift.md)と[timeoff](../resources/timeoff.md)の各アイテムのコレクションを作成します (従業員とマネージャーを含む)。</span><span class="sxs-lookup"><span data-stu-id="6a508-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="6a508-106">[スケジュール](../resources/schedule.md)内の各[シフト](../resources/shift.md)および[timeoff](../resources/timeoff.md)インスタンスでは、アイテムの下書きバージョンと共有バージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="6a508-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="6a508-107">下書きバージョンは、管理者のみが表示でき、共有バージョンは従業員とマネージャーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="6a508-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="6a508-108">指定した時間範囲の各[シフト](../resources/shift.md)と[timeoff](../resources/timeoff.md)のインスタンスについては、共有アクションは下書きバージョンの共有バージョンを更新するので、マネージャーに加えて、アイテムに関する最新情報を表示することもできます。</span><span class="sxs-lookup"><span data-stu-id="6a508-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="6a508-109">**Notifyteam**パラメーターは、アイテムを表示できる従業員をさらに指定します。</span><span class="sxs-lookup"><span data-stu-id="6a508-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a508-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6a508-110">Permissions</span></span>

<span data-ttu-id="6a508-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a508-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a508-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a508-113">Permission type</span></span>      | <span data-ttu-id="6a508-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a508-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a508-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a508-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6a508-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a508-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6a508-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a508-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a508-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a508-118">Not supported.</span></span>    |
|<span data-ttu-id="6a508-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a508-119">Application</span></span> | <span data-ttu-id="6a508-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a508-120">Not supported.</span></span> |

> <span data-ttu-id="6a508-121">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6a508-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6a508-122">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6a508-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6a508-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a508-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="6a508-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a508-124">Request headers</span></span>

| <span data-ttu-id="6a508-125">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a508-125">Header</span></span>       | <span data-ttu-id="6a508-126">値</span><span class="sxs-lookup"><span data-stu-id="6a508-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6a508-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a508-127">Authorization</span></span>  | <span data-ttu-id="6a508-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6a508-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6a508-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6a508-130">Content-Type</span></span>  | <span data-ttu-id="6a508-131">application/json</span><span class="sxs-lookup"><span data-stu-id="6a508-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6a508-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a508-132">Request body</span></span>

<span data-ttu-id="6a508-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6a508-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="6a508-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6a508-134">Parameter</span></span>                   |<span data-ttu-id="6a508-135">型</span><span class="sxs-lookup"><span data-stu-id="6a508-135">Type</span></span>           |<span data-ttu-id="6a508-136">説明</span><span class="sxs-lookup"><span data-stu-id="6a508-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="6a508-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="6a508-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="6a508-138">チーム全体がこのアクションの通知を表示するかどうかを指定します。または、共有されていた交代が割り当てられた従業員のみを取得します。</span><span class="sxs-lookup"><span data-stu-id="6a508-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="6a508-139">必須です。</span><span class="sxs-lookup"><span data-stu-id="6a508-139">Required.</span></span>       |
| <span data-ttu-id="6a508-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6a508-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="6a508-141">スケジュールの開始時刻を開始する時刻。</span><span class="sxs-lookup"><span data-stu-id="6a508-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="6a508-142">必須です。</span><span class="sxs-lookup"><span data-stu-id="6a508-142">Required.</span></span>   |
| <span data-ttu-id="6a508-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6a508-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="6a508-144">スケジュールによる移動を終了するまでの終了時刻。</span><span class="sxs-lookup"><span data-stu-id="6a508-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="6a508-145">応答</span><span class="sxs-lookup"><span data-stu-id="6a508-145">Response</span></span>

<span data-ttu-id="6a508-p107">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6a508-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a508-148">例</span><span class="sxs-lookup"><span data-stu-id="6a508-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6a508-149">要求</span><span class="sxs-lookup"><span data-stu-id="6a508-149">Request</span></span>

<span data-ttu-id="6a508-150">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a508-150">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a508-151">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6a508-151">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="6a508-152">C#</span><span class="sxs-lookup"><span data-stu-id="6a508-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-share-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a508-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="6a508-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-share-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a508-154">目的-C</span><span class="sxs-lookup"><span data-stu-id="6a508-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-share-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6a508-155">応答</span><span class="sxs-lookup"><span data-stu-id="6a508-155">Response</span></span>

<span data-ttu-id="6a508-156">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6a508-156">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

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
  ]
}
-->
