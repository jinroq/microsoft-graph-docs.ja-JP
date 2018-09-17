# <a name="process-resource-type"></a><span data-ttu-id="7f25e-101">プロセス リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f25e-101">process resource type</span></span>

<span data-ttu-id="7f25e-102">ステートフルなアラートに関連するプロセスについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="7f25e-102">Contains stateful information about the process related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="7f25e-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f25e-103">Properties</span></span>

| <span data-ttu-id="7f25e-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f25e-104">Property</span></span>   | <span data-ttu-id="7f25e-105">型</span><span class="sxs-lookup"><span data-stu-id="7f25e-105">Type</span></span>|<span data-ttu-id="7f25e-106">説明</span><span class="sxs-lookup"><span data-stu-id="7f25e-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f25e-107">accountName</span><span class="sxs-lookup"><span data-stu-id="7f25e-107">accountName</span></span>|<span data-ttu-id="7f25e-108">文字列</span><span class="sxs-lookup"><span data-stu-id="7f25e-108">String</span></span>|<span data-ttu-id="7f25e-109">ユーザーは、例、アカウント名、SID、およびように識別子 (ユーザー アカウントのコンテキストでプロセスが実行された) を考慮します。</span><span class="sxs-lookup"><span data-stu-id="7f25e-109">User account identifier (user account context the process ran under) for example, AccountName, SID, and so on.</span></span>|
|<span data-ttu-id="7f25e-110">commandLine</span><span class="sxs-lookup"><span data-stu-id="7f25e-110">commandLine</span></span>|<span data-ttu-id="7f25e-111">文字列</span><span class="sxs-lookup"><span data-stu-id="7f25e-111">String</span></span>|<span data-ttu-id="7f25e-112">完全な処理の呼び出しは、すべてのパラメーターを含むを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7f25e-112">The full process invocation commandline including all parameters.</span></span>|
|<span data-ttu-id="7f25e-113">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f25e-113">createdDateTime</span></span>|<span data-ttu-id="7f25e-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f25e-114">DateTimeOffset</span></span>|<span data-ttu-id="7f25e-115">プロセスが開始された時刻です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-115">Time at which the process was started.</span></span> <span data-ttu-id="7f25e-116">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表示し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f25e-117">例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります：`'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="7f25e-117">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7f25e-118">fileHash</span><span class="sxs-lookup"><span data-stu-id="7f25e-118">fileHash</span></span>|[<span data-ttu-id="7f25e-119">fileHash</span><span class="sxs-lookup"><span data-stu-id="7f25e-119">fileHash</span></span>](filehash.md)|<span data-ttu-id="7f25e-120">複合型の暗号化などの場所に依存したファイルのハッシュが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7f25e-120">Complex type containing file hashes (cryptographic and location-sensitive).</span></span>|
|<span data-ttu-id="7f25e-121">integrityLevel</span><span class="sxs-lookup"><span data-stu-id="7f25e-121">integrityLevel</span></span>|<span data-ttu-id="7f25e-122">processIntegrityLevel</span><span class="sxs-lookup"><span data-stu-id="7f25e-122">processIntegrityLevel</span></span>|<span data-ttu-id="7f25e-123">プロセスの整合性レベルです。</span><span class="sxs-lookup"><span data-stu-id="7f25e-123">The integrity level of the process.</span></span> <span data-ttu-id="7f25e-124">可能な値は、`unknown`、`untrusted`、`low`、`medium`、`high`、`system` です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-124">Possible values are: `unknown`, `untrusted`, `low`, `medium`, `high`, `system`.</span></span>|
|<span data-ttu-id="7f25e-125">isElevated</span><span class="sxs-lookup"><span data-stu-id="7f25e-125">isElevated</span></span>|<span data-ttu-id="7f25e-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="7f25e-126">Boolean</span></span>|<span data-ttu-id="7f25e-127">プロセスが昇格した場合はTrueです。</span><span class="sxs-lookup"><span data-stu-id="7f25e-127">True if the process is elevated.</span></span>|
|<span data-ttu-id="7f25e-128">名前</span><span class="sxs-lookup"><span data-stu-id="7f25e-128">name</span></span>|<span data-ttu-id="7f25e-129">文字列</span><span class="sxs-lookup"><span data-stu-id="7f25e-129">String</span></span>|<span data-ttu-id="7f25e-130">プロセスの画像ファイル名です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-130">The name of the process' Image file.</span></span>|
|<span data-ttu-id="7f25e-131">parentProcessCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f25e-131">parentProcessCreatedDateTime</span></span>|<span data-ttu-id="7f25e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f25e-132">DateTimeOffset</span></span>|<span data-ttu-id="7f25e-133">親プロセスの開始日時。</span><span class="sxs-lookup"><span data-stu-id="7f25e-133">DateTime at which the parent process was started.</span></span> <span data-ttu-id="7f25e-134">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表示し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7f25e-135">例えば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります：`'2014-01-01T00:00:00Z'` 。</span><span class="sxs-lookup"><span data-stu-id="7f25e-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="7f25e-136">parentProcessId</span><span class="sxs-lookup"><span data-stu-id="7f25e-136">parentProcessId</span></span>|<span data-ttu-id="7f25e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="7f25e-137">Int32</span></span>|<span data-ttu-id="7f25e-138"> 親プロセスのプロセス ID (PID)です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-138">The Process ID (PID) of the parent process.</span></span>|
|<span data-ttu-id="7f25e-139">parentProcessName</span><span class="sxs-lookup"><span data-stu-id="7f25e-139">parentProcessName</span></span>|<span data-ttu-id="7f25e-140">文字列</span><span class="sxs-lookup"><span data-stu-id="7f25e-140">String</span></span>|<span data-ttu-id="7f25e-141">親プロセスの画像ファイル名です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-141">The name of the image file of the parent process.</span></span>|
|<span data-ttu-id="7f25e-142">パス</span><span class="sxs-lookup"><span data-stu-id="7f25e-142">path</span></span>|<span data-ttu-id="7f25e-143">文字列</span><span class="sxs-lookup"><span data-stu-id="7f25e-143">String</span></span>|<span data-ttu-id="7f25e-144">ファイル名を含む完全パスです。</span><span class="sxs-lookup"><span data-stu-id="7f25e-144">Full path, including filename.</span></span>|
|<span data-ttu-id="7f25e-145">processId</span><span class="sxs-lookup"><span data-stu-id="7f25e-145">processId</span></span>|<span data-ttu-id="7f25e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="7f25e-146">Int32</span></span>|<span data-ttu-id="7f25e-147">プロセスのプロセス ID (PID)です。</span><span class="sxs-lookup"><span data-stu-id="7f25e-147">The Process ID (PID) of the process.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7f25e-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f25e-148">JSON representation</span></span>

<span data-ttu-id="7f25e-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f25e-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.process"
}-->

```json
{
  "accountName": "String",
  "commandLine": "String",
  "createdDateTime": "String (timestamp)",
  "fileHash": {"@odata.type": "microsoft.graph.fileHash"},
  "integrityLevel": "@odata.type: microsoft.graph.processIntegrityLevel",
  "isElevated": true,
  "name": "String",
  "parentProcessCreatedDateTime": "String (timestamp)",
  "parentProcessId": 1024,
  "parentProcessName": "String",
  "path": "String",
  "processId": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "process resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->