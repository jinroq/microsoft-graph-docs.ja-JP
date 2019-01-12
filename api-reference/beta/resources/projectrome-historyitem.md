---
title: historyItem リソースの種類
description: アプリケーション内のアクティビティの履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 168587aa54446aeee78107deaa9087c6bffb8586
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976955"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="d8d9e-106">historyItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d8d9e-106">historyItem resource type</span></span>

> <span data-ttu-id="d8d9e-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8d9e-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8d9e-109">アプリケーション内の[アクティビティ](projectrome-activity.md)の履歴項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-109">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="d8d9e-110">ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-110">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="d8d9e-111">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-111">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="d8d9e-112">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-112">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="d8d9e-113">アプリケーションは、セッションを作成するときは、ユーザー契約の期間を反映するように**アクティビティ**オブジェクトに**historyItem**オブジェクトを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-113">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="d8d9e-114">ユーザーは、再活動と連携して、たびに、新しい**historyItem**がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-114">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="d8d9e-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8d9e-115">Methods</span></span>

|<span data-ttu-id="d8d9e-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="d8d9e-116">Method</span></span> | <span data-ttu-id="d8d9e-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d8d9e-117">Return Type</span></span> | <span data-ttu-id="d8d9e-118">説明</span><span class="sxs-lookup"><span data-stu-id="d8d9e-118">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="d8d9e-119">作成または置換 historyItem</span><span class="sxs-lookup"><span data-stu-id="d8d9e-119">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="d8d9e-120">historyItem</span><span class="sxs-lookup"><span data-stu-id="d8d9e-120">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="d8d9e-121">作成するか、その活動 (アップサート) の既存の**historyItem**に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-121">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="d8d9e-122">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-122">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="d8d9e-123">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-123">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="d8d9e-124">内容なし</span><span class="sxs-lookup"><span data-stu-id="d8d9e-124">No Content</span></span> | <span data-ttu-id="d8d9e-125">そのアクティビティに指定された**historyItem**を削除します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-125">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8d9e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8d9e-126">Properties</span></span>

|<span data-ttu-id="d8d9e-127">名前</span><span class="sxs-lookup"><span data-stu-id="d8d9e-127">Name</span></span> | <span data-ttu-id="d8d9e-128">型</span><span class="sxs-lookup"><span data-stu-id="d8d9e-128">Type</span></span> | <span data-ttu-id="d8d9e-129">説明</span><span class="sxs-lookup"><span data-stu-id="d8d9e-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d8d9e-130">status</span><span class="sxs-lookup"><span data-stu-id="d8d9e-130">status</span></span> | <span data-ttu-id="d8d9e-131">EnumType</span><span class="sxs-lookup"><span data-stu-id="d8d9e-131">EnumType</span></span> | <span data-ttu-id="d8d9e-132">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-132">Set by the server.</span></span> <span data-ttu-id="d8d9e-133">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-133">A status code used to identify valid objects.</span></span> <span data-ttu-id="d8d9e-134">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-134">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="d8d9e-135">userTimezone</span><span class="sxs-lookup"><span data-stu-id="d8d9e-135">userTimezone</span></span> | <span data-ttu-id="d8d9e-136">String</span><span class="sxs-lookup"><span data-stu-id="d8d9e-136">String</span></span> | <span data-ttu-id="d8d9e-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-137">Optional.</span></span> <span data-ttu-id="d8d9e-138">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-138">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="d8d9e-139">クロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-139">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="d8d9e-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d9e-140">createdDateTime</span></span> | <span data-ttu-id="d8d9e-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d9e-141">DateTimeOffset</span></span> | <span data-ttu-id="d8d9e-142">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-142">Set by the server.</span></span> <span data-ttu-id="d8d9e-143">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-143">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="d8d9e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d9e-144">lastModifiedDateTime</span></span> | <span data-ttu-id="d8d9e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d9e-145">DateTimeOffset</span></span> | <span data-ttu-id="d8d9e-146">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-146">Set by the server.</span></span> <span data-ttu-id="d8d9e-147">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-147">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="d8d9e-148">id</span><span class="sxs-lookup"><span data-stu-id="d8d9e-148">id</span></span> | <span data-ttu-id="d8d9e-149">String</span><span class="sxs-lookup"><span data-stu-id="d8d9e-149">String</span></span> | <span data-ttu-id="d8d9e-150">必須。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-150">Required.</span></span> <span data-ttu-id="d8d9e-151">**HistoryItem**オブジェクトの GUID をクライアントに設定します。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-151">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="d8d9e-152">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d9e-152">startedDateTime</span></span> | <span data-ttu-id="d8d9e-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d9e-153">DateTimeOffset</span></span> | <span data-ttu-id="d8d9e-154">必須。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-154">Required.</span></span> <span data-ttu-id="d8d9e-155">**HistoryItem** (アクティビティ セッション) が開始されたときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-155">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="d8d9e-156">タイムラインの履歴が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-156">Required for timeline history.</span></span>|
|<span data-ttu-id="d8d9e-157">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d9e-157">lastActiveDateTime</span></span> | <span data-ttu-id="d8d9e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d9e-158">DateTimeOffset</span></span> | <span data-ttu-id="d8d9e-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-159">Optional.</span></span> <span data-ttu-id="d8d9e-160">**HistoryItem** (アクティビティ セッション) がアクティブまたは終了の null の場合、 **historyItem**の状態として理解された最後のときの UTC 日時は、継続中にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-160">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="d8d9e-161">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d8d9e-161">expirationDateTime</span></span> | <span data-ttu-id="d8d9e-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8d9e-162">DateTimeOffset</span></span> | <span data-ttu-id="d8d9e-163">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-163">Optional.</span></span> <span data-ttu-id="d8d9e-164">**HistoryItem**がハード削除を行うときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-164">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="d8d9e-165">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-165">Can be set by the client.</span></span>|
|<span data-ttu-id="d8d9e-166">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="d8d9e-166">activeDurationSeconds</span></span> | <span data-ttu-id="d8d9e-167">int</span><span class="sxs-lookup"><span data-stu-id="d8d9e-167">int</span></span> | <span data-ttu-id="d8d9e-168">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-168">Optional.</span></span> <span data-ttu-id="d8d9e-169">アクティブなユーザーの活動の期間です。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-169">The duration of active user engagement.</span></span> <span data-ttu-id="d8d9e-170">指定されなかった場合、この**startedDateTime**と**lastActiveDateTime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-170">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8d9e-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8d9e-171">Relationships</span></span>

|<span data-ttu-id="d8d9e-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d8d9e-172">Relationship</span></span> | <span data-ttu-id="d8d9e-173">型</span><span class="sxs-lookup"><span data-stu-id="d8d9e-173">Type</span></span> | <span data-ttu-id="d8d9e-174">説明</span><span class="sxs-lookup"><span data-stu-id="d8d9e-174">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="d8d9e-175">activity</span><span class="sxs-lookup"><span data-stu-id="d8d9e-175">activity</span></span>| [<span data-ttu-id="d8d9e-176">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="d8d9e-176">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="d8d9e-177">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-177">Optional.</span></span> <span data-ttu-id="d8d9e-178">受け取りますおよび抑制ソリューションです。ナビゲーション プロパティに関連する活動です。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-178">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d8d9e-179">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d8d9e-179">JSON representation</span></span>

<span data-ttu-id="d8d9e-180">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d8d9e-180">Here is a JSON representation of the resource.</span></span>

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
