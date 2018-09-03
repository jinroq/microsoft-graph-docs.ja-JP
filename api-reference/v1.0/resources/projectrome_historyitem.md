# <a name="historyitem-resource-type"></a><span data-ttu-id="4ab6f-101">historyItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ab6f-101">historyItem resource type</span></span>

<span data-ttu-id="4ab6f-102">アプリ内の [アクティビティ](projectrome_activity.md) の履歴項目を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-102">Represents a history item for an [activity](projectrome_activity.md) in an app.</span></span> <span data-ttu-id="4ab6f-103">ユーザーのアクティビティは、アプリ内の単一の宛先 (たとえば、テレビ番組、ドキュメント、またはビデオ ゲームの現在のキャンペーンなど) を表します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-103">User activities represent a single destination within your app - for example, a TV show, a document, or a current campaign in a video game.</span></span> <span data-ttu-id="4ab6f-104">ユーザーがそのアクティビティを行っている場合、そのアクティビティの開始時刻と終了時刻を示す履歴項目としてユーザーの動作がキャプチャされます。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-104">When a user engages with that activity, the engagement is captured as a history item that indicates the start and end time for that activity.</span></span> <span data-ttu-id="4ab6f-105">時間が経過してユーザーがそのアクティビティを再度行うと、複数の履歴項目が 1 人のユーザーのアクティビティに対して記録されます。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-105">As the user re-engages with that activity over time, multiple history items are recorded for a single user activity.</span></span>

<span data-ttu-id="4ab6f-106">アプリがセッションを作成する場合は、**historyItem** オブジェクトを **activity** オブジェクトに追加して、ユーザーの動作期間を反映する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-106">When an app creates a session, a **historyItem** object should be added to the **activity** object to reflect the period of user engagement.</span></span> <span data-ttu-id="4ab6f-107">ユーザーがアクティビティを再度行うごとに、新しい **historyItem** が追加され、ユーザーの動作が蓄積されます。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-107">Each time a user reengages with an activity, a new history item is added to the activity to accrue user engagement.</span></span>

## <a name="methods"></a><span data-ttu-id="4ab6f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ab6f-108">Methods</span></span>

|<span data-ttu-id="4ab6f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4ab6f-109">Method</span></span> | <span data-ttu-id="4ab6f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4ab6f-110">Return Type</span></span> | <span data-ttu-id="4ab6f-111">説明</span><span class="sxs-lookup"><span data-stu-id="4ab6f-111">Description</span></span>|
|:------|:------------|:-----------|
|[<span data-ttu-id="4ab6f-112">Create or replace historyItem</span><span class="sxs-lookup"><span data-stu-id="4ab6f-112">Create or replace historyItem</span></span>](../api/projectrome_put_historyitem.md) | <span data-ttu-id="4ab6f-113">[historyItem](projectrome_historyitem.md)</span><span class="sxs-lookup"><span data-stu-id="4ab6f-113">Added [historyItem](projectrome_historyitem.md)</span></span> | <span data-ttu-id="4ab6f-114">その動作の既存の **historyItem** を作成または置換します (UPSERT)。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-114">Creates or replaces an existing **historyItem** for that activity (upsert).</span></span> <span data-ttu-id="4ab6f-115">ID は GUID である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-115">The ID needs to be a GUID.</span></span>|
|[<span data-ttu-id="4ab6f-116">Delete a historyItem</span><span class="sxs-lookup"><span data-stu-id="4ab6f-116">Delete a historyItem</span></span>](../api/projectrome_delete_historyitem.md) | <span data-ttu-id="4ab6f-117">コンテンツなし</span><span class="sxs-lookup"><span data-stu-id="4ab6f-117">No Content</span></span> | <span data-ttu-id="4ab6f-118">そのアクティビティに指定された **historyItem** を削除します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-118">Deletes the specified **historyItem** for that activity.</span></span>|

## <a name="properties"></a><span data-ttu-id="4ab6f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ab6f-119">Properties</span></span>

