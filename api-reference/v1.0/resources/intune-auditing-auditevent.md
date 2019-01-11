---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 914d4ac5aa666aa430224f582df8f99dbcf60701
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862364"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="c18a6-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c18a6-103">auditEvent resource type</span></span>

> <span data-ttu-id="c18a6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c18a6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c18a6-105">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="c18a6-105">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="c18a6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="c18a6-106">Methods</span></span>
|<span data-ttu-id="c18a6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c18a6-107">Method</span></span>|<span data-ttu-id="c18a6-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c18a6-108">Return Type</span></span>|<span data-ttu-id="c18a6-109">説明</span><span class="sxs-lookup"><span data-stu-id="c18a6-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c18a6-110">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="c18a6-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="c18a6-111">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c18a6-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="c18a6-112">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c18a6-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="c18a6-113">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="c18a6-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="c18a6-115">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c18a6-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="c18a6-116">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="c18a6-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="c18a6-118">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c18a6-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="c18a6-119">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="c18a6-120">なし</span><span class="sxs-lookup"><span data-stu-id="c18a6-120">None</span></span>|<span data-ttu-id="c18a6-121">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c18a6-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="c18a6-122">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="c18a6-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="c18a6-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="c18a6-124">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c18a6-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="c18a6-125">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="c18a6-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="c18a6-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c18a6-126">String collection</span></span>|<span data-ttu-id="c18a6-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c18a6-127">Not yet documented</span></span>|
|[<span data-ttu-id="c18a6-128">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="c18a6-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="c18a6-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c18a6-129">String collection</span></span>|<span data-ttu-id="c18a6-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c18a6-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c18a6-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18a6-131">Properties</span></span>
|<span data-ttu-id="c18a6-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18a6-132">Property</span></span>|<span data-ttu-id="c18a6-133">種類</span><span class="sxs-lookup"><span data-stu-id="c18a6-133">Type</span></span>|<span data-ttu-id="c18a6-134">説明</span><span class="sxs-lookup"><span data-stu-id="c18a6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c18a6-135">ID</span><span class="sxs-lookup"><span data-stu-id="c18a6-135">id</span></span>|<span data-ttu-id="c18a6-136">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-136">String</span></span>|<span data-ttu-id="c18a6-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c18a6-137">Key of the entity.</span></span>|
|<span data-ttu-id="c18a6-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c18a6-138">displayName</span></span>|<span data-ttu-id="c18a6-139">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-139">String</span></span>|<span data-ttu-id="c18a6-140">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="c18a6-140">Event display name.</span></span>|
|<span data-ttu-id="c18a6-141">componentName</span><span class="sxs-lookup"><span data-stu-id="c18a6-141">componentName</span></span>|<span data-ttu-id="c18a6-142">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-142">String</span></span>|<span data-ttu-id="c18a6-143">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="c18a6-143">Component name.</span></span>|
|<span data-ttu-id="c18a6-144">actor</span><span class="sxs-lookup"><span data-stu-id="c18a6-144">actor</span></span>|[<span data-ttu-id="c18a6-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="c18a6-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="c18a6-146">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="c18a6-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="c18a6-147">activity</span><span class="sxs-lookup"><span data-stu-id="c18a6-147">activity</span></span>|<span data-ttu-id="c18a6-148">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-148">String</span></span>|<span data-ttu-id="c18a6-149">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="c18a6-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="c18a6-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="c18a6-150">activityDateTime</span></span>|<span data-ttu-id="c18a6-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c18a6-151">DateTimeOffset</span></span>|<span data-ttu-id="c18a6-152">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="c18a6-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="c18a6-153">activityType</span><span class="sxs-lookup"><span data-stu-id="c18a6-153">activityType</span></span>|<span data-ttu-id="c18a6-154">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-154">String</span></span>|<span data-ttu-id="c18a6-155">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="c18a6-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="c18a6-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="c18a6-156">activityOperationType</span></span>|<span data-ttu-id="c18a6-157">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-157">String</span></span>|<span data-ttu-id="c18a6-158">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="c18a6-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="c18a6-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="c18a6-159">activityResult</span></span>|<span data-ttu-id="c18a6-160">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-160">String</span></span>|<span data-ttu-id="c18a6-161">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="c18a6-161">The result of the activity.</span></span>|
|<span data-ttu-id="c18a6-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="c18a6-162">correlationId</span></span>|<span data-ttu-id="c18a6-163">Guid</span><span class="sxs-lookup"><span data-stu-id="c18a6-163">Guid</span></span>|<span data-ttu-id="c18a6-164">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="c18a6-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="c18a6-165">resources</span><span class="sxs-lookup"><span data-stu-id="c18a6-165">resources</span></span>|<span data-ttu-id="c18a6-166">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c18a6-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="c18a6-167">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="c18a6-167">Resources being modified.</span></span>|
|<span data-ttu-id="c18a6-168">category</span><span class="sxs-lookup"><span data-stu-id="c18a6-168">category</span></span>|<span data-ttu-id="c18a6-169">String</span><span class="sxs-lookup"><span data-stu-id="c18a6-169">String</span></span>|<span data-ttu-id="c18a6-170">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="c18a6-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c18a6-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c18a6-171">Relationships</span></span>
<span data-ttu-id="c18a6-172">なし</span><span class="sxs-lookup"><span data-stu-id="c18a6-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c18a6-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c18a6-173">JSON Representation</span></span>
<span data-ttu-id="c18a6-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c18a6-174">Here is a JSON representation of the resource.</span></span>
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



