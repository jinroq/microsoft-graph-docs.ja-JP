---
title: historyItem リソースの種類
description: アプリケーション内のアクティビティの履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
ms.openlocfilehash: f413da4280f7b39f0be2a9dafd872ebee041ccc8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022870"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="99175-106">historyItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99175-106">historyItem resource type</span></span>

<span data-ttu-id="99175-107">アプリケーション内の[アクティビティ](projectrome-activity.md)の履歴項目を表します。</span><span class="sxs-lookup"><span data-stu-id="99175-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="99175-108">ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。</span><span class="sxs-lookup"><span data-stu-id="99175-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="99175-109">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="99175-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="99175-110">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="99175-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="99175-111">アプリケーションは、セッションを作成するときは、ユーザー契約の期間を反映するように**アクティビティ**オブジェクトに**historyItem**オブジェクトを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99175-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="99175-112">ユーザーは、再活動と連携して、たびに、新しい**historyItem**がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="99175-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="99175-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="99175-113">Methods</span></span>

|<span data-ttu-id="99175-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="99175-114">Method</span></span> | <span data-ttu-id="99175-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="99175-115">Return Type</span></span> | <span data-ttu-id="99175-116">説明</span><span class="sxs-lookup"><span data-stu-id="99175-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="99175-117">作成または置換 historyItem</span><span class="sxs-lookup"><span data-stu-id="99175-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="99175-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="99175-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="99175-119">作成するか、その活動 (アップサート) の既存の**historyItem**に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="99175-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="99175-120">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="99175-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="99175-121">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="99175-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="99175-122">内容なし</span><span class="sxs-lookup"><span data-stu-id="99175-122">No Content</span></span> | <span data-ttu-id="99175-123">そのアクティビティに指定された**historyItem**を削除します。</span><span class="sxs-lookup"><span data-stu-id="99175-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="99175-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99175-124">Properties</span></span>

|<span data-ttu-id="99175-125">名前</span><span class="sxs-lookup"><span data-stu-id="99175-125">Name</span></span> | <span data-ttu-id="99175-126">型</span><span class="sxs-lookup"><span data-stu-id="99175-126">Type</span></span> | <span data-ttu-id="99175-127">説明</span><span class="sxs-lookup"><span data-stu-id="99175-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="99175-128">status</span><span class="sxs-lookup"><span data-stu-id="99175-128">status</span></span> | <span data-ttu-id="99175-129">status</span><span class="sxs-lookup"><span data-stu-id="99175-129">status</span></span> | <span data-ttu-id="99175-130">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="99175-130">Set by the server.</span></span> <span data-ttu-id="99175-131">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="99175-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="99175-132">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="99175-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="99175-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="99175-133">userTimezone</span></span> | <span data-ttu-id="99175-134">String</span><span class="sxs-lookup"><span data-stu-id="99175-134">String</span></span> | <span data-ttu-id="99175-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="99175-135">Optional.</span></span> <span data-ttu-id="99175-136">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="99175-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="99175-137">クロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="99175-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="99175-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99175-138">createdDateTime</span></span> | <span data-ttu-id="99175-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99175-139">DateTimeOffset</span></span> | <span data-ttu-id="99175-140">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="99175-140">Set by the server.</span></span> <span data-ttu-id="99175-141">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="99175-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="99175-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99175-142">lastModifiedDateTime</span></span> | <span data-ttu-id="99175-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99175-143">DateTimeOffset</span></span> | <span data-ttu-id="99175-144">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="99175-144">Set by the server.</span></span> <span data-ttu-id="99175-145">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="99175-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="99175-146">id</span><span class="sxs-lookup"><span data-stu-id="99175-146">id</span></span> | <span data-ttu-id="99175-147">String</span><span class="sxs-lookup"><span data-stu-id="99175-147">String</span></span> | <span data-ttu-id="99175-148">必須。</span><span class="sxs-lookup"><span data-stu-id="99175-148">Required.</span></span> <span data-ttu-id="99175-149">**HistoryItem**オブジェクトの GUID をクライアントに設定します。</span><span class="sxs-lookup"><span data-stu-id="99175-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="99175-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="99175-150">startedDateTime</span></span> | <span data-ttu-id="99175-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99175-151">DateTimeOffset</span></span> | <span data-ttu-id="99175-152">必須。</span><span class="sxs-lookup"><span data-stu-id="99175-152">Required.</span></span> <span data-ttu-id="99175-153">**HistoryItem** (アクティビティ セッション) が開始されたときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="99175-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="99175-154">タイムラインの履歴が必要です。</span><span class="sxs-lookup"><span data-stu-id="99175-154">Required for timeline history.</span></span>|
|<span data-ttu-id="99175-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="99175-155">lastActiveDateTime</span></span> | <span data-ttu-id="99175-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99175-156">DateTimeOffset</span></span> | <span data-ttu-id="99175-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="99175-157">Optional.</span></span> <span data-ttu-id="99175-158">**HistoryItem** (アクティビティ セッション) がアクティブまたは終了の null の場合、 **historyItem**の状態として理解された最後のときの UTC 日時は、継続中にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="99175-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="99175-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99175-159">expirationDateTime</span></span> | <span data-ttu-id="99175-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99175-160">DateTimeOffset</span></span> | <span data-ttu-id="99175-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="99175-161">Optional.</span></span> <span data-ttu-id="99175-162">**HistoryItem**がハード削除を行うときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="99175-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="99175-163">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="99175-163">Can be set by the client.</span></span>|
|<span data-ttu-id="99175-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="99175-164">activeDurationSeconds</span></span> | <span data-ttu-id="99175-165">int</span><span class="sxs-lookup"><span data-stu-id="99175-165">int</span></span> | <span data-ttu-id="99175-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="99175-166">Optional.</span></span> <span data-ttu-id="99175-167">アクティブなユーザーの活動の期間です。</span><span class="sxs-lookup"><span data-stu-id="99175-167">The duration of active user engagement.</span></span> <span data-ttu-id="99175-168">指定されなかった場合、この**startedDateTime**と**lastActiveDateTime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="99175-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99175-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="99175-169">Relationships</span></span>

|<span data-ttu-id="99175-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="99175-170">Relationship</span></span> | <span data-ttu-id="99175-171">型</span><span class="sxs-lookup"><span data-stu-id="99175-171">Type</span></span> | <span data-ttu-id="99175-172">説明</span><span class="sxs-lookup"><span data-stu-id="99175-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="99175-173">activity</span><span class="sxs-lookup"><span data-stu-id="99175-173">activity</span></span>| [<span data-ttu-id="99175-174">userActivity</span><span class="sxs-lookup"><span data-stu-id="99175-174">userActivity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="99175-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="99175-175">Optional.</span></span> <span data-ttu-id="99175-176">受け取りますおよび抑制ソリューションです。ナビゲーション プロパティに関連する活動です。</span><span class="sxs-lookup"><span data-stu-id="99175-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99175-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99175-177">JSON representation</span></span>

<span data-ttu-id="99175-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="99175-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