|<span data-ttu-id="4ab6f-120">名前</span><span class="sxs-lookup"><span data-stu-id="4ab6f-120">Name</span></span> | <span data-ttu-id="4ab6f-121">型</span><span class="sxs-lookup"><span data-stu-id="4ab6f-121">Type</span></span> | <span data-ttu-id="4ab6f-122">説明</span><span class="sxs-lookup"><span data-stu-id="4ab6f-122">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4ab6f-123">status</span><span class="sxs-lookup"><span data-stu-id="4ab6f-123">status</span></span> | <span data-ttu-id="4ab6f-124">status</span><span class="sxs-lookup"><span data-stu-id="4ab6f-124">status</span></span> | <span data-ttu-id="4ab6f-125">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-125">Provided by the server.</span></span> <span data-ttu-id="4ab6f-126">有効なオブジェクトを識別するために使用するステータス コードです。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-126">A status code used to identify valid objects.</span></span> <span data-ttu-id="4ab6f-127">値は、 active、updated、deleted、ignored です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-127">Values: active, updated, deleted, ignored.</span></span>|
|<span data-ttu-id="4ab6f-128">userTimezone</span><span class="sxs-lookup"><span data-stu-id="4ab6f-128">userTimezone</span></span> | <span data-ttu-id="4ab6f-129">String</span><span class="sxs-lookup"><span data-stu-id="4ab6f-129">String</span></span> | <span data-ttu-id="4ab6f-130">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-130">Optional.</span></span> <span data-ttu-id="4ab6f-131">アクティビティを生成するために使用されたユーザーのデバイスが、アクティビティ作成時に存在していた場所のタイム ゾーンです。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-131">The timezone in which the user's device used to generate the activity was located at activity creation time.</span></span> <span data-ttu-id="4ab6f-132">クロス プラットフォームの表示をサポートするために、Olson の ID として指定された値です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-132">Values supplied as Olson IDs in order to support cross-platform representation.</span></span>|
|<span data-ttu-id="4ab6f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6f-133">createdDateTime</span></span> | <span data-ttu-id="4ab6f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab6f-134">DateTimeOffset</span></span> | <span data-ttu-id="4ab6f-135">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-135">Provided by the server.</span></span> <span data-ttu-id="4ab6f-136">サーバー上でオブジェクトが作成されたときの UTC の DateTime です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-136">DateTime in UTC when the object was created on the server.</span></span>|
|<span data-ttu-id="4ab6f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6f-137">lastModifiedDateTime</span></span> | <span data-ttu-id="4ab6f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab6f-138">DateTimeOffset</span></span> | <span data-ttu-id="4ab6f-139">サーバーで設定します。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-139">Provided by the server.</span></span> <span data-ttu-id="4ab6f-140">サーバー上でオブジェクトが変更されたときの UTC の DateTime です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-140">DateTime in UTC when the object was modified on the server.</span></span>|
|<span data-ttu-id="4ab6f-141">id</span><span class="sxs-lookup"><span data-stu-id="4ab6f-141">id</span></span> | <span data-ttu-id="4ab6f-142">文字列</span><span class="sxs-lookup"><span data-stu-id="4ab6f-142">String</span></span> | <span data-ttu-id="4ab6f-143">必須。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-143">Required.</span></span> <span data-ttu-id="4ab6f-144"> **HistoryItem** オブジェクトのクライアント設定の GUID です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-144">Client-set GUID for the **historyItem** object.</span></span>|
|<span data-ttu-id="4ab6f-145">startedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6f-145">startedDateTime</span></span> | <span data-ttu-id="4ab6f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab6f-146">DateTimeOffset</span></span> | <span data-ttu-id="4ab6f-147">必須。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-147">Required.</span></span> <span data-ttu-id="4ab6f-148"> **historyItem** (アクティビティ セッション) が開始されたときの UTC DateTime です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-148">UTC DateTime when the **historyItem** (activity session) was started.</span></span> <span data-ttu-id="4ab6f-149">タイムラインの履歴に必要です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-149">Required for timeline history.</span></span>|
|<span data-ttu-id="4ab6f-150">lastActiveDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6f-150">lastActiveDateTime</span></span> | <span data-ttu-id="4ab6f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab6f-151">DateTimeOffset</span></span> | <span data-ttu-id="4ab6f-152">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-152">Optional.</span></span> <span data-ttu-id="4ab6f-153">**historyItem** (アクティビティ セッション) が最後にアクティブ状態または終了状態と理解されたときの UTC DateTime です。null の場合は、**historyItem** は Ongoing の状態である必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-153">UTC DateTime when the **historyItem** (activity session) was last understood as active or finished - if null, **historyItem** status should be Ongoing.</span></span>|
|<span data-ttu-id="4ab6f-154">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4ab6f-154">expirationDateTime</span></span> | <span data-ttu-id="4ab6f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ab6f-155">DateTimeOffset</span></span> | <span data-ttu-id="4ab6f-156">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-156">Optional.</span></span> <span data-ttu-id="4ab6f-157"> **HistoryItem** が物理削除されるときの UTC DateTime です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-157">UTC DateTime when the **historyItem** will undergo hard-delete.</span></span> <span data-ttu-id="4ab6f-158">クライアントによって設定できます。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-158">Can be set by the client.</span></span>|
|<span data-ttu-id="4ab6f-159">activeDurationSeconds</span><span class="sxs-lookup"><span data-stu-id="4ab6f-159">activeDurationSeconds</span></span> | <span data-ttu-id="4ab6f-160">int</span><span class="sxs-lookup"><span data-stu-id="4ab6f-160">int</span></span> | <span data-ttu-id="4ab6f-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-161">Optional.</span></span> <span data-ttu-id="4ab6f-162">アクティブ ユーザーの動作期間です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-162">The duration of active user engagement.</span></span> <span data-ttu-id="4ab6f-163">指定されなかった場合、**startedDateTime** と **lastActiveDateTime** から計算されます。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-163">if not supplied, this is calculated from the **startedDateTime** and **lastActiveDateTime**.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ab6f-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ab6f-164">Relationships</span></span>

|<span data-ttu-id="4ab6f-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4ab6f-165">Relationship</span></span> | <span data-ttu-id="4ab6f-166">型</span><span class="sxs-lookup"><span data-stu-id="4ab6f-166">Type</span></span> | <span data-ttu-id="4ab6f-167">説明</span><span class="sxs-lookup"><span data-stu-id="4ab6f-167">Description</span></span>|
|:------------|:-----|:-----------|
|<span data-ttu-id="4ab6f-168">activity</span><span class="sxs-lookup"><span data-stu-id="4ab6f-168">activity</span></span>| [<span data-ttu-id="4ab6f-169">userActivity</span><span class="sxs-lookup"><span data-stu-id="4ab6f-169">userActivity</span></span>](../resources/projectrome_activity.md) | <span data-ttu-id="4ab6f-170">省略可能。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-170">Optional.</span></span> <span data-ttu-id="4ab6f-171">NavigationProperty/Containment; 関連するアクティビティのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-171">NavigationProperty/Containment; navigation property to the associated activity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ab6f-172">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ab6f-172">JSON representation</span></span>

<span data-ttu-id="4ab6f-173">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ab6f-173">Here is a JSON representation of the resource.</span></span>

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
