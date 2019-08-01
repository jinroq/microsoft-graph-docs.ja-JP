---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 18d56205f0602016f4d2ecdd2587b06ae5c676fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028855"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="8c54a-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8c54a-103">auditEvent resource type</span></span>

> <span data-ttu-id="8c54a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c54a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c54a-105">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="8c54a-105">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="8c54a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c54a-106">Methods</span></span>
|<span data-ttu-id="8c54a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c54a-107">Method</span></span>|<span data-ttu-id="8c54a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8c54a-108">Return Type</span></span>|<span data-ttu-id="8c54a-109">説明</span><span class="sxs-lookup"><span data-stu-id="8c54a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c54a-110">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="8c54a-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="8c54a-111">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8c54a-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="8c54a-112">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8c54a-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="8c54a-113">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="8c54a-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="8c54a-115">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8c54a-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="8c54a-116">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="8c54a-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="8c54a-118">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c54a-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="8c54a-119">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="8c54a-120">なし</span><span class="sxs-lookup"><span data-stu-id="8c54a-120">None</span></span>|<span data-ttu-id="8c54a-121">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8c54a-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="8c54a-122">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="8c54a-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="8c54a-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="8c54a-124">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c54a-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="8c54a-125">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="8c54a-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="8c54a-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8c54a-126">String collection</span></span>|<span data-ttu-id="8c54a-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8c54a-127">Not yet documented</span></span>|
|[<span data-ttu-id="8c54a-128">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="8c54a-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="8c54a-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8c54a-129">String collection</span></span>|<span data-ttu-id="8c54a-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8c54a-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8c54a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c54a-131">Properties</span></span>
|<span data-ttu-id="8c54a-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c54a-132">Property</span></span>|<span data-ttu-id="8c54a-133">型</span><span class="sxs-lookup"><span data-stu-id="8c54a-133">Type</span></span>|<span data-ttu-id="8c54a-134">説明</span><span class="sxs-lookup"><span data-stu-id="8c54a-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c54a-135">id</span><span class="sxs-lookup"><span data-stu-id="8c54a-135">id</span></span>|<span data-ttu-id="8c54a-136">文字列</span><span class="sxs-lookup"><span data-stu-id="8c54a-136">String</span></span>|<span data-ttu-id="8c54a-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8c54a-137">Key of the entity.</span></span>|
|<span data-ttu-id="8c54a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8c54a-138">displayName</span></span>|<span data-ttu-id="8c54a-139">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-139">String</span></span>|<span data-ttu-id="8c54a-140">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="8c54a-140">Event display name.</span></span>|
|<span data-ttu-id="8c54a-141">componentName</span><span class="sxs-lookup"><span data-stu-id="8c54a-141">componentName</span></span>|<span data-ttu-id="8c54a-142">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-142">String</span></span>|<span data-ttu-id="8c54a-143">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="8c54a-143">Component name.</span></span>|
|<span data-ttu-id="8c54a-144">actor</span><span class="sxs-lookup"><span data-stu-id="8c54a-144">actor</span></span>|[<span data-ttu-id="8c54a-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="8c54a-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="8c54a-146">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="8c54a-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="8c54a-147">activity</span><span class="sxs-lookup"><span data-stu-id="8c54a-147">activity</span></span>|<span data-ttu-id="8c54a-148">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-148">String</span></span>|<span data-ttu-id="8c54a-149">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="8c54a-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="8c54a-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="8c54a-150">activityDateTime</span></span>|<span data-ttu-id="8c54a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c54a-151">DateTimeOffset</span></span>|<span data-ttu-id="8c54a-152">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="8c54a-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="8c54a-153">activityType</span><span class="sxs-lookup"><span data-stu-id="8c54a-153">activityType</span></span>|<span data-ttu-id="8c54a-154">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-154">String</span></span>|<span data-ttu-id="8c54a-155">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="8c54a-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="8c54a-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="8c54a-156">activityOperationType</span></span>|<span data-ttu-id="8c54a-157">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-157">String</span></span>|<span data-ttu-id="8c54a-158">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="8c54a-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="8c54a-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="8c54a-159">activityResult</span></span>|<span data-ttu-id="8c54a-160">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-160">String</span></span>|<span data-ttu-id="8c54a-161">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="8c54a-161">The result of the activity.</span></span>|
|<span data-ttu-id="8c54a-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="8c54a-162">correlationId</span></span>|<span data-ttu-id="8c54a-163">Guid</span><span class="sxs-lookup"><span data-stu-id="8c54a-163">Guid</span></span>|<span data-ttu-id="8c54a-164">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="8c54a-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="8c54a-165">resources</span><span class="sxs-lookup"><span data-stu-id="8c54a-165">resources</span></span>|<span data-ttu-id="8c54a-166">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8c54a-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="8c54a-167">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="8c54a-167">Resources being modified.</span></span>|
|<span data-ttu-id="8c54a-168">category</span><span class="sxs-lookup"><span data-stu-id="8c54a-168">category</span></span>|<span data-ttu-id="8c54a-169">String</span><span class="sxs-lookup"><span data-stu-id="8c54a-169">String</span></span>|<span data-ttu-id="8c54a-170">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="8c54a-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c54a-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c54a-171">Relationships</span></span>
<span data-ttu-id="8c54a-172">なし</span><span class="sxs-lookup"><span data-stu-id="8c54a-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c54a-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c54a-173">JSON Representation</span></span>
<span data-ttu-id="8c54a-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c54a-174">Here is a JSON representation of the resource.</span></span>
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



