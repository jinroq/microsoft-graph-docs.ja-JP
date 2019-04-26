---
title: 履歴項目リソースの種類
description: アプリ内のアクティビティの履歴アイテムを表します。 ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 640b2e777337182b95572ba086f1caf3459ef57e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563302"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="504e2-106">履歴項目リソースの種類</span><span class="sxs-lookup"><span data-stu-id="504e2-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="504e2-107">アプリ内の[アクティビティ](projectrome-activity.md)の履歴アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="504e2-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="504e2-108">ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="504e2-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="504e2-109">ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="504e2-110">ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="504e2-111">アプリでセッションを作成するときには、ユーザーの活動期間を反映するために、**履歴項目**オブジェクトを**activity**オブジェクトに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="504e2-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="504e2-112">ユーザーがアクティビティを再実行するたびに、新しい**履歴アイテム**が、[見越計上] ユーザー契約に追加されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="504e2-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="504e2-113">Methods</span></span>

|<span data-ttu-id="504e2-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="504e2-114">Method</span></span> | <span data-ttu-id="504e2-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="504e2-115">Return Type</span></span> | <span data-ttu-id="504e2-116">説明</span><span class="sxs-lookup"><span data-stu-id="504e2-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="504e2-117">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="504e2-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="504e2-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="504e2-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="504e2-119">そのアクティビティの既存の**履歴アイテム**を作成または置換します (upsert)。</span><span class="sxs-lookup"><span data-stu-id="504e2-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="504e2-120">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="504e2-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="504e2-121">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="504e2-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="504e2-122">No Content</span><span class="sxs-lookup"><span data-stu-id="504e2-122">No Content</span></span> | <span data-ttu-id="504e2-123">そのアクティビティの指定した**履歴アイテム**を削除します。</span><span class="sxs-lookup"><span data-stu-id="504e2-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="504e2-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="504e2-124">Properties</span></span>

