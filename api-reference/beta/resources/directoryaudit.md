---
title: directoryAudit リソース型
description: このリソースでは、ディレクトリの監査アイテムとそのコレクションについて示します
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0f56dea1b07f0814c4b9f1295498c2555c98a2df
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573159"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="22ac5-103">directoryAudit リソース型</span><span class="sxs-lookup"><span data-stu-id="22ac5-103">directoryAudit resource type</span></span>
<span data-ttu-id="22ac5-104">このリソースでは、ディレクトリの監査アイテムとそのコレクションについて示します</span><span class="sxs-lookup"><span data-stu-id="22ac5-104">This resource represents the directory Audit items and its collection</span></span>


## <a name="methods"></a><span data-ttu-id="22ac5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="22ac5-105">Methods</span></span>

| <span data-ttu-id="22ac5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="22ac5-106">Method</span></span>           | <span data-ttu-id="22ac5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="22ac5-107">Return Type</span></span>    |<span data-ttu-id="22ac5-108">説明</span><span class="sxs-lookup"><span data-stu-id="22ac5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22ac5-109">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="22ac5-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="22ac5-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="22ac5-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="22ac5-111">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="22ac5-112">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="22ac5-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="22ac5-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="22ac5-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="22ac5-114">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-114">Get a specific directory audit item and its properties.</span></span>|


## <a name="properties"></a><span data-ttu-id="22ac5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ac5-115">Properties</span></span>
| <span data-ttu-id="22ac5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ac5-116">Property</span></span>     | <span data-ttu-id="22ac5-117">型</span><span class="sxs-lookup"><span data-stu-id="22ac5-117">Type</span></span>   |<span data-ttu-id="22ac5-118">説明</span><span class="sxs-lookup"><span data-stu-id="22ac5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22ac5-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="22ac5-119">activityDateTime</span></span>|<span data-ttu-id="22ac5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22ac5-120">DateTimeOffset</span></span>|<span data-ttu-id="22ac5-121">アクティビティが実行された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="22ac5-122">Timestamp 型は、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="22ac5-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="22ac5-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="22ac5-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="22ac5-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="22ac5-124">activityDisplayName</span></span>|<span data-ttu-id="22ac5-125">String</span><span class="sxs-lookup"><span data-stu-id="22ac5-125">String</span></span>|<span data-ttu-id="22ac5-126">アクティビティ名または操作名 (例:</span><span class="sxs-lookup"><span data-stu-id="22ac5-126">Indicates the activity name or the operation name (E.g.</span></span> <span data-ttu-id="22ac5-127">"Create User"、"Add member to group")。</span><span class="sxs-lookup"><span data-stu-id="22ac5-127">"Create User", "Add member to group").</span></span> <span data-ttu-id="22ac5-128">記録されるアクティビティの一覧は、[Azure AD アクティビティの一覧](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22ac5-128">For a list of activities logged,refer to [Azure Ad activity list](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="22ac5-129">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="22ac5-129">additionalDetails</span></span>|<span data-ttu-id="22ac5-130">[keyvalue](keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22ac5-130">[keyvalue](keyvalue.md) collection</span></span>|<span data-ttu-id="22ac5-131">アクティビティに関する詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-131">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="22ac5-132">category</span><span class="sxs-lookup"><span data-stu-id="22ac5-132">category</span></span>|<span data-ttu-id="22ac5-133">String</span><span class="sxs-lookup"><span data-stu-id="22ac5-133">String</span></span>|<span data-ttu-id="22ac5-134">どのリソース カテゴリがアクティビティの対象となっているかを示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-134">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="22ac5-135">(例: ユーザー管理、グループ管理など)</span><span class="sxs-lookup"><span data-stu-id="22ac5-135">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="22ac5-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="22ac5-136">correlationId</span></span>| <span data-ttu-id="22ac5-137">String (識別子)</span><span class="sxs-lookup"><span data-stu-id="22ac5-137">String (identifier)</span></span> |<span data-ttu-id="22ac5-138">さまざまなサービスの間にまたがるアクティビティを関連付けるのに役立つ一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-138">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="22ac5-139">サービスのログを追跡するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="22ac5-139">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="22ac5-140">id</span><span class="sxs-lookup"><span data-stu-id="22ac5-140">id</span></span>|<span data-ttu-id="22ac5-141">String</span><span class="sxs-lookup"><span data-stu-id="22ac5-141">String</span></span>| <span data-ttu-id="22ac5-142">アクティビティの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-142">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="22ac5-143">これは、GUID です。</span><span class="sxs-lookup"><span data-stu-id="22ac5-143">This is a GUID.</span></span>|
|<span data-ttu-id="22ac5-144">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="22ac5-144">initiatedBy</span></span>|[<span data-ttu-id="22ac5-145">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="22ac5-145">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="22ac5-146">アクティビティを開始したユーザーまたはアプリについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-146">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="22ac5-147">loggedByService</span><span class="sxs-lookup"><span data-stu-id="22ac5-147">loggedByService</span></span>|<span data-ttu-id="22ac5-148">String</span><span class="sxs-lookup"><span data-stu-id="22ac5-148">String</span></span>|<span data-ttu-id="22ac5-149">アクティビティを開始するサービスについての情報を示します (例: セルフ サービス パスワード管理、コア ディレクトリ、B2C、招待されたユーザー、Microsoft Identity Manager、Privileged Identity Management)。</span><span class="sxs-lookup"><span data-stu-id="22ac5-149">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="22ac5-150">result</span><span class="sxs-lookup"><span data-stu-id="22ac5-150">result</span></span>|<span data-ttu-id="22ac5-151">string</span><span class="sxs-lookup"><span data-stu-id="22ac5-151">string</span></span>| <span data-ttu-id="22ac5-152">アクティビティの結果を示します。使用可能な値は `success`、`failure`、`timeout`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="22ac5-152">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="22ac5-153">resultReason</span><span class="sxs-lookup"><span data-stu-id="22ac5-153">resultReason</span></span>|<span data-ttu-id="22ac5-154">String</span><span class="sxs-lookup"><span data-stu-id="22ac5-154">String</span></span>|<span data-ttu-id="22ac5-155">結果が「エラー」または「タイムアウト」の場合の、エラーの原因を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-155">Indicates the reason for failure if the result is "Failure" or "timeout".</span></span>|
|<span data-ttu-id="22ac5-156">targetResources</span><span class="sxs-lookup"><span data-stu-id="22ac5-156">targetResources</span></span>|<span data-ttu-id="22ac5-157">[targetResource](targetresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="22ac5-157">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="22ac5-158">アクティビティのためにどのリソースが変更されたかについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="22ac5-158">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="22ac5-159">ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリ、役割、グループ、ポリシー、その他があります。</span><span class="sxs-lookup"><span data-stu-id="22ac5-159">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="22ac5-160">関係</span><span class="sxs-lookup"><span data-stu-id="22ac5-160">Relationships</span></span>
<span data-ttu-id="22ac5-161">なし</span><span class="sxs-lookup"><span data-stu-id="22ac5-161">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="22ac5-162">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22ac5-162">JSON representation</span></span>

<span data-ttu-id="22ac5-163">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22ac5-163">Here is a JSON representation of the resource.</span></span>

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
  "correlationId": "String (identifier)",
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
