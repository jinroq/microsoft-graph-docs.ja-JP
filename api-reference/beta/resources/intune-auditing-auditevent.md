---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3eddfcbd94153bfc1f7d1798f8806fb84b6341bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425163"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="91367-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="91367-103">auditEvent resource type</span></span>

> <span data-ttu-id="91367-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91367-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="91367-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91367-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91367-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91367-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91367-107">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="91367-107">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="91367-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="91367-108">Methods</span></span>
|<span data-ttu-id="91367-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="91367-109">Method</span></span>|<span data-ttu-id="91367-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91367-110">Return Type</span></span>|<span data-ttu-id="91367-111">説明</span><span class="sxs-lookup"><span data-stu-id="91367-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91367-112">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="91367-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="91367-113">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91367-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="91367-114">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="91367-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="91367-115">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="91367-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91367-117">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="91367-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91367-118">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="91367-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91367-120">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91367-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91367-121">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="91367-122">なし</span><span class="sxs-lookup"><span data-stu-id="91367-122">None</span></span>|<span data-ttu-id="91367-123">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="91367-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="91367-124">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="91367-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91367-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91367-126">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="91367-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91367-127">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="91367-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="91367-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="91367-128">String collection</span></span>|<span data-ttu-id="91367-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="91367-129">Not yet documented</span></span>|
|[<span data-ttu-id="91367-130">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="91367-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="91367-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="91367-131">String collection</span></span>|<span data-ttu-id="91367-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="91367-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="91367-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91367-133">Properties</span></span>
|<span data-ttu-id="91367-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91367-134">Property</span></span>|<span data-ttu-id="91367-135">型</span><span class="sxs-lookup"><span data-stu-id="91367-135">Type</span></span>|<span data-ttu-id="91367-136">説明</span><span class="sxs-lookup"><span data-stu-id="91367-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91367-137">id</span><span class="sxs-lookup"><span data-stu-id="91367-137">id</span></span>|<span data-ttu-id="91367-138">String</span><span class="sxs-lookup"><span data-stu-id="91367-138">String</span></span>|<span data-ttu-id="91367-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="91367-139">Key of the entity.</span></span>|
|<span data-ttu-id="91367-140">displayName</span><span class="sxs-lookup"><span data-stu-id="91367-140">displayName</span></span>|<span data-ttu-id="91367-141">String</span><span class="sxs-lookup"><span data-stu-id="91367-141">String</span></span>|<span data-ttu-id="91367-142">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="91367-142">Event display name.</span></span>|
|<span data-ttu-id="91367-143">componentName</span><span class="sxs-lookup"><span data-stu-id="91367-143">componentName</span></span>|<span data-ttu-id="91367-144">String</span><span class="sxs-lookup"><span data-stu-id="91367-144">String</span></span>|<span data-ttu-id="91367-145">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="91367-145">Component name.</span></span>|
|<span data-ttu-id="91367-146">actor</span><span class="sxs-lookup"><span data-stu-id="91367-146">actor</span></span>|[<span data-ttu-id="91367-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="91367-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="91367-148">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="91367-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="91367-149">activity</span><span class="sxs-lookup"><span data-stu-id="91367-149">activity</span></span>|<span data-ttu-id="91367-150">String</span><span class="sxs-lookup"><span data-stu-id="91367-150">String</span></span>|<span data-ttu-id="91367-151">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="91367-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="91367-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="91367-152">activityDateTime</span></span>|<span data-ttu-id="91367-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91367-153">DateTimeOffset</span></span>|<span data-ttu-id="91367-154">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="91367-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="91367-155">activityType</span><span class="sxs-lookup"><span data-stu-id="91367-155">activityType</span></span>|<span data-ttu-id="91367-156">String</span><span class="sxs-lookup"><span data-stu-id="91367-156">String</span></span>|<span data-ttu-id="91367-157">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="91367-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="91367-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="91367-158">activityOperationType</span></span>|<span data-ttu-id="91367-159">String</span><span class="sxs-lookup"><span data-stu-id="91367-159">String</span></span>|<span data-ttu-id="91367-160">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="91367-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="91367-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="91367-161">activityResult</span></span>|<span data-ttu-id="91367-162">String</span><span class="sxs-lookup"><span data-stu-id="91367-162">String</span></span>|<span data-ttu-id="91367-163">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="91367-163">The result of the activity.</span></span>|
|<span data-ttu-id="91367-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="91367-164">correlationId</span></span>|<span data-ttu-id="91367-165">Guid</span><span class="sxs-lookup"><span data-stu-id="91367-165">Guid</span></span>|<span data-ttu-id="91367-166">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="91367-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="91367-167">resources</span><span class="sxs-lookup"><span data-stu-id="91367-167">resources</span></span>|<span data-ttu-id="91367-168">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91367-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="91367-169">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="91367-169">Resources being modified.</span></span>|
|<span data-ttu-id="91367-170">category</span><span class="sxs-lookup"><span data-stu-id="91367-170">category</span></span>|<span data-ttu-id="91367-171">String</span><span class="sxs-lookup"><span data-stu-id="91367-171">String</span></span>|<span data-ttu-id="91367-172">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="91367-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91367-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91367-173">Relationships</span></span>
<span data-ttu-id="91367-174">なし</span><span class="sxs-lookup"><span data-stu-id="91367-174">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91367-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91367-175">JSON Representation</span></span>
<span data-ttu-id="91367-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91367-176">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```




