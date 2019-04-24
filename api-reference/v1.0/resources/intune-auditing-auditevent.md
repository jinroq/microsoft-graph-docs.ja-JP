---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fa86724affd94d3eaaf6584ce3e70dc8266a5f00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584811"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="a7772-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a7772-103">auditEvent resource type</span></span>

> <span data-ttu-id="a7772-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a7772-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7772-105">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="a7772-105">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="a7772-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7772-106">Methods</span></span>
|<span data-ttu-id="a7772-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a7772-107">Method</span></span>|<span data-ttu-id="a7772-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a7772-108">Return Type</span></span>|<span data-ttu-id="a7772-109">説明</span><span class="sxs-lookup"><span data-stu-id="a7772-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a7772-110">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="a7772-110">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="a7772-111">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7772-111">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="a7772-112">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a7772-112">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="a7772-113">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-113">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="a7772-114">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-114">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a7772-115">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a7772-115">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a7772-116">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-116">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="a7772-117">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-117">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a7772-118">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a7772-118">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a7772-119">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-119">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="a7772-120">なし</span><span class="sxs-lookup"><span data-stu-id="a7772-120">None</span></span>|<span data-ttu-id="a7772-121">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a7772-121">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="a7772-122">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-122">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="a7772-123">auditEvent</span><span class="sxs-lookup"><span data-stu-id="a7772-123">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="a7772-124">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a7772-124">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="a7772-125">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="a7772-125">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="a7772-126">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7772-126">String collection</span></span>|<span data-ttu-id="a7772-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a7772-127">Not yet documented</span></span>|
|[<span data-ttu-id="a7772-128">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="a7772-128">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="a7772-129">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a7772-129">String collection</span></span>|<span data-ttu-id="a7772-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a7772-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a7772-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7772-131">Properties</span></span>
|<span data-ttu-id="a7772-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a7772-132">Property</span></span>|<span data-ttu-id="a7772-133">型</span><span class="sxs-lookup"><span data-stu-id="a7772-133">Type</span></span>|<span data-ttu-id="a7772-134">説明</span><span class="sxs-lookup"><span data-stu-id="a7772-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7772-135">id</span><span class="sxs-lookup"><span data-stu-id="a7772-135">id</span></span>|<span data-ttu-id="a7772-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a7772-136">String</span></span>|<span data-ttu-id="a7772-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a7772-137">Key of the entity.</span></span>|
|<span data-ttu-id="a7772-138">displayName</span><span class="sxs-lookup"><span data-stu-id="a7772-138">displayName</span></span>|<span data-ttu-id="a7772-139">String</span><span class="sxs-lookup"><span data-stu-id="a7772-139">String</span></span>|<span data-ttu-id="a7772-140">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="a7772-140">Event display name.</span></span>|
|<span data-ttu-id="a7772-141">componentName</span><span class="sxs-lookup"><span data-stu-id="a7772-141">componentName</span></span>|<span data-ttu-id="a7772-142">String</span><span class="sxs-lookup"><span data-stu-id="a7772-142">String</span></span>|<span data-ttu-id="a7772-143">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="a7772-143">Component name.</span></span>|
|<span data-ttu-id="a7772-144">actor</span><span class="sxs-lookup"><span data-stu-id="a7772-144">actor</span></span>|[<span data-ttu-id="a7772-145">auditActor</span><span class="sxs-lookup"><span data-stu-id="a7772-145">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="a7772-146">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="a7772-146">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="a7772-147">activity</span><span class="sxs-lookup"><span data-stu-id="a7772-147">activity</span></span>|<span data-ttu-id="a7772-148">String</span><span class="sxs-lookup"><span data-stu-id="a7772-148">String</span></span>|<span data-ttu-id="a7772-149">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="a7772-149">Friendly name of the activity.</span></span>|
|<span data-ttu-id="a7772-150">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="a7772-150">activityDateTime</span></span>|<span data-ttu-id="a7772-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a7772-151">DateTimeOffset</span></span>|<span data-ttu-id="a7772-152">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="a7772-152">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="a7772-153">activityType</span><span class="sxs-lookup"><span data-stu-id="a7772-153">activityType</span></span>|<span data-ttu-id="a7772-154">String</span><span class="sxs-lookup"><span data-stu-id="a7772-154">String</span></span>|<span data-ttu-id="a7772-155">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="a7772-155">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="a7772-156">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="a7772-156">activityOperationType</span></span>|<span data-ttu-id="a7772-157">String</span><span class="sxs-lookup"><span data-stu-id="a7772-157">String</span></span>|<span data-ttu-id="a7772-158">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="a7772-158">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="a7772-159">activityResult</span><span class="sxs-lookup"><span data-stu-id="a7772-159">activityResult</span></span>|<span data-ttu-id="a7772-160">String</span><span class="sxs-lookup"><span data-stu-id="a7772-160">String</span></span>|<span data-ttu-id="a7772-161">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="a7772-161">The result of the activity.</span></span>|
|<span data-ttu-id="a7772-162">correlationId</span><span class="sxs-lookup"><span data-stu-id="a7772-162">correlationId</span></span>|<span data-ttu-id="a7772-163">Guid</span><span class="sxs-lookup"><span data-stu-id="a7772-163">Guid</span></span>|<span data-ttu-id="a7772-164">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="a7772-164">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="a7772-165">resources</span><span class="sxs-lookup"><span data-stu-id="a7772-165">resources</span></span>|<span data-ttu-id="a7772-166">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a7772-166">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="a7772-167">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="a7772-167">Resources being modified.</span></span>|
|<span data-ttu-id="a7772-168">category</span><span class="sxs-lookup"><span data-stu-id="a7772-168">category</span></span>|<span data-ttu-id="a7772-169">String</span><span class="sxs-lookup"><span data-stu-id="a7772-169">String</span></span>|<span data-ttu-id="a7772-170">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="a7772-170">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7772-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a7772-171">Relationships</span></span>
<span data-ttu-id="a7772-172">なし</span><span class="sxs-lookup"><span data-stu-id="a7772-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7772-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a7772-173">JSON Representation</span></span>
<span data-ttu-id="a7772-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a7772-174">Here is a JSON representation of the resource.</span></span>
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



