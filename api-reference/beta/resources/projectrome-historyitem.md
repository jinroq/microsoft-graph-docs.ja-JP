---
title: historyItem リソースの種類
description: アプリケーション内のアクティビティの履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.openlocfilehash: 7eb6d72b55530d1938c9c092dd5b80f54929a3e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825775"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="21416-106">historyItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21416-106">historyItem resource type</span></span>

> <span data-ttu-id="21416-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21416-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21416-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21416-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="21416-109">アプリケーション内の[アクティビティ](projectrome-activity.md)の履歴項目を表します。</span><span class="sxs-lookup"><span data-stu-id="21416-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="21416-110">ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。</span><span class="sxs-lookup"><span data-stu-id="21416-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="21416-111">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="21416-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="21416-112">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="21416-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="21416-113">アプリケーションは、セッションを作成するときは、ユーザー契約の期間を反映するように**アクティビティ**オブジェクトに**historyItem**オブジェクトを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="21416-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="21416-114">ユーザーは、再活動と連携して、たびに、新しい**historyItem**がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="21416-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="21416-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="21416-115">Methods</span></span>

|<span data-ttu-id="21416-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="21416-116">Method</span></span> | <span data-ttu-id="21416-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="21416-117">Return Type</span></span> | <span data-ttu-id="21416-118">説明</span><span class="sxs-lookup"><span data-stu-id="21416-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="21416-119">作成または置換 historyItem</span><span class="sxs-lookup"><span data-stu-id="21416-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="21416-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="21416-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="21416-121">作成するか、その活動 (アップサート) の既存の**historyItem**に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="21416-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="21416-122">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="21416-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="21416-123">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="21416-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="21416-124">内容なし</span><span class="sxs-lookup"><span data-stu-id="21416-124">No Content</span></span> | <span data-ttu-id="21416-125">そのアクティビティに指定された**historyItem**を削除します。</span><span class="sxs-lookup"><span data-stu-id="21416-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="21416-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21416-126">Properties</span></span>

|<span data-ttu-id="21416-127">名前</span><span class="sxs-lookup"><span data-stu-id="21416-127">Name</span></span> | <span data-ttu-id="21416-128">種類</span><span class="sxs-lookup"><span data-stu-id="21416-128">Type</span></span> | <span data-ttu-id="21416-129">説明</span><span class="sxs-lookup"><span data-stu-id="21416-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="21416-130">status</span><span class="sxs-lookup"><span data-stu-id="21416-130">status</span></span> | <span data-ttu-id="21416-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="21416-131">EnumType</span></span> | <span data-ttu-id="21416-132">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="21416-132">Set by the server.</span></span> <span data-ttu-id="21416-133">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="21416-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="21416-134">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="21416-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="21416-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="21416-135">userTimezone</span></span> | <span data-ttu-id="21416-136">String</span><span class="sxs-lookup"><span data-stu-id="21416-136">String</span></span> | <span data-ttu-id="21416-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21416-137">Optional.</span></span> <span data-ttu-id="21416-138">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="21416-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="21416-139">クロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="21416-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="21416-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="21416-140">createdDateTime</span></span> | <span data-ttu-id="21416-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21416-141">DateTimeOffset</span></span> | <span data-ttu-id="21416-142">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="21416-142">Set by the server.</span></span> <span data-ttu-id="21416-143">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="21416-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="21416-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="21416-144">lastModifiedDateTime</span></span> | <span data-ttu-id="21416-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21416-145">DateTimeOffset</span></span> | <span data-ttu-id="21416-146">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="21416-146">Set by the server.</span></span> <span data-ttu-id="21416-147">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="21416-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="21416-148">id</span><span class="sxs-lookup"><span data-stu-id="21416-148">id</span></span> | <span data-ttu-id="21416-149">String</span><span class="sxs-lookup"><span data-stu-id="21416-149">String</span></span> | <span data-ttu-id="21416-150">必須。</span><span class="sxs-lookup"><span data-stu-id="21416-150">Required.</span></span> <span data-ttu-id="21416-151">**HistoryItem**オブジェクトの GUID をクライアントに設定します。</span><span class="sxs-lookup"><span data-stu-id="21416-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="21416-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="21416-152">startedDateTime</span></span> | <span data-ttu-id="21416-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21416-153">DateTimeOffset</span></span> | <span data-ttu-id="21416-154">必須。</span><span class="sxs-lookup"><span data-stu-id="21416-154">Required.</span></span> <span data-ttu-id="21416-155">**HistoryItem** (アクティビティ セッション) が開始されたときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="21416-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="21416-156">タイムラインの履歴が必要です。</span><span class="sxs-lookup"><span data-stu-id="21416-156">Required for timeline history.</span></span>|
|<span data-ttu-id="21416-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="21416-157">lastActiveDateTime</span></span> | <span data-ttu-id="21416-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21416-158">DateTimeOffset</span></span> | <span data-ttu-id="21416-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21416-159">Optional.</span></span> <span data-ttu-id="21416-160">**HistoryItem** (アクティビティ セッション) がアクティブまたは終了の null の場合、 **historyItem**の状態として理解された最後のときの UTC 日時は、継続中にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="21416-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="21416-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21416-161">expirationDateTime</span></span> | <span data-ttu-id="21416-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21416-162">DateTimeOffset</span></span> | <span data-ttu-id="21416-163">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21416-163">Optional.</span></span> <span data-ttu-id="21416-164">**HistoryItem**がハード削除を行うときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="21416-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="21416-165">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="21416-165">Can be set by the client.</span></span>|
|<span data-ttu-id="21416-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="21416-166">activeDurationSeconds</span></span> | <span data-ttu-id="21416-167">int</span><span class="sxs-lookup"><span data-stu-id="21416-167">int</span></span> | <span data-ttu-id="21416-168">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21416-168">Optional.</span></span> <span data-ttu-id="21416-169">アクティブなユーザーの活動の期間です。</span><span class="sxs-lookup"><span data-stu-id="21416-169">The duration of active user engagement.</span></span> <span data-ttu-id="21416-170">指定されなかった場合、この**startedDateTime**と**lastActiveDateTime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="21416-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21416-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21416-171">Relationships</span></span>

|<span data-ttu-id="21416-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21416-172">Relationship</span></span> | <span data-ttu-id="21416-173">型</span><span class="sxs-lookup"><span data-stu-id="21416-173">Type</span></span> | <span data-ttu-id="21416-174">説明</span><span class="sxs-lookup"><span data-stu-id="21416-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="21416-175">activity</span><span class="sxs-lookup"><span data-stu-id="21416-175">activity</span></span>| [<span data-ttu-id="21416-176">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="21416-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="21416-177">省略可能。</span><span class="sxs-lookup"><span data-stu-id="21416-177">Optional.</span></span> <span data-ttu-id="21416-178">受け取りますおよび抑制ソリューションです。ナビゲーション プロパティに関連する活動です。</span><span class="sxs-lookup"><span data-stu-id="21416-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21416-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21416-179">JSON representation</span></span>

<span data-ttu-id="21416-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21416-180">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
