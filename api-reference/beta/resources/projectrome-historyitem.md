---
title: 履歴項目リソースの種類
description: アプリ内のアクティビティの履歴アイテムを表します。 ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。 ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。 ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: c43a4f0515f8d61625e11abe8bbdbe2464c729f9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344081"
---
# <a name="historyitem-resource-type"></a><span data-ttu-id="d6bbf-106">履歴項目リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d6bbf-106">historyItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6bbf-107">アプリ内の[アクティビティ](projectrome-activity.md)の履歴アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-107">Represents a history item for an [activity](projectrome-activity.md) in an app.</span></span> <span data-ttu-id="d6bbf-108">ユーザーアクティビティは、テレビ番組、ドキュメント、ビデオゲームの現在のキャンペーンなど、アプリ内の単一の場所を表します。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-108">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="d6bbf-109">ユーザーがそのアクティビティを使用すると、そのアクティビティの開始時刻と終了時刻を示す履歴項目として契約が取得されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-109">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="d6bbf-110">ユーザーが時間をかけてそのアクティビティを再実行すると、1つのユーザーアクティビティに対して複数の履歴項目が記録されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-110">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="d6bbf-111">アプリでセッションを作成するときには、ユーザーの活動期間を反映するために、**履歴項目**オブジェクトを**activity**オブジェクトに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-111">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="d6bbf-112">ユーザーがアクティビティを再実行するたびに、新しい**履歴アイテム**が、[見越計上] ユーザー契約に追加されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-112">Each time a user re-engages with an activity, a new **historyItem** is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="d6bbf-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6bbf-113">Methods</span></span>

|<span data-ttu-id="d6bbf-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="d6bbf-114">Method</span></span> | <span data-ttu-id="d6bbf-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d6bbf-115">Return Type</span></span> | <span data-ttu-id="d6bbf-116">説明</span><span class="sxs-lookup"><span data-stu-id="d6bbf-116">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="d6bbf-117">履歴項目を作成または置換する</span><span class="sxs-lookup"><span data-stu-id="d6bbf-117">Create or replace historyItem</span></span>](../api/projectrome-put-historyitem.md) | [<span data-ttu-id="d6bbf-118">historyItem</span><span class="sxs-lookup"><span data-stu-id="d6bbf-118">historyItem</span></span>](projectrome-historyitem.md) | <span data-ttu-id="d6bbf-119">そのアクティビティの既存の**履歴アイテム**を作成または置換します (upsert)。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-119">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="d6bbf-120">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-120">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="d6bbf-121">履歴項目を削除する</span><span class="sxs-lookup"><span data-stu-id="d6bbf-121">Delete a historyItem</span></span>](../api/projectrome-delete-historyitem.md) | <span data-ttu-id="d6bbf-122">No Content</span><span class="sxs-lookup"><span data-stu-id="d6bbf-122">No Content</span></span> | <span data-ttu-id="d6bbf-123">そのアクティビティの指定した**履歴アイテム**を削除します。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-123">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="d6bbf-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d6bbf-124">Properties</span></span>