|<span data-ttu-id="504e2-125">名前</span><span class="sxs-lookup"><span data-stu-id="504e2-125">Name</span></span> | <span data-ttu-id="504e2-126">型</span><span class="sxs-lookup"><span data-stu-id="504e2-126">Type</span></span> | <span data-ttu-id="504e2-127">説明</span><span class="sxs-lookup"><span data-stu-id="504e2-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="504e2-128">status</span><span class="sxs-lookup"><span data-stu-id="504e2-128">status</span></span> | <span data-ttu-id="504e2-129">EnumType</span><span class="sxs-lookup"><span data-stu-id="504e2-129">EnumType</span></span> | <span data-ttu-id="504e2-130">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-130">Set by the server.</span></span> <span data-ttu-id="504e2-131">有効なオブジェクトを識別するために使用される状態コード。</span><span class="sxs-lookup"><span data-stu-id="504e2-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="504e2-132">値: アクティブ、更新済み、削除済み、無視。</span><span class="sxs-lookup"><span data-stu-id="504e2-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="504e2-133">usertimezone</span><span class="sxs-lookup"><span data-stu-id="504e2-133">userTimezone</span></span> | <span data-ttu-id="504e2-134">String</span><span class="sxs-lookup"><span data-stu-id="504e2-134">String</span></span> | <span data-ttu-id="504e2-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="504e2-135">Optional.</span></span> <span data-ttu-id="504e2-136">アクティビティの生成に使用されたユーザーのデバイスがアクティビティの作成時に配置されたタイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="504e2-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="504e2-137">クロスプラットフォーム表現をサポートするために olson id として提供される値。</span><span class="sxs-lookup"><span data-stu-id="504e2-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="504e2-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="504e2-138">createdDateTime</span></span> | <span data-ttu-id="504e2-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504e2-139">DateTimeOffset</span></span> | <span data-ttu-id="504e2-140">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-140">Set by the server.</span></span> <span data-ttu-id="504e2-141">サーバー上でオブジェクトが作成された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="504e2-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="504e2-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="504e2-142">lastModifiedDateTime</span></span> | <span data-ttu-id="504e2-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504e2-143">DateTimeOffset</span></span> | <span data-ttu-id="504e2-144">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-144">Set by the server.</span></span> <span data-ttu-id="504e2-145">サーバー上のオブジェクトが変更された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="504e2-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="504e2-146">id</span><span class="sxs-lookup"><span data-stu-id="504e2-146">id</span></span> | <span data-ttu-id="504e2-147">String</span><span class="sxs-lookup"><span data-stu-id="504e2-147">String</span></span> | <span data-ttu-id="504e2-148">必須。</span><span class="sxs-lookup"><span data-stu-id="504e2-148">Required.</span></span> <span data-ttu-id="504e2-149">**履歴項目**オブジェクトのクライアントセット GUID。</span><span class="sxs-lookup"><span data-stu-id="504e2-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="504e2-150">開始日時</span><span class="sxs-lookup"><span data-stu-id="504e2-150">startedDateTime</span></span> | <span data-ttu-id="504e2-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504e2-151">DateTimeOffset</span></span> | <span data-ttu-id="504e2-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="504e2-152">Required.</span></span> <span data-ttu-id="504e2-153">**履歴アイテム**(アクティビティセッション) が開始された UTC の DateTime。</span><span class="sxs-lookup"><span data-stu-id="504e2-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="504e2-154">タイムライン履歴に必要です。</span><span class="sxs-lookup"><span data-stu-id="504e2-154">Required for timeline history.</span></span>|
|<span data-ttu-id="504e2-155">lastactivedatetime</span><span class="sxs-lookup"><span data-stu-id="504e2-155">lastActiveDateTime</span></span> | <span data-ttu-id="504e2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504e2-156">DateTimeOffset</span></span> | <span data-ttu-id="504e2-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="504e2-157">Optional.</span></span> <span data-ttu-id="504e2-158">**履歴項目**(アクティビティセッション) が最後にアクティブまたは完了として認識された UTC の DateTime。 null の場合は、**履歴アイテム**の状態が進行中である必要があります。</span><span class="sxs-lookup"><span data-stu-id="504e2-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="504e2-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="504e2-159">expirationDateTime</span></span> | <span data-ttu-id="504e2-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="504e2-160">DateTimeOffset</span></span> | <span data-ttu-id="504e2-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="504e2-161">Optional.</span></span> <span data-ttu-id="504e2-162">**履歴アイテム**がハード削除されるときの UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="504e2-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="504e2-163">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="504e2-163">Can be set by the client.</span></span>|
|<span data-ttu-id="504e2-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="504e2-164">activeDurationSeconds</span></span> | <span data-ttu-id="504e2-165">int</span><span class="sxs-lookup"><span data-stu-id="504e2-165">int</span></span> | <span data-ttu-id="504e2-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="504e2-166">Optional.</span></span> <span data-ttu-id="504e2-167">アクティブなユーザー契約の期間。</span><span class="sxs-lookup"><span data-stu-id="504e2-167">The duration of active user engagement.</span></span> <span data-ttu-id="504e2-168">指定しない場合、これは開始日\*\*\*\* と**lastactivedatetime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="504e2-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="504e2-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="504e2-169">Relationships</span></span>

|<span data-ttu-id="504e2-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="504e2-170">Relationship</span></span> | <span data-ttu-id="504e2-171">型</span><span class="sxs-lookup"><span data-stu-id="504e2-171">Type</span></span> | <span data-ttu-id="504e2-172">説明</span><span class="sxs-lookup"><span data-stu-id="504e2-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="504e2-173">activity</span><span class="sxs-lookup"><span data-stu-id="504e2-173">activity</span></span>| [<span data-ttu-id="504e2-174">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="504e2-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="504e2-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="504e2-175">Optional.</span></span> <span data-ttu-id="504e2-176">NavigationProperty/コンテインメント;関連付けられたアクティビティへのナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="504e2-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="504e2-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="504e2-177">JSON representation</span></span>

<span data-ttu-id="504e2-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="504e2-178">Here is a JSON representation of the resource.</span></span>

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
