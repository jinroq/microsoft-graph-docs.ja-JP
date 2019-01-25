---
title: historyItem リソースの種類
description: アプリケーション内のアクティビティの履歴項目を表します。 ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。 ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。 ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 640b2e777337182b95572ba086f1caf3459ef57e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514699"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="fc3b3-106">historyItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc3b3-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc3b3-107">アプリケーション内の[アクティビティ](projectrome-activity.md)の履歴項目を表します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="fc3b3-108">ユーザーのアクティビティでは、アプリのテレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーン内で単一の宛先を表します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="fc3b3-109">ユーザーは、その活動と連携して、ときに、そのアクティビティの開始と終了時刻を示す履歴項目として契約がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="fc3b3-110">ようにユーザーには、再、時間の経過と共にその活動と連携して、1 人のユーザーの活動の複数の項目の履歴が記録されます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="fc3b3-111">アプリケーションは、セッションを作成するときは、ユーザー契約の期間を反映するように**アクティビティ**オブジェクトに**historyItem**オブジェクトを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="fc3b3-112">ユーザーは、再活動と連携して、たびに、新しい**historyItem**がユーザーの活動を見越計上するアクティビティに追加されます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="fc3b3-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc3b3-113">Methods</span></span>

|<span data-ttu-id="fc3b3-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="fc3b3-114">Method</span></span> | <span data-ttu-id="fc3b3-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fc3b3-115">Return Type</span></span> | <span data-ttu-id="fc3b3-116">説明</span><span class="sxs-lookup"><span data-stu-id="fc3b3-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="fc3b3-117">作成または置換 historyItem</span><span class="sxs-lookup"><span data-stu-id="fc3b3-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="fc3b3-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="fc3b3-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="fc3b3-119">作成するか、その活動 (アップサート) の既存の**historyItem**に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="fc3b3-120">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="fc3b3-121">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="fc3b3-122">内容なし</span><span class="sxs-lookup"><span data-stu-id="fc3b3-122">No Content</span></span> | <span data-ttu-id="fc3b3-123">そのアクティビティに指定された**historyItem**を削除します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="fc3b3-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc3b3-124">Properties</span></span>

|<span data-ttu-id="fc3b3-125">名前</span><span class="sxs-lookup"><span data-stu-id="fc3b3-125">Name</span></span> | <span data-ttu-id="fc3b3-126">型</span><span class="sxs-lookup"><span data-stu-id="fc3b3-126">Type</span></span> | <span data-ttu-id="fc3b3-127">説明</span><span class="sxs-lookup"><span data-stu-id="fc3b3-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="fc3b3-128">status</span><span class="sxs-lookup"><span data-stu-id="fc3b3-128">status</span></span> | <span data-ttu-id="fc3b3-129">EnumType</span><span class="sxs-lookup"><span data-stu-id="fc3b3-129">EnumType</span></span> | <span data-ttu-id="fc3b3-130">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-130">Set by the server.</span></span> <span data-ttu-id="fc3b3-131">有効なオブジェクトを識別するために使用する状態コードです。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="fc3b3-132">値: アクティブな場合、更新、削除、無視されます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="fc3b3-133">userTimezone</span><span class="sxs-lookup"><span data-stu-id="fc3b3-133">userTimezone</span></span> | <span data-ttu-id="fc3b3-134">文字列</span><span class="sxs-lookup"><span data-stu-id="fc3b3-134">String</span></span> | <span data-ttu-id="fc3b3-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-135">Optional.</span></span> <span data-ttu-id="fc3b3-136">活動の作成時に配置されましたユーザーのデバイスのアクティビティを生成するために使用するタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="fc3b3-137">クロスプラット フォーム形式をサポートするために、Olson の Id として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="fc3b3-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3b3-138">createdDateTime</span></span> | <span data-ttu-id="fc3b3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3b3-139">DateTimeOffset</span></span> | <span data-ttu-id="fc3b3-140">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-140">Set by the server.</span></span> <span data-ttu-id="fc3b3-141">サーバー上にオブジェクトが作成されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="fc3b3-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3b3-142">lastModifiedDateTime</span></span> | <span data-ttu-id="fc3b3-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3b3-143">DateTimeOffset</span></span> | <span data-ttu-id="fc3b3-144">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-144">Set by the server.</span></span> <span data-ttu-id="fc3b3-145">サーバー上にオブジェクトが変更されたときの utc 日時。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="fc3b3-146">id</span><span class="sxs-lookup"><span data-stu-id="fc3b3-146">id</span></span> | <span data-ttu-id="fc3b3-147">String</span><span class="sxs-lookup"><span data-stu-id="fc3b3-147">String</span></span> | <span data-ttu-id="fc3b3-148">必須。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-148">Required.</span></span> <span data-ttu-id="fc3b3-149">**HistoryItem**オブジェクトの GUID をクライアントに設定します。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="fc3b3-150">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3b3-150">startedDateTime</span></span> | <span data-ttu-id="fc3b3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3b3-151">DateTimeOffset</span></span> | <span data-ttu-id="fc3b3-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-152">Required.</span></span> <span data-ttu-id="fc3b3-153">**HistoryItem** (アクティビティ セッション) が開始されたときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="fc3b3-154">タイムラインの履歴が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-154">Required for timeline history.</span></span>|
|<span data-ttu-id="fc3b3-155">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3b3-155">lastActiveDateTime</span></span> | <span data-ttu-id="fc3b3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3b3-156">DateTimeOffset</span></span> | <span data-ttu-id="fc3b3-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-157">Optional.</span></span> <span data-ttu-id="fc3b3-158">**HistoryItem** (アクティビティ セッション) がアクティブまたは終了の null の場合、 **historyItem**の状態として理解された最後のときの UTC 日時は、継続中にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="fc3b3-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fc3b3-159">expirationDateTime</span></span> | <span data-ttu-id="fc3b3-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc3b3-160">DateTimeOffset</span></span> | <span data-ttu-id="fc3b3-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-161">Optional.</span></span> <span data-ttu-id="fc3b3-162">**HistoryItem**がハード削除を行うときの UTC 日時。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="fc3b3-163">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-163">Can be set by the client.</span></span>|
|<span data-ttu-id="fc3b3-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="fc3b3-164">activeDurationSeconds</span></span> | <span data-ttu-id="fc3b3-165">int</span><span class="sxs-lookup"><span data-stu-id="fc3b3-165">int</span></span> | <span data-ttu-id="fc3b3-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-166">Optional.</span></span> <span data-ttu-id="fc3b3-167">アクティブなユーザーの活動の期間です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-167">The duration of active user engagement.</span></span> <span data-ttu-id="fc3b3-168">指定されなかった場合、この**startedDateTime**と**lastActiveDateTime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc3b3-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc3b3-169">Relationships</span></span>

|<span data-ttu-id="fc3b3-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc3b3-170">Relationship</span></span> | <span data-ttu-id="fc3b3-171">型</span><span class="sxs-lookup"><span data-stu-id="fc3b3-171">Type</span></span> | <span data-ttu-id="fc3b3-172">説明</span><span class="sxs-lookup"><span data-stu-id="fc3b3-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="fc3b3-173">activity</span><span class="sxs-lookup"><span data-stu-id="fc3b3-173">activity</span></span>| [<span data-ttu-id="fc3b3-174">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="fc3b3-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="fc3b3-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-175">Optional.</span></span> <span data-ttu-id="fc3b3-176">受け取りますおよび抑制ソリューションです。ナビゲーション プロパティに関連する活動です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc3b3-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc3b3-177">JSON representation</span></span>

<span data-ttu-id="fc3b3-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc3b3-178">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/projectrome-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