|<span data-ttu-id="d6bbf-125">名前</span><span class="sxs-lookup"><span data-stu-id="d6bbf-125">Name</span></span> | <span data-ttu-id="d6bbf-126">型</span><span class="sxs-lookup"><span data-stu-id="d6bbf-126">Type</span></span> | <span data-ttu-id="d6bbf-127">説明</span><span class="sxs-lookup"><span data-stu-id="d6bbf-127">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d6bbf-128">status</span><span class="sxs-lookup"><span data-stu-id="d6bbf-128">status</span></span> | <span data-ttu-id="d6bbf-129">string</span><span class="sxs-lookup"><span data-stu-id="d6bbf-129">string</span></span> | <span data-ttu-id="d6bbf-130">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-130">Set by the server.</span></span> <span data-ttu-id="d6bbf-131">有効なオブジェクトを識別するために使用される状態コード。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-131">A status code used to identify valid objects.</span></span> <span data-ttu-id="d6bbf-132">値: アクティブ、更新済み、削除済み、無視。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-132">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="d6bbf-133">usertimezone</span><span class="sxs-lookup"><span data-stu-id="d6bbf-133">userTimezone</span></span> | <span data-ttu-id="d6bbf-134">String</span><span class="sxs-lookup"><span data-stu-id="d6bbf-134">String</span></span> | <span data-ttu-id="d6bbf-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-135">Optional.</span></span> <span data-ttu-id="d6bbf-136">アクティビティの生成に使用されたユーザーのデバイスがアクティビティの作成時に配置されたタイムゾーン。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-136">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="d6bbf-137">クロスプラットフォーム表現をサポートするために olson id として提供される値。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-137">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="d6bbf-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6bbf-138">createdDateTime</span></span> | <span data-ttu-id="d6bbf-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bbf-139">DateTimeOffset</span></span> | <span data-ttu-id="d6bbf-140">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-140">Set by the server.</span></span> <span data-ttu-id="d6bbf-141">サーバー上でオブジェクトが作成された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-141">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="d6bbf-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6bbf-142">lastModifiedDateTime</span></span> | <span data-ttu-id="d6bbf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bbf-143">DateTimeOffset</span></span> | <span data-ttu-id="d6bbf-144">サーバーによって設定されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-144">Set by the server.</span></span> <span data-ttu-id="d6bbf-145">サーバー上のオブジェクトが変更された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-145">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="d6bbf-146">id</span><span class="sxs-lookup"><span data-stu-id="d6bbf-146">id</span></span> | <span data-ttu-id="d6bbf-147">String</span><span class="sxs-lookup"><span data-stu-id="d6bbf-147">String</span></span> | <span data-ttu-id="d6bbf-148">必須。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-148">Required.</span></span> <span data-ttu-id="d6bbf-149">**履歴項目**オブジェクトのクライアントセット GUID。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-149">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="d6bbf-150">開始日時</span><span class="sxs-lookup"><span data-stu-id="d6bbf-150">startedDateTime</span></span> | <span data-ttu-id="d6bbf-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bbf-151">DateTimeOffset</span></span> | <span data-ttu-id="d6bbf-152">必須です。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-152">Required.</span></span> <span data-ttu-id="d6bbf-153">**履歴アイテム**(アクティビティセッション) が開始された UTC の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-153">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="d6bbf-154">タイムライン履歴に必要です。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-154">Required for timeline history.</span></span>|
|<span data-ttu-id="d6bbf-155">lastactivedatetime</span><span class="sxs-lookup"><span data-stu-id="d6bbf-155">lastActiveDateTime</span></span> | <span data-ttu-id="d6bbf-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bbf-156">DateTimeOffset</span></span> | <span data-ttu-id="d6bbf-157">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-157">Optional.</span></span> <span data-ttu-id="d6bbf-158">**履歴項目**(アクティビティセッション) が最後にアクティブまたは完了として認識された UTC の DateTime。 null の場合は、**履歴アイテム**の状態が進行中である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-158">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="d6bbf-159">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d6bbf-159">expirationDateTime</span></span> | <span data-ttu-id="d6bbf-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bbf-160">DateTimeOffset</span></span> | <span data-ttu-id="d6bbf-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-161">Optional.</span></span> <span data-ttu-id="d6bbf-162">**履歴アイテム**がハード削除されるときの UTC DateTime。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-162">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="d6bbf-163">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-163">Can be set by the client.</span></span>|
|<span data-ttu-id="d6bbf-164">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="d6bbf-164">activeDurationSeconds</span></span> | <span data-ttu-id="d6bbf-165">int</span><span class="sxs-lookup"><span data-stu-id="d6bbf-165">int</span></span> | <span data-ttu-id="d6bbf-166">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-166">Optional.</span></span> <span data-ttu-id="d6bbf-167">アクティブなユーザー契約の期間。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-167">The duration of active user engagement.</span></span> <span data-ttu-id="d6bbf-168">指定しない場合、これは開始日\*\*\*\* と**lastactivedatetime**から計算されます。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-168">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6bbf-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6bbf-169">Relationships</span></span>

|<span data-ttu-id="d6bbf-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d6bbf-170">Relationship</span></span> | <span data-ttu-id="d6bbf-171">型</span><span class="sxs-lookup"><span data-stu-id="d6bbf-171">Type</span></span> | <span data-ttu-id="d6bbf-172">説明</span><span class="sxs-lookup"><span data-stu-id="d6bbf-172">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="d6bbf-173">activity</span><span class="sxs-lookup"><span data-stu-id="d6bbf-173">activity</span></span>| [<span data-ttu-id="d6bbf-174">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="d6bbf-174">activity</span></span>](../resources/projectrome-activity.md) | <span data-ttu-id="d6bbf-175">省略可能。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-175">Optional.</span></span> <span data-ttu-id="d6bbf-176">NavigationProperty/コンテインメント;関連付けられたアクティビティへのナビゲーションプロパティ。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-176">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d6bbf-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d6bbf-177">JSON representation</span></span>

<span data-ttu-id="d6bbf-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d6bbf-178">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "keyProperty": "id",
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
  "suppressions": []
}
-->
