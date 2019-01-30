# <a name="datapolicyoperation-resource-type"></a><span data-ttu-id="cc634-101">dataPolicyOperation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc634-101">dataPolicyOperation resource type</span></span>

<span data-ttu-id="cc634-102">送信されたデータ ポリシー操作を表します。</span><span class="sxs-lookup"><span data-stu-id="cc634-102">Represents a submitted data policy operation.</span></span> <span data-ttu-id="cc634-103">操作のステータスを追跡するために必要な情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc634-103">It contains necessary information for tracking the status of an operation.</span></span> <span data-ttu-id="cc634-104">など、企業の管理者は、従業員の会社のデータをエクスポートするのにはデータのポリシーの操作要求を送信し、その要求を後で追跡できます。</span><span class="sxs-lookup"><span data-stu-id="cc634-104">For example, a company administrator can submit a data policy operation request to export an employee's company data, and then later track that request.</span></span>

## <a name="methods"></a><span data-ttu-id="cc634-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc634-105">Methods</span></span>

| <span data-ttu-id="cc634-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc634-106">Method</span></span>           | <span data-ttu-id="cc634-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc634-107">Return Type</span></span>    |<span data-ttu-id="cc634-108">説明</span><span class="sxs-lookup"><span data-stu-id="cc634-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cc634-109">DataPolicyOperation を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc634-109">Get dataPolicyOperation</span></span>](../api/datapolicyoperation-get.md) | [<span data-ttu-id="cc634-110">dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="cc634-110">dataPolicyOperation</span></span>](datapolicyoperation.md) |<span data-ttu-id="cc634-111">**DataPolicyOperation**オブジェクトのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="cc634-111">Retrieve properties of the **dataPolicyOperation** object.</span></span>|
|[<span data-ttu-id="cc634-112">個人データをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="cc634-112">Export personal data</span></span>](../api/user-exportpersonaldata.md) | <span data-ttu-id="cc634-113">なし</span><span class="sxs-lookup"><span data-stu-id="cc634-113">None</span></span> |<span data-ttu-id="cc634-114">[DataPolicyOperation の取得](../api/datapolicyoperation-get.md)を使用して後で読み取ることができますが、組織のユーザーのデータをエクスポートするのには、データ ポリシーの操作要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="cc634-114">Submit a data policy operation request to export organizational user's data which can later be read using [Get dataPolicyOperation](../api/datapolicyoperation-get.md)</span></span>|

## <a name="properties"></a><span data-ttu-id="cc634-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc634-115">Properties</span></span>

> <span data-ttu-id="cc634-116">**注:** このリソースのすべてのプロパティは、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cc634-116">**Note:** All properties of this resource are read-only.</span></span>

| <span data-ttu-id="cc634-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc634-117">Property</span></span>     | <span data-ttu-id="cc634-118">型</span><span class="sxs-lookup"><span data-stu-id="cc634-118">Type</span></span>   |<span data-ttu-id="cc634-119">説明</span><span class="sxs-lookup"><span data-stu-id="cc634-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc634-120">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc634-120">completedDateTime</span></span>|<span data-ttu-id="cc634-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc634-121">DateTimeOffset</span></span>|<span data-ttu-id="cc634-122">このデータ ポリシーの操作の要求が完了すると、UTC 時刻での ISO 8601 形式を使用して表します。</span><span class="sxs-lookup"><span data-stu-id="cc634-122">Represents when the request for this data policy operation was completed, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="cc634-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="cc634-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="cc634-124">操作が完了するまで null になります。</span><span class="sxs-lookup"><span data-stu-id="cc634-124">Null until the operation completes.</span></span>|
|<span data-ttu-id="cc634-125">id</span><span class="sxs-lookup"><span data-stu-id="cc634-125">id</span></span>|<span data-ttu-id="cc634-126">String</span><span class="sxs-lookup"><span data-stu-id="cc634-126">String</span></span>| <span data-ttu-id="cc634-127">この操作に固有のキーです。</span><span class="sxs-lookup"><span data-stu-id="cc634-127">Unique key for this operation.</span></span> |
|<span data-ttu-id="cc634-128">status</span><span class="sxs-lookup"><span data-stu-id="cc634-128">status</span></span>|<span data-ttu-id="cc634-129">string</span><span class="sxs-lookup"><span data-stu-id="cc634-129">string</span></span>| <span data-ttu-id="cc634-130">可能な値は、`notStarted`、`running`、`complete`、`failed`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="cc634-130">Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="cc634-131">storageLocation</span><span class="sxs-lookup"><span data-stu-id="cc634-131">storageLocation</span></span>|<span data-ttu-id="cc634-132">String</span><span class="sxs-lookup"><span data-stu-id="cc634-132">String</span></span>|<span data-ttu-id="cc634-133">URL の場所のデータをエクスポートするのには、要求をエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="cc634-133">The URL location to where data is being exported for export requests.</span></span>|
|<span data-ttu-id="cc634-134">userId</span><span class="sxs-lookup"><span data-stu-id="cc634-134">userId</span></span>|<span data-ttu-id="cc634-135">String</span><span class="sxs-lookup"><span data-stu-id="cc634-135">String</span></span>|<span data-ttu-id="cc634-136">操作を実行するユーザーのユーザーの id。</span><span class="sxs-lookup"><span data-stu-id="cc634-136">The id for the user on whom the operation is performed.</span></span>|
|<span data-ttu-id="cc634-137">submittedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc634-137">submittedDateTime</span></span>|<span data-ttu-id="cc634-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc634-138">DateTimeOffset</span></span>|<span data-ttu-id="cc634-139">このデータの操作の要求が送信された UTC 時刻での ISO 8601 形式を使用する場合を表します。</span><span class="sxs-lookup"><span data-stu-id="cc634-139">Represents when the request for this data operation was submitted, in UTC time, using the ISO 8601 format.</span></span> <span data-ttu-id="cc634-140">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cc634-140">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cc634-141">進行状況</span><span class="sxs-lookup"><span data-stu-id="cc634-141">progress</span></span>|<span data-ttu-id="cc634-142">String</span><span class="sxs-lookup"><span data-stu-id="cc634-142">String</span></span>|<span data-ttu-id="cc634-143">操作の進行状況を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc634-143">Specifies the progress of an operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc634-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc634-144">Relationships</span></span>
<span data-ttu-id="cc634-145">なし。</span><span class="sxs-lookup"><span data-stu-id="cc634-145">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="cc634-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc634-146">JSON representation</span></span>

<span data-ttu-id="cc634-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc634-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}-->

```json
{
  "completedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "status": "string",
  "storageLocation": "String",
  "userId": "String",
  "submittedDateTime": "String (timestamp)", 
  "progress": "String (double)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dataPolicyOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
