---
title: directoryAudit リソース型
description: ディレクトリ (テナント) のアクティビティ (ベータ版) を監査するための、Microsoft Graph API (REST) の directoryAudit リソース (エンティティ) について説明します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e7e2c2bcf9708dd00054a31bcee3ba06fd100549
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657946"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="6e66d-103">directoryAudit リソース型</span><span class="sxs-lookup"><span data-stu-id="6e66d-103">directoryAudit resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e66d-104">ディレクトリの監査アイテムとそのコレクションについて示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-104">This resource represents the directory Audit items and its collection</span></span>

## <a name="methods"></a><span data-ttu-id="6e66d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e66d-105">Methods</span></span>

| <span data-ttu-id="6e66d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6e66d-106">Method</span></span>           | <span data-ttu-id="6e66d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6e66d-107">Return Type</span></span>    |<span data-ttu-id="6e66d-108">説明</span><span class="sxs-lookup"><span data-stu-id="6e66d-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6e66d-109">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="6e66d-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="6e66d-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6e66d-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="6e66d-111">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="6e66d-112">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="6e66d-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="6e66d-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="6e66d-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="6e66d-114">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="6e66d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e66d-115">Properties</span></span>
| <span data-ttu-id="6e66d-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6e66d-116">Property</span></span>     | <span data-ttu-id="6e66d-117">型</span><span class="sxs-lookup"><span data-stu-id="6e66d-117">Type</span></span>   |<span data-ttu-id="6e66d-118">説明</span><span class="sxs-lookup"><span data-stu-id="6e66d-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e66d-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="6e66d-119">activityDateTime</span></span>|<span data-ttu-id="6e66d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e66d-120">DateTimeOffset</span></span>|<span data-ttu-id="6e66d-121">アクティビティが実行された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="6e66d-122">Timestamp 型は、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="6e66d-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="6e66d-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6e66d-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6e66d-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="6e66d-124">activityDisplayName</span></span>|<span data-ttu-id="6e66d-125">String</span><span class="sxs-lookup"><span data-stu-id="6e66d-125">String</span></span>|<span data-ttu-id="6e66d-126">アクティビティ名または操作名 (例:</span><span class="sxs-lookup"><span data-stu-id="6e66d-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="6e66d-127">"Create User"、"Add member to group")。</span><span class="sxs-lookup"><span data-stu-id="6e66d-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="6e66d-128">記録されるアクティビティの一覧は、[Azure AD アクティビティの一覧](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e66d-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="6e66d-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="6e66d-129">additionalDetails</span></span>|<span data-ttu-id="6e66d-130">[keyvalue](keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e66d-130">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="6e66d-131">アクティビティに関する詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="6e66d-132">category</span><span class="sxs-lookup"><span data-stu-id="6e66d-132">category</span></span>|<span data-ttu-id="6e66d-133">String</span><span class="sxs-lookup"><span data-stu-id="6e66d-133">String</span></span>|<span data-ttu-id="6e66d-134">どのリソース カテゴリがアクティビティの対象となっているかを示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="6e66d-135">(例: ユーザー管理、グループ管理など)</span><span class="sxs-lookup"><span data-stu-id="6e66d-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="6e66d-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="6e66d-136">correlationId</span></span>|<span data-ttu-id="6e66d-137">GUID</span><span class="sxs-lookup"><span data-stu-id="6e66d-137">GUID</span></span>|<span data-ttu-id="6e66d-138">さまざまなサービスの間にまたがるアクティビティを関連付けるのに役立つ一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="6e66d-139">サービスのログを追跡するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="6e66d-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="6e66d-140">id</span><span class="sxs-lookup"><span data-stu-id="6e66d-140">id</span></span>|<span data-ttu-id="6e66d-141">String</span><span class="sxs-lookup"><span data-stu-id="6e66d-141">String</span></span>| <span data-ttu-id="6e66d-142">アクティビティの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="6e66d-143">これは、GUID です。</span><span class="sxs-lookup"><span data-stu-id="6e66d-143">This is a GUID.</span></span>|
|<span data-ttu-id="6e66d-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="6e66d-144">initiatedBy</span></span>|[<span data-ttu-id="6e66d-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="6e66d-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="6e66d-146">アクティビティを開始したユーザーまたはアプリについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="6e66d-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="6e66d-147">loggedByService</span></span>|<span data-ttu-id="6e66d-148">String</span><span class="sxs-lookup"><span data-stu-id="6e66d-148">String</span></span>|<span data-ttu-id="6e66d-149">アクティビティを開始するサービスについての情報を示します (例: セルフ サービス パスワード管理、コア ディレクトリ、B2C、招待されたユーザー、Microsoft Identity Manager、Privileged Identity Management)。</span><span class="sxs-lookup"><span data-stu-id="6e66d-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="6e66d-150">result</span><span class="sxs-lookup"><span data-stu-id="6e66d-150">result</span></span>|<span data-ttu-id="6e66d-151">string</span><span class="sxs-lookup"><span data-stu-id="6e66d-151">string</span></span>| <span data-ttu-id="6e66d-152">アクティビティの結果を示します。使用可能な値は `success`、`failure`、`timeout`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="6e66d-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="6e66d-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="6e66d-153">resultReason</span></span>|<span data-ttu-id="6e66d-154">String</span><span class="sxs-lookup"><span data-stu-id="6e66d-154">String</span></span>|<span data-ttu-id="6e66d-155">結果が「エラー」または「タイムアウト」の場合の、エラーの原因を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="6e66d-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="6e66d-156">targetResources</span></span>|<span data-ttu-id="6e66d-157">[targetResource](targetresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6e66d-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="6e66d-158">アクティビティのためにどのリソースが変更されたかについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="6e66d-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="6e66d-159">ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリ、役割、グループ、ポリシー、その他があります。</span><span class="sxs-lookup"><span data-stu-id="6e66d-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="6e66d-160">関係</span><span class="sxs-lookup"><span data-stu-id="6e66d-160">Relationships</span></span>
<span data-ttu-id="6e66d-161">なし</span><span class="sxs-lookup"><span data-stu-id="6e66d-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e66d-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6e66d-162">JSON representation</span></span>

<span data-ttu-id="6e66d-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6e66d-163">Here is a JSON representation of the resource.</span></span>

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
