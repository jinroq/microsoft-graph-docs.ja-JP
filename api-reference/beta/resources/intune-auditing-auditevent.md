---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fd9971b5b6ddce9b3a826ff569d1925ef9cff97
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153677"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="4999c-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4999c-103">auditEvent resource type</span></span>

> <span data-ttu-id="4999c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4999c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4999c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4999c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4999c-106">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="4999c-106">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="4999c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4999c-107">Methods</span></span>
|<span data-ttu-id="4999c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4999c-108">Method</span></span>|<span data-ttu-id="4999c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4999c-109">Return Type</span></span>|<span data-ttu-id="4999c-110">説明</span><span class="sxs-lookup"><span data-stu-id="4999c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4999c-111">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="4999c-111">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="4999c-112">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4999c-112">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="4999c-113">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4999c-113">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="4999c-114">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-114">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="4999c-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-115">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="4999c-116">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4999c-116">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="4999c-117">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-117">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="4999c-118">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-118">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="4999c-119">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4999c-119">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="4999c-120">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-120">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="4999c-121">なし</span><span class="sxs-lookup"><span data-stu-id="4999c-121">None</span></span>|<span data-ttu-id="4999c-122">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4999c-122">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="4999c-123">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-123">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="4999c-124">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4999c-124">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="4999c-125">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4999c-125">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="4999c-126">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="4999c-126">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="4999c-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4999c-127">String collection</span></span>|<span data-ttu-id="4999c-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4999c-128">Not yet documented</span></span>|
|[<span data-ttu-id="4999c-129">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="4999c-129">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="4999c-130">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4999c-130">String collection</span></span>|<span data-ttu-id="4999c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4999c-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4999c-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4999c-132">Properties</span></span>
|<span data-ttu-id="4999c-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4999c-133">Property</span></span>|<span data-ttu-id="4999c-134">型</span><span class="sxs-lookup"><span data-stu-id="4999c-134">Type</span></span>|<span data-ttu-id="4999c-135">説明</span><span class="sxs-lookup"><span data-stu-id="4999c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4999c-136">id</span><span class="sxs-lookup"><span data-stu-id="4999c-136">id</span></span>|<span data-ttu-id="4999c-137">文字列</span><span class="sxs-lookup"><span data-stu-id="4999c-137">String</span></span>|<span data-ttu-id="4999c-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4999c-138">Key of the entity.</span></span>|
|<span data-ttu-id="4999c-139">displayName</span><span class="sxs-lookup"><span data-stu-id="4999c-139">displayName</span></span>|<span data-ttu-id="4999c-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4999c-140">String</span></span>|<span data-ttu-id="4999c-141">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="4999c-141">Event display name.</span></span>|
|<span data-ttu-id="4999c-142">componentName</span><span class="sxs-lookup"><span data-stu-id="4999c-142">componentName</span></span>|<span data-ttu-id="4999c-143">String</span><span class="sxs-lookup"><span data-stu-id="4999c-143">String</span></span>|<span data-ttu-id="4999c-144">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="4999c-144">Component name.</span></span>|
|<span data-ttu-id="4999c-145">actor</span><span class="sxs-lookup"><span data-stu-id="4999c-145">actor</span></span>|[<span data-ttu-id="4999c-146">auditActor</span><span class="sxs-lookup"><span data-stu-id="4999c-146">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="4999c-147">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="4999c-147">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="4999c-148">activity</span><span class="sxs-lookup"><span data-stu-id="4999c-148">activity</span></span>|<span data-ttu-id="4999c-149">String</span><span class="sxs-lookup"><span data-stu-id="4999c-149">String</span></span>|<span data-ttu-id="4999c-150">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="4999c-150">Friendly name of the activity.</span></span>|
|<span data-ttu-id="4999c-151">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="4999c-151">activityDateTime</span></span>|<span data-ttu-id="4999c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4999c-152">DateTimeOffset</span></span>|<span data-ttu-id="4999c-153">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="4999c-153">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="4999c-154">activityType</span><span class="sxs-lookup"><span data-stu-id="4999c-154">activityType</span></span>|<span data-ttu-id="4999c-155">String</span><span class="sxs-lookup"><span data-stu-id="4999c-155">String</span></span>|<span data-ttu-id="4999c-156">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="4999c-156">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="4999c-157">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="4999c-157">activityOperationType</span></span>|<span data-ttu-id="4999c-158">String</span><span class="sxs-lookup"><span data-stu-id="4999c-158">String</span></span>|<span data-ttu-id="4999c-159">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="4999c-159">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="4999c-160">activityResult</span><span class="sxs-lookup"><span data-stu-id="4999c-160">activityResult</span></span>|<span data-ttu-id="4999c-161">String</span><span class="sxs-lookup"><span data-stu-id="4999c-161">String</span></span>|<span data-ttu-id="4999c-162">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="4999c-162">The result of the activity.</span></span>|
|<span data-ttu-id="4999c-163">correlationId</span><span class="sxs-lookup"><span data-stu-id="4999c-163">correlationId</span></span>|<span data-ttu-id="4999c-164">Guid</span><span class="sxs-lookup"><span data-stu-id="4999c-164">Guid</span></span>|<span data-ttu-id="4999c-165">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="4999c-165">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="4999c-166">resources</span><span class="sxs-lookup"><span data-stu-id="4999c-166">resources</span></span>|<span data-ttu-id="4999c-167">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4999c-167">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="4999c-168">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="4999c-168">Resources being modified.</span></span>|
|<span data-ttu-id="4999c-169">category</span><span class="sxs-lookup"><span data-stu-id="4999c-169">category</span></span>|<span data-ttu-id="4999c-170">String</span><span class="sxs-lookup"><span data-stu-id="4999c-170">String</span></span>|<span data-ttu-id="4999c-171">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="4999c-171">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4999c-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4999c-172">Relationships</span></span>
<span data-ttu-id="4999c-173">なし</span><span class="sxs-lookup"><span data-stu-id="4999c-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4999c-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4999c-174">JSON Representation</span></span>
<span data-ttu-id="4999c-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4999c-175">Here is a JSON representation of the resource.</span></span>
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




