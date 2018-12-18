---
title: directoryAudit リソースの種類
description: このリソースを表し、ディレクトリの監査項目のコレクション
author: lleonard-msft
ms.openlocfilehash: 5cbfc1320f721afd71ed3f196bb94a5c716d2c5c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312790"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="06b87-103">directoryAudit リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06b87-103">directoryAudit resource type</span></span>
<span data-ttu-id="06b87-104">このリソースを表し、ディレクトリの監査項目のコレクション</span><span class="sxs-lookup"><span data-stu-id="06b87-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="06b87-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="06b87-105">Methods</span></span>

| <span data-ttu-id="06b87-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="06b87-106">Method</span></span>           | <span data-ttu-id="06b87-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="06b87-107">Return Type</span></span>    |<span data-ttu-id="06b87-108">説明</span><span class="sxs-lookup"><span data-stu-id="06b87-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="06b87-109">リスト directoryAudits</span><span class="sxs-lookup"><span data-stu-id="06b87-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="06b87-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="06b87-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="06b87-111">コレクションとそのプロパティでディレクトリの監査項目を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="06b87-112">DirectoryAudit を取得します。</span><span class="sxs-lookup"><span data-stu-id="06b87-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="06b87-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="06b87-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="06b87-114">特定のディレクトリの監査項目とそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="06b87-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="06b87-115">Properties</span><span class="sxs-lookup"><span data-stu-id="06b87-115">Properties</span></span>
| <span data-ttu-id="06b87-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06b87-116">Property</span></span>     | <span data-ttu-id="06b87-117">種類</span><span class="sxs-lookup"><span data-stu-id="06b87-117">Type</span></span>   |<span data-ttu-id="06b87-118">説明</span><span class="sxs-lookup"><span data-stu-id="06b87-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06b87-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="06b87-119">activityDateTime</span></span>|<span data-ttu-id="06b87-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="06b87-120">DateTimeOffset</span></span>|<span data-ttu-id="06b87-121">アクティビティが実行された日時を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="06b87-122">タイムスタンプ型が、常に UTC 時刻です。</span><span class="sxs-lookup"><span data-stu-id="06b87-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="06b87-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="06b87-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="06b87-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="06b87-124">activityDisplayName</span></span>|<span data-ttu-id="06b87-125">String</span><span class="sxs-lookup"><span data-stu-id="06b87-125">String</span></span>|<span data-ttu-id="06b87-126">アクティビティ名または操作の名前 (例。</span><span class="sxs-lookup"><span data-stu-id="06b87-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="06b87-127">「ユーザーを作成する」、「グループ メンバーの追加」)。</span><span class="sxs-lookup"><span data-stu-id="06b87-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="06b87-128">ログに記録する活動のリストは、 [Azure の広告活動のリスト](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06b87-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="06b87-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="06b87-129">additionalDetails</span></span>|<span data-ttu-id="06b87-130">[keyValue](keyvalue.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b87-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="06b87-131">活動に関する詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="06b87-132">category</span><span class="sxs-lookup"><span data-stu-id="06b87-132">category</span></span>|<span data-ttu-id="06b87-133">String</span><span class="sxs-lookup"><span data-stu-id="06b87-133">String</span></span>|<span data-ttu-id="06b87-134">活動の対象となっているリソース カテゴリを示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="06b87-135">(例: ユーザーの管理、グループの管理などです。)。</span><span class="sxs-lookup"><span data-stu-id="06b87-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="06b87-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="06b87-136">correlationId</span></span>|<span data-ttu-id="06b87-137">GUID</span><span class="sxs-lookup"><span data-stu-id="06b87-137">GUID</span></span>|<span data-ttu-id="06b87-138">により、さまざまなサービス全体にわたる活動を関連付ける一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="06b87-139">サービス全体にわたるトレース ログを使用できます。</span><span class="sxs-lookup"><span data-stu-id="06b87-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="06b87-140">id</span><span class="sxs-lookup"><span data-stu-id="06b87-140">id</span></span>|<span data-ttu-id="06b87-141">String</span><span class="sxs-lookup"><span data-stu-id="06b87-141">String</span></span>| <span data-ttu-id="06b87-142">アクティビティの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="06b87-143">これは、GUID です。</span><span class="sxs-lookup"><span data-stu-id="06b87-143">This is a GUID.</span></span>|
|<span data-ttu-id="06b87-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="06b87-144">initiatedBy</span></span>|[<span data-ttu-id="06b87-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="06b87-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="06b87-146">ユーザーまたはアプリケーションに関する情報が、アクティビティを開始することを示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="06b87-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="06b87-147">loggedByService</span></span>|<span data-ttu-id="06b87-148">String</span><span class="sxs-lookup"><span data-stu-id="06b87-148">String</span></span>|<span data-ttu-id="06b87-149">サービスが動作を開始する情報を示します (例: セルフ サービスのパスワード管理、コア ディレクトリ、B2C、ユーザーの招待、Microsoft 個人情報管理、Id 管理の権限を持つ。</span><span class="sxs-lookup"><span data-stu-id="06b87-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="06b87-150">result</span><span class="sxs-lookup"><span data-stu-id="06b87-150">result</span></span>|<span data-ttu-id="06b87-151">string</span><span class="sxs-lookup"><span data-stu-id="06b87-151">string</span></span>| <span data-ttu-id="06b87-152">活動の結果を示します。使用可能な値: `success`、 `failure`、 `timeout`、 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="06b87-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="06b87-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="06b87-153">resultReason</span></span>|<span data-ttu-id="06b87-154">String</span><span class="sxs-lookup"><span data-stu-id="06b87-154">String</span></span>|<span data-ttu-id="06b87-155">結果が [エラー] または [タイムアウト] の場合は、エラーの原因を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="06b87-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="06b87-156">targetResources</span></span>|<span data-ttu-id="06b87-157">[targetResource](targetresource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="06b87-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="06b87-158">活動のためのリソースが変更された情報を示します。</span><span class="sxs-lookup"><span data-stu-id="06b87-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="06b87-159">ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリケーション、役割、グループ、ポリシーまたはその他を指定できます。</span><span class="sxs-lookup"><span data-stu-id="06b87-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="06b87-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06b87-160">Relationships</span></span>
<span data-ttu-id="06b87-161">なし</span><span class="sxs-lookup"><span data-stu-id="06b87-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="06b87-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06b87-162">JSON representation</span></span>

<span data-ttu-id="06b87-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06b87-163">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryAudit"
}-->

```json
{
  "activityDateTime": "String (timestamp)",
  "activityDisplayName": "String",
  "additionalDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
  "category": "String",
  "correlationId": "Guid",
  "id": "String (identifier)",
  "initiatedBy": {"@odata.type": "microsoft.graph.auditActivityInitiator"},
  "loggedByService": "String",
  "result": "string",
  "resultReason": "String",
  "targetResources": [{"@odata.type": "microsoft.graph.targetResource"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryAudit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->