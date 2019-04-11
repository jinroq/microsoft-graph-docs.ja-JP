---
title: auditEvent リソース タイプ
description: 監査イベントのプロパティが含まれるクラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c6004db55f25f92261de8fd6ee2a5418928e9a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798524"
---
# <a name="auditevent-resource-type"></a><span data-ttu-id="0c18d-103">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0c18d-103">auditEvent resource type</span></span>

> <span data-ttu-id="0c18d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c18d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c18d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c18d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c18d-106">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="0c18d-106">A class containing the properties for Audit Event.</span></span>

## <a name="methods"></a><span data-ttu-id="0c18d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c18d-107">Methods</span></span>
|<span data-ttu-id="0c18d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0c18d-108">Method</span></span>|<span data-ttu-id="0c18d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0c18d-109">Return Type</span></span>|<span data-ttu-id="0c18d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c18d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0c18d-111">auditEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="0c18d-111">List auditEvents</span></span>](../api/intune-auditing-auditevent-list.md)|<span data-ttu-id="0c18d-112">[auditEvent](../resources/intune-auditing-auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c18d-112">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="0c18d-113">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0c18d-113">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>|
|[<span data-ttu-id="0c18d-114">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="0c18d-114">Get auditEvent</span></span>](../api/intune-auditing-auditevent-get.md)|[<span data-ttu-id="0c18d-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="0c18d-115">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="0c18d-116">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0c18d-116">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="0c18d-117">auditEvent の作成</span><span class="sxs-lookup"><span data-stu-id="0c18d-117">Create auditEvent</span></span>](../api/intune-auditing-auditevent-create.md)|[<span data-ttu-id="0c18d-118">auditEvent</span><span class="sxs-lookup"><span data-stu-id="0c18d-118">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="0c18d-119">新しい [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c18d-119">Create a new [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="0c18d-120">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="0c18d-120">Delete auditEvent</span></span>](../api/intune-auditing-auditevent-delete.md)|<span data-ttu-id="0c18d-121">なし</span><span class="sxs-lookup"><span data-stu-id="0c18d-121">None</span></span>|<span data-ttu-id="0c18d-122">[auditEvent](../resources/intune-auditing-auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0c18d-122">Deletes a [auditEvent](../resources/intune-auditing-auditevent.md).</span></span>|
|[<span data-ttu-id="0c18d-123">auditEvent の更新</span><span class="sxs-lookup"><span data-stu-id="0c18d-123">Update auditEvent</span></span>](../api/intune-auditing-auditevent-update.md)|[<span data-ttu-id="0c18d-124">auditEvent</span><span class="sxs-lookup"><span data-stu-id="0c18d-124">auditEvent</span></span>](../resources/intune-auditing-auditevent.md)|<span data-ttu-id="0c18d-125">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0c18d-125">Update the properties of a [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>|
|[<span data-ttu-id="0c18d-126">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="0c18d-126">getAuditCategories function</span></span>](../api/intune-auditing-auditevent-getauditcategories.md)|<span data-ttu-id="0c18d-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0c18d-127">String collection</span></span>|<span data-ttu-id="0c18d-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c18d-128">Not yet documented</span></span>|
|[<span data-ttu-id="0c18d-129">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="0c18d-129">getAuditActivityTypes function</span></span>](../api/intune-auditing-auditevent-getauditactivitytypes.md)|<span data-ttu-id="0c18d-130">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0c18d-130">String collection</span></span>|<span data-ttu-id="0c18d-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0c18d-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0c18d-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c18d-132">Properties</span></span>
|<span data-ttu-id="0c18d-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c18d-133">Property</span></span>|<span data-ttu-id="0c18d-134">型</span><span class="sxs-lookup"><span data-stu-id="0c18d-134">Type</span></span>|<span data-ttu-id="0c18d-135">説明</span><span class="sxs-lookup"><span data-stu-id="0c18d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c18d-136">id</span><span class="sxs-lookup"><span data-stu-id="0c18d-136">id</span></span>|<span data-ttu-id="0c18d-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0c18d-137">String</span></span>|<span data-ttu-id="0c18d-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0c18d-138">Key of the entity.</span></span>|
|<span data-ttu-id="0c18d-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0c18d-139">displayName</span></span>|<span data-ttu-id="0c18d-140">String</span><span class="sxs-lookup"><span data-stu-id="0c18d-140">String</span></span>|<span data-ttu-id="0c18d-141">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="0c18d-141">Event display name.</span></span>|
|<span data-ttu-id="0c18d-142">componentName</span><span class="sxs-lookup"><span data-stu-id="0c18d-142">componentName</span></span>|<span data-ttu-id="0c18d-143">文字列</span><span class="sxs-lookup"><span data-stu-id="0c18d-143">String</span></span>|<span data-ttu-id="0c18d-144">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="0c18d-144">Component name.</span></span>|
|<span data-ttu-id="0c18d-145">actor</span><span class="sxs-lookup"><span data-stu-id="0c18d-145">actor</span></span>|[<span data-ttu-id="0c18d-146">auditActor</span><span class="sxs-lookup"><span data-stu-id="0c18d-146">auditActor</span></span>](../resources/intune-auditing-auditactor.md)|<span data-ttu-id="0c18d-147">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="0c18d-147">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="0c18d-148">activity</span><span class="sxs-lookup"><span data-stu-id="0c18d-148">activity</span></span>|<span data-ttu-id="0c18d-149">文字列</span><span class="sxs-lookup"><span data-stu-id="0c18d-149">String</span></span>|<span data-ttu-id="0c18d-150">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="0c18d-150">Friendly name of the activity.</span></span>|
|<span data-ttu-id="0c18d-151">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="0c18d-151">activityDateTime</span></span>|<span data-ttu-id="0c18d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c18d-152">DateTimeOffset</span></span>|<span data-ttu-id="0c18d-153">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="0c18d-153">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="0c18d-154">activityType</span><span class="sxs-lookup"><span data-stu-id="0c18d-154">activityType</span></span>|<span data-ttu-id="0c18d-155">文字列</span><span class="sxs-lookup"><span data-stu-id="0c18d-155">String</span></span>|<span data-ttu-id="0c18d-156">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="0c18d-156">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="0c18d-157">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="0c18d-157">activityOperationType</span></span>|<span data-ttu-id="0c18d-158">文字列</span><span class="sxs-lookup"><span data-stu-id="0c18d-158">String</span></span>|<span data-ttu-id="0c18d-159">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="0c18d-159">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="0c18d-160">activityResult</span><span class="sxs-lookup"><span data-stu-id="0c18d-160">activityResult</span></span>|<span data-ttu-id="0c18d-161">String</span><span class="sxs-lookup"><span data-stu-id="0c18d-161">String</span></span>|<span data-ttu-id="0c18d-162">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="0c18d-162">The result of the activity.</span></span>|
|<span data-ttu-id="0c18d-163">correlationId</span><span class="sxs-lookup"><span data-stu-id="0c18d-163">correlationId</span></span>|<span data-ttu-id="0c18d-164">Guid</span><span class="sxs-lookup"><span data-stu-id="0c18d-164">Guid</span></span>|<span data-ttu-id="0c18d-165">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="0c18d-165">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="0c18d-166">resources</span><span class="sxs-lookup"><span data-stu-id="0c18d-166">resources</span></span>|<span data-ttu-id="0c18d-167">[auditResource](../resources/intune-auditing-auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0c18d-167">[auditResource](../resources/intune-auditing-auditresource.md) collection</span></span>|<span data-ttu-id="0c18d-168">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="0c18d-168">Resources being modified.</span></span>|
|<span data-ttu-id="0c18d-169">category</span><span class="sxs-lookup"><span data-stu-id="0c18d-169">category</span></span>|<span data-ttu-id="0c18d-170">String</span><span class="sxs-lookup"><span data-stu-id="0c18d-170">String</span></span>|<span data-ttu-id="0c18d-171">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="0c18d-171">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c18d-172">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c18d-172">Relationships</span></span>
<span data-ttu-id="0c18d-173">なし</span><span class="sxs-lookup"><span data-stu-id="0c18d-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c18d-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c18d-174">JSON Representation</span></span>
<span data-ttu-id="0c18d-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c18d-175">Here is a JSON representation of the resource.</span></span>
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





