---
title: directoryAudit リソース型
description: ディレクトリ監査アイテムとそのコレクションを表します。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f49229ed1ce461a0e9dcc104087ec89726597267
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629293"
---
# <a name="directoryaudit-resource-type"></a><span data-ttu-id="bf6d1-103">directoryAudit リソース型</span><span class="sxs-lookup"><span data-stu-id="bf6d1-103">directoryAudit resource type</span></span>

<span data-ttu-id="bf6d1-104">ディレクトリ監査アイテムとそのコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-104">Represents the directory audit items and its collection.</span></span>

## <a name="methods"></a><span data-ttu-id="bf6d1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf6d1-105">Methods</span></span>

| <span data-ttu-id="bf6d1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="bf6d1-106">Method</span></span>           | <span data-ttu-id="bf6d1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bf6d1-107">Return Type</span></span>    |<span data-ttu-id="bf6d1-108">説明</span><span class="sxs-lookup"><span data-stu-id="bf6d1-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bf6d1-109">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="bf6d1-109">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="bf6d1-110">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="bf6d1-110">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="bf6d1-111">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-111">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="bf6d1-112">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="bf6d1-112">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="bf6d1-113">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="bf6d1-113">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="bf6d1-114">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-114">Get a specific directory audit item and its properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="bf6d1-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf6d1-115">Properties</span></span>

