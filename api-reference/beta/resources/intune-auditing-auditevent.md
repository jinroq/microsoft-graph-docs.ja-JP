---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
ms.openlocfilehash: 99fbcfb07f08d10b20d8d57d0b16bc6d020f9e09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354006"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="91afa-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="91afa-103">auditEvent resource type</span></span>

> <span data-ttu-id="91afa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="91afa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91afa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91afa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91afa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="91afa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91afa-107">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="91afa-107">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="91afa-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="91afa-108">Methods</span></span>
|<span data-ttu-id="91afa-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="91afa-109">Method</span></span>|<span data-ttu-id="91afa-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="91afa-110">Return Type</span></span>|<span data-ttu-id="91afa-111">説明</span><span class="sxs-lookup"><span data-stu-id="91afa-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="91afa-112">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="91afa-112">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="91afa-113">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91afa-113">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="91afa-114">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="91afa-114">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="91afa-115">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-115">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="91afa-116">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-116">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91afa-117">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="91afa-117">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91afa-118">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-118">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="91afa-119">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-119">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91afa-120">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91afa-120">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91afa-121">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-121">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="91afa-122">なし</span><span class="sxs-lookup"><span data-stu-id="91afa-122">None</span></span>|<span data-ttu-id="91afa-123">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="91afa-123">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="91afa-124">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-124">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="91afa-125">auditEvent</span><span class="sxs-lookup"><span data-stu-id="91afa-125">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="91afa-126">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="91afa-126">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="91afa-127">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="91afa-127">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="91afa-128">String コレクション</span><span class="sxs-lookup"><span data-stu-id="91afa-128">String collection</span></span>|<span data-ttu-id="91afa-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="91afa-129">Not yet documented</span></span>|
|[<span data-ttu-id="91afa-130">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="91afa-130">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="91afa-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="91afa-131">String collection</span></span>|<span data-ttu-id="91afa-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="91afa-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="91afa-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91afa-133">Properties</span></span>
|<span data-ttu-id="91afa-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91afa-134">Property</span></span>|<span data-ttu-id="91afa-135">種類</span><span class="sxs-lookup"><span data-stu-id="91afa-135">Type</span></span>|<span data-ttu-id="91afa-136">説明</span><span class="sxs-lookup"><span data-stu-id="91afa-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91afa-137">ID</span><span class="sxs-lookup"><span data-stu-id="91afa-137">id</span></span>|<span data-ttu-id="91afa-138">String</span><span class="sxs-lookup"><span data-stu-id="91afa-138">String</span></span>|<span data-ttu-id="91afa-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="91afa-139">Key of the entity.</span></span>|
|<span data-ttu-id="91afa-140">displayName</span><span class="sxs-lookup"><span data-stu-id="91afa-140">displayName</span></span>|<span data-ttu-id="91afa-141">String</span><span class="sxs-lookup"><span data-stu-id="91afa-141">String</span></span>|<span data-ttu-id="91afa-142">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="91afa-142">Event display name.</span></span>|
|<span data-ttu-id="91afa-143">componentName</span><span class="sxs-lookup"><span data-stu-id="91afa-143">componentName</span></span>|<span data-ttu-id="91afa-144">String</span><span class="sxs-lookup"><span data-stu-id="91afa-144">String</span></span>|<span data-ttu-id="91afa-145">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="91afa-145">Component name.</span></span>|
|<span data-ttu-id="91afa-146">actor</span><span class="sxs-lookup"><span data-stu-id="91afa-146">actor</span></span>|[<span data-ttu-id="91afa-147">auditActor</span><span class="sxs-lookup"><span data-stu-id="91afa-147">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="91afa-148">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="91afa-148">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="91afa-149">activity</span><span class="sxs-lookup"><span data-stu-id="91afa-149">activity</span></span>|<span data-ttu-id="91afa-150">String</span><span class="sxs-lookup"><span data-stu-id="91afa-150">String</span></span>|<span data-ttu-id="91afa-151">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="91afa-151">Friendly name of the activity.</span></span>|
|<span data-ttu-id="91afa-152">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="91afa-152">activityDateTime</span></span>|<span data-ttu-id="91afa-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91afa-153">DateTimeOffset</span></span>|<span data-ttu-id="91afa-154">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="91afa-154">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="91afa-155">activityType</span><span class="sxs-lookup"><span data-stu-id="91afa-155">activityType</span></span>|<span data-ttu-id="91afa-156">String</span><span class="sxs-lookup"><span data-stu-id="91afa-156">String</span></span>|<span data-ttu-id="91afa-157">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="91afa-157">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="91afa-158">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="91afa-158">activityOperationType</span></span>|<span data-ttu-id="91afa-159">String</span><span class="sxs-lookup"><span data-stu-id="91afa-159">String</span></span>|<span data-ttu-id="91afa-160">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="91afa-160">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="91afa-161">activityResult</span><span class="sxs-lookup"><span data-stu-id="91afa-161">activityResult</span></span>|<span data-ttu-id="91afa-162">String</span><span class="sxs-lookup"><span data-stu-id="91afa-162">String</span></span>|<span data-ttu-id="91afa-163">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="91afa-163">The result of the activity.</span></span>|
|<span data-ttu-id="91afa-164">correlationId</span><span class="sxs-lookup"><span data-stu-id="91afa-164">correlationId</span></span>|<span data-ttu-id="91afa-165">Guid</span><span class="sxs-lookup"><span data-stu-id="91afa-165">Guid</span></span>|<span data-ttu-id="91afa-166">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="91afa-166">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="91afa-167">resources</span><span class="sxs-lookup"><span data-stu-id="91afa-167">resources</span></span>|<span data-ttu-id="91afa-168">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91afa-168">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="91afa-169">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="91afa-169">Resources being modified.</span></span>|
|<span data-ttu-id="91afa-170">category</span><span class="sxs-lookup"><span data-stu-id="91afa-170">category</span></span>|<span data-ttu-id="91afa-171">String</span><span class="sxs-lookup"><span data-stu-id="91afa-171">String</span></span>|<span data-ttu-id="91afa-172">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="91afa-172">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91afa-173">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="91afa-173">Relationships</span></span>
<span data-ttu-id="91afa-174">なし</span><span class="sxs-lookup"><span data-stu-id="91afa-174">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91afa-175">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="91afa-175">JSON Representation</span></span>
<span data-ttu-id="91afa-176">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="91afa-176">Here is a JSON representation of the resource.</span></span>
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





