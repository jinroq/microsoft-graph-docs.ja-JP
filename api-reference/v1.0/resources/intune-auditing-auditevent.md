---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 445ed776de946c3b557e387164f81dcf4ee16ab2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940968"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="3e960-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="3e960-103">auditEvent resource type</span></span>

> <span data-ttu-id="3e960-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3e960-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e960-105">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="3e960-105">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="3e960-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="3e960-106">Methods</span></span>
|<span data-ttu-id="3e960-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3e960-107">Method</span></span>|<span data-ttu-id="3e960-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3e960-108">Return Type</span></span>|<span data-ttu-id="3e960-109">説明</span><span class="sxs-lookup"><span data-stu-id="3e960-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3e960-110">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="3e960-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="3e960-111">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3e960-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="3e960-112">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3e960-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="3e960-113">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="3e960-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="3e960-115">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3e960-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="3e960-116">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="3e960-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="3e960-118">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3e960-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="3e960-119">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="3e960-120">なし</span><span class="sxs-lookup"><span data-stu-id="3e960-120">None</span></span>|<span data-ttu-id="3e960-121">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3e960-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="3e960-122">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="3e960-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="3e960-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="3e960-124">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3e960-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="3e960-125">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="3e960-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="3e960-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3e960-126">String collection</span></span>|<span data-ttu-id="3e960-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3e960-127">Not yet documented</span></span>|
|[<span data-ttu-id="3e960-128">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="3e960-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="3e960-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3e960-129">String collection</span></span>|<span data-ttu-id="3e960-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3e960-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3e960-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e960-131">Properties</span></span>
|<span data-ttu-id="3e960-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e960-132">Property</span></span>|<span data-ttu-id="3e960-133">型</span><span class="sxs-lookup"><span data-stu-id="3e960-133">Type</span></span>|<span data-ttu-id="3e960-134">説明</span><span class="sxs-lookup"><span data-stu-id="3e960-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e960-135">ID</span><span class="sxs-lookup"><span data-stu-id="3e960-135">id</span></span>|<span data-ttu-id="3e960-136">String</span><span class="sxs-lookup"><span data-stu-id="3e960-136">String</span></span>|<span data-ttu-id="3e960-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3e960-137">Key of the entity.</span></span>|
|<span data-ttu-id="3e960-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3e960-138">displayName</span></span>|<span data-ttu-id="3e960-139">String</span><span class="sxs-lookup"><span data-stu-id="3e960-139">String</span></span>|<span data-ttu-id="3e960-140">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="3e960-140">Event display name.</span></span>|
|<span data-ttu-id="3e960-141">componentName</span><span class="sxs-lookup"><span data-stu-id="3e960-141">componentName</span></span>|<span data-ttu-id="3e960-142">String</span><span class="sxs-lookup"><span data-stu-id="3e960-142">String</span></span>|<span data-ttu-id="3e960-143">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="3e960-143">Component name.</span></span>|
|<span data-ttu-id="3e960-144">actor</span><span class="sxs-lookup"><span data-stu-id="3e960-144">actor</span></span>|[<span data-ttu-id="3e960-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="3e960-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="3e960-146">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="3e960-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="3e960-147">activity</span><span class="sxs-lookup"><span data-stu-id="3e960-147">activity</span></span>|<span data-ttu-id="3e960-148">String</span><span class="sxs-lookup"><span data-stu-id="3e960-148">String</span></span>|<span data-ttu-id="3e960-149">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="3e960-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="3e960-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="3e960-150">activityDateTime</span></span>|<span data-ttu-id="3e960-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e960-151">DateTimeOffset</span></span>|<span data-ttu-id="3e960-152">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="3e960-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="3e960-153">activityType</span><span class="sxs-lookup"><span data-stu-id="3e960-153">activityType</span></span>|<span data-ttu-id="3e960-154">String</span><span class="sxs-lookup"><span data-stu-id="3e960-154">String</span></span>|<span data-ttu-id="3e960-155">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="3e960-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="3e960-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="3e960-156">activityOperationType</span></span>|<span data-ttu-id="3e960-157">String</span><span class="sxs-lookup"><span data-stu-id="3e960-157">String</span></span>|<span data-ttu-id="3e960-158">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="3e960-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="3e960-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="3e960-159">activityResult</span></span>|<span data-ttu-id="3e960-160">String</span><span class="sxs-lookup"><span data-stu-id="3e960-160">String</span></span>|<span data-ttu-id="3e960-161">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="3e960-161">The result of the activity.</span></span>|
|<span data-ttu-id="3e960-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="3e960-162">correlationId</span></span>|<span data-ttu-id="3e960-163">Guid</span><span class="sxs-lookup"><span data-stu-id="3e960-163">Guid</span></span>|<span data-ttu-id="3e960-164">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="3e960-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="3e960-165">resources</span><span class="sxs-lookup"><span data-stu-id="3e960-165">resources</span></span>|<span data-ttu-id="3e960-166">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3e960-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="3e960-167">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="3e960-167">Resources being modified.</span></span>|
|<span data-ttu-id="3e960-168">category</span><span class="sxs-lookup"><span data-stu-id="3e960-168">category</span></span>|<span data-ttu-id="3e960-169">String</span><span class="sxs-lookup"><span data-stu-id="3e960-169">String</span></span>|<span data-ttu-id="3e960-170">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="3e960-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e960-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3e960-171">Relationships</span></span>
<span data-ttu-id="3e960-172">なし</span><span class="sxs-lookup"><span data-stu-id="3e960-172">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e960-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e960-173">JSON Representation</span></span>
<span data-ttu-id="3e960-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e960-174">Here is a JSON representation of the resource.</span></span>
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