| <span data-ttu-id="bf6d1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf6d1-116">Property</span></span>     | <span data-ttu-id="bf6d1-117">型</span><span class="sxs-lookup"><span data-stu-id="bf6d1-117">Type</span></span>   |<span data-ttu-id="bf6d1-118">説明</span><span class="sxs-lookup"><span data-stu-id="bf6d1-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bf6d1-119">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="bf6d1-119">activityDateTime</span></span>|<span data-ttu-id="bf6d1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf6d1-120">DateTimeOffset</span></span>|<span data-ttu-id="bf6d1-121">アクティビティが実行された日付と時刻を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-121">Indicates the date and time the activity was performed.</span></span> <span data-ttu-id="bf6d1-122">Timestamp 型は、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-122">The Timestamp type is always in UTC time.</span></span> <span data-ttu-id="bf6d1-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="bf6d1-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="bf6d1-124">activityDisplayName</span><span class="sxs-lookup"><span data-stu-id="bf6d1-124">activityDisplayName</span></span>|<span data-ttu-id="bf6d1-125">String</span><span class="sxs-lookup"><span data-stu-id="bf6d1-125">String</span></span>|<span data-ttu-id="bf6d1-126">アクティビティ名または操作名 (例: [ユーザーの作成] と [グループにメンバーを追加]) を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-126">Indicates the activity name or the operation name (examples: "Create User" and "Add member to group").</span></span> <span data-ttu-id="bf6d1-127">完全なリストについては、「 [AZURE AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-127">For full list, see [Azure AD activity list](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-activity-audit-logs#azure-ad-audit-activity-list).</span></span>|
|<span data-ttu-id="bf6d1-128">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="bf6d1-128">additionalDetails</span></span>|<span data-ttu-id="bf6d1-129">[keyvalue](keyvalue.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bf6d1-129">[keyValue](keyvalue.md) collection</span></span>|<span data-ttu-id="bf6d1-130">アクティビティに関する詳細情報を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-130">Indicates additional details on the activity.</span></span>|
|<span data-ttu-id="bf6d1-131">category</span><span class="sxs-lookup"><span data-stu-id="bf6d1-131">category</span></span>|<span data-ttu-id="bf6d1-132">String</span><span class="sxs-lookup"><span data-stu-id="bf6d1-132">String</span></span>|<span data-ttu-id="bf6d1-133">どのリソース カテゴリがアクティビティの対象となっているかを示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-133">Indicates which resource category that's targeted by the activity.</span></span> <span data-ttu-id="bf6d1-134">(例: ユーザー管理、グループ管理など)</span><span class="sxs-lookup"><span data-stu-id="bf6d1-134">(For example: User Management, Group Management etc..)</span></span>|
|<span data-ttu-id="bf6d1-135">correlationId</span><span class="sxs-lookup"><span data-stu-id="bf6d1-135">correlationId</span></span>|<span data-ttu-id="bf6d1-136">GUID</span><span class="sxs-lookup"><span data-stu-id="bf6d1-136">GUID</span></span>|<span data-ttu-id="bf6d1-137">さまざまなサービスの間にまたがるアクティビティを関連付けるのに役立つ一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-137">Indicates a unique ID that helps correlate activities that span across various services.</span></span> <span data-ttu-id="bf6d1-138">サービスのログを追跡するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-138">Can be used to trace logs across services.</span></span>|
|<span data-ttu-id="bf6d1-139">id</span><span class="sxs-lookup"><span data-stu-id="bf6d1-139">id</span></span>|<span data-ttu-id="bf6d1-140">文字列</span><span class="sxs-lookup"><span data-stu-id="bf6d1-140">String</span></span>| <span data-ttu-id="bf6d1-141">アクティビティの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-141">Indicates the unique ID for the activity.</span></span> <span data-ttu-id="bf6d1-142">これは、GUID です。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-142">This is a GUID.</span></span>|
|<span data-ttu-id="bf6d1-143">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="bf6d1-143">initiatedBy</span></span>|[<span data-ttu-id="bf6d1-144">auditActivityInitiator</span><span class="sxs-lookup"><span data-stu-id="bf6d1-144">auditActivityInitiator</span></span>](auditactivityinitiator.md)|<span data-ttu-id="bf6d1-145">アクティビティを開始したユーザーまたはアプリについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-145">Indicates information about the user or app initiated the activity.</span></span>|
|<span data-ttu-id="bf6d1-146">loggedByService</span><span class="sxs-lookup"><span data-stu-id="bf6d1-146">loggedByService</span></span>|<span data-ttu-id="bf6d1-147">String</span><span class="sxs-lookup"><span data-stu-id="bf6d1-147">String</span></span>|<span data-ttu-id="bf6d1-148">アクティビティを開始するサービスについての情報を示します (例: セルフ サービス パスワード管理、コア ディレクトリ、B2C、招待されたユーザー、Microsoft Identity Manager、Privileged Identity Management)。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-148">Indicates information on which service initiated the activity (For example: Self-service Password Management, Core Directory, B2C, Invited Users, Microsoft Identity Manager, Privileged Identity Management.</span></span>|
|<span data-ttu-id="bf6d1-149">result</span><span class="sxs-lookup"><span data-stu-id="bf6d1-149">result</span></span>|<span data-ttu-id="bf6d1-150">string</span><span class="sxs-lookup"><span data-stu-id="bf6d1-150">string</span></span>| <span data-ttu-id="bf6d1-151">アクティビティの結果を示します。使用可能な値は `success`、`failure`、`timeout`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-151">Indicates the result of the activity.Possible values are: `success`, `failure`, `timeout`, `unknownFutureValue`.</span></span>||
|<span data-ttu-id="bf6d1-152">resultReason</span><span class="sxs-lookup"><span data-stu-id="bf6d1-152">resultReason</span></span>|<span data-ttu-id="bf6d1-153">String</span><span class="sxs-lookup"><span data-stu-id="bf6d1-153">String</span></span>|<span data-ttu-id="bf6d1-154">"失敗" または "タイムアウト" の結果について説明します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-154">Describes cause of "failure" or "timeout" results.</span></span>|
|<span data-ttu-id="bf6d1-155">targetResources</span><span class="sxs-lookup"><span data-stu-id="bf6d1-155">targetResources</span></span>|<span data-ttu-id="bf6d1-156">[targetResource](targetresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bf6d1-156">[targetResource](targetresource.md) collection</span></span>|<span data-ttu-id="bf6d1-157">アクティビティのためにどのリソースが変更されたかについての情報を示します。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-157">Indicates information on which resource was changed due to the activity.</span></span> <span data-ttu-id="bf6d1-158">ターゲット リソースの型には、ユーザー、デバイス、ディレクトリ、アプリ、役割、グループ、ポリシー、その他があります。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-158">Target Resource Type can be User, Device, Directory, App, Role, Group, Policy or Other.</span></span>

## <a name="relationships"></a><span data-ttu-id="bf6d1-159">関係</span><span class="sxs-lookup"><span data-stu-id="bf6d1-159">Relationships</span></span>

<span data-ttu-id="bf6d1-160">なし</span><span class="sxs-lookup"><span data-stu-id="bf6d1-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf6d1-161">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf6d1-161">JSON representation</span></span>

<span data-ttu-id="bf6d1-162">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf6d1-162">Here is a JSON representation of the resource.</span></span>

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