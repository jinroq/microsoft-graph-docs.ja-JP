---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa86724affd94d3eaaf6584ce3e70dc8266a5f00
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251630"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="e66df-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e66df-103">auditEvent resource type</span></span>

> <span data-ttu-id="e66df-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e66df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e66df-105">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="e66df-105">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="e66df-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e66df-106">Methods</span></span>
|<span data-ttu-id="e66df-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e66df-107">Method</span></span>|<span data-ttu-id="e66df-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e66df-108">Return Type</span></span>|<span data-ttu-id="e66df-109">説明</span><span class="sxs-lookup"><span data-stu-id="e66df-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e66df-110">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="e66df-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="e66df-111">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e66df-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="e66df-112">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e66df-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="e66df-113">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="e66df-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e66df-115">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e66df-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e66df-116">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="e66df-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e66df-118">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e66df-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e66df-119">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="e66df-120">なし</span><span class="sxs-lookup"><span data-stu-id="e66df-120">None</span></span>|<span data-ttu-id="e66df-121">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e66df-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="e66df-122">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="e66df-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="e66df-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="e66df-124">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e66df-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="e66df-125">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="e66df-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="e66df-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e66df-126">String collection</span></span>|<span data-ttu-id="e66df-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e66df-127">Not yet documented</span></span>|
|[<span data-ttu-id="e66df-128">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="e66df-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="e66df-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e66df-129">String collection</span></span>|<span data-ttu-id="e66df-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e66df-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e66df-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e66df-131">Properties</span></span>
|<span data-ttu-id="e66df-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e66df-132">Property</span></span>|<span data-ttu-id="e66df-133">型</span><span class="sxs-lookup"><span data-stu-id="e66df-133">Type</span></span>|<span data-ttu-id="e66df-134">説明</span><span class="sxs-lookup"><span data-stu-id="e66df-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e66df-135">id</span><span class="sxs-lookup"><span data-stu-id="e66df-135">id</span></span>|<span data-ttu-id="e66df-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e66df-136">String</span></span>|<span data-ttu-id="e66df-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e66df-137">Key of the entity.</span></span>|
|<span data-ttu-id="e66df-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e66df-138">displayName</span></span>|<span data-ttu-id="e66df-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e66df-139">String</span></span>|<span data-ttu-id="e66df-140">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="e66df-140">Event display name.</span></span>|
|<span data-ttu-id="e66df-141">componentName</span><span class="sxs-lookup"><span data-stu-id="e66df-141">componentName</span></span>|<span data-ttu-id="e66df-142">String</span><span class="sxs-lookup"><span data-stu-id="e66df-142">String</span></span>|<span data-ttu-id="e66df-143">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="e66df-143">Component name.</span></span>|
|<span data-ttu-id="e66df-144">actor</span><span class="sxs-lookup"><span data-stu-id="e66df-144">actor</span></span>|[<span data-ttu-id="e66df-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="e66df-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="e66df-146">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="e66df-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="e66df-147">activity</span><span class="sxs-lookup"><span data-stu-id="e66df-147">activity</span></span>|<span data-ttu-id="e66df-148">String</span><span class="sxs-lookup"><span data-stu-id="e66df-148">String</span></span>|<span data-ttu-id="e66df-149">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="e66df-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="e66df-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="e66df-150">activityDateTime</span></span>|<span data-ttu-id="e66df-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e66df-151">DateTimeOffset</span></span>|<span data-ttu-id="e66df-152">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="e66df-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="e66df-153">activityType</span><span class="sxs-lookup"><span data-stu-id="e66df-153">activityType</span></span>|<span data-ttu-id="e66df-154">String</span><span class="sxs-lookup"><span data-stu-id="e66df-154">String</span></span>|<span data-ttu-id="e66df-155">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="e66df-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="e66df-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="e66df-156">activityOperationType</span></span>|<span data-ttu-id="e66df-157">String</span><span class="sxs-lookup"><span data-stu-id="e66df-157">String</span></span>|<span data-ttu-id="e66df-158">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="e66df-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="e66df-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="e66df-159">activityResult</span></span>|<span data-ttu-id="e66df-160">String</span><span class="sxs-lookup"><span data-stu-id="e66df-160">String</span></span>|<span data-ttu-id="e66df-161">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="e66df-161">The result of the activity.</span></span>|
|<span data-ttu-id="e66df-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="e66df-162">correlationId</span></span>|<span data-ttu-id="e66df-163">Guid</span><span class="sxs-lookup"><span data-stu-id="e66df-163">Guid</span></span>|<span data-ttu-id="e66df-164">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="e66df-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="e66df-165">resources</span><span class="sxs-lookup"><span data-stu-id="e66df-165">resources</span></span>|<span data-ttu-id="e66df-166">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e66df-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="e66df-167">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="e66df-167">Resources being modified.</span></span>|
|<span data-ttu-id="e66df-168">category</span><span class="sxs-lookup"><span data-stu-id="e66df-168">category</span></span>|<span data-ttu-id="e66df-169">String</span><span class="sxs-lookup"><span data-stu-id="e66df-169">String</span></span>|<span data-ttu-id="e66df-170">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="e66df-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e66df-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e66df-171">Relationships</span></span>
<span data-ttu-id="e66df-172">なし</span><span class="sxs-lookup"><span data-stu-id="e66df-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e66df-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e66df-173">JSON Representation</span></span>
<span data-ttu-id="e66df-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e66df-174">Here is a JSON representation of the resource.</span></span>
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



