---
title: devicemanagementintentuserstate リソースの種類
description: 目的のユーザー状態を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5dddc3585d6a99f8ad1613a01a796c34128c5d4e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802927"
---
# <a name="devicemanagementintentuserstate-resource-type"></a><span data-ttu-id="45a37-103">devicemanagementintentuserstate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45a37-103">deviceManagementIntentUserState resource type</span></span>

> <span data-ttu-id="45a37-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45a37-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45a37-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45a37-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45a37-106">目的のユーザー状態を表すエンティティ</span><span class="sxs-lookup"><span data-stu-id="45a37-106">Entity that represents user state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="45a37-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="45a37-107">Methods</span></span>
|<span data-ttu-id="45a37-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="45a37-108">Method</span></span>|<span data-ttu-id="45a37-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="45a37-109">Return Type</span></span>|<span data-ttu-id="45a37-110">説明</span><span class="sxs-lookup"><span data-stu-id="45a37-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45a37-111">devicemanagementintentuserstates のリスト</span><span class="sxs-lookup"><span data-stu-id="45a37-111">List deviceManagementIntentUserStates</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|<span data-ttu-id="45a37-112">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="45a37-112">[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) collection</span></span>|<span data-ttu-id="45a37-113">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="45a37-113">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>|
|[<span data-ttu-id="45a37-114">devicemanagementintentuserstate の取得</span><span class="sxs-lookup"><span data-stu-id="45a37-114">Get deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[<span data-ttu-id="45a37-115">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="45a37-115">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="45a37-116">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="45a37-116">Read properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="45a37-117">devicemanagementintentuserstate の作成</span><span class="sxs-lookup"><span data-stu-id="45a37-117">Create deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[<span data-ttu-id="45a37-118">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="45a37-118">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="45a37-119">新しい[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45a37-119">Create a new [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|
|[<span data-ttu-id="45a37-120">devicemanagementintentuserstate の削除</span><span class="sxs-lookup"><span data-stu-id="45a37-120">Delete deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|<span data-ttu-id="45a37-121">なし</span><span class="sxs-lookup"><span data-stu-id="45a37-121">None</span></span>|<span data-ttu-id="45a37-122">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="45a37-122">Deletes a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md).</span></span>|
|[<span data-ttu-id="45a37-123">devicemanagementintentuserstate の更新</span><span class="sxs-lookup"><span data-stu-id="45a37-123">Update deviceManagementIntentUserState</span></span>](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[<span data-ttu-id="45a37-124">deviceManagementIntentUserState</span><span class="sxs-lookup"><span data-stu-id="45a37-124">deviceManagementIntentUserState</span></span>](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|<span data-ttu-id="45a37-125">[devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45a37-125">Update the properties of a [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="45a37-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45a37-126">Properties</span></span>
|<span data-ttu-id="45a37-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45a37-127">Property</span></span>|<span data-ttu-id="45a37-128">型</span><span class="sxs-lookup"><span data-stu-id="45a37-128">Type</span></span>|<span data-ttu-id="45a37-129">説明</span><span class="sxs-lookup"><span data-stu-id="45a37-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45a37-130">id</span><span class="sxs-lookup"><span data-stu-id="45a37-130">id</span></span>|<span data-ttu-id="45a37-131">String</span><span class="sxs-lookup"><span data-stu-id="45a37-131">String</span></span>|<span data-ttu-id="45a37-132">ID</span><span class="sxs-lookup"><span data-stu-id="45a37-132">The ID</span></span>|
|<span data-ttu-id="45a37-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="45a37-133">userPrincipalName</span></span>|<span data-ttu-id="45a37-134">String</span><span class="sxs-lookup"><span data-stu-id="45a37-134">String</span></span>|<span data-ttu-id="45a37-135">デバイスで報告されているユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="45a37-135">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="45a37-136">userName</span><span class="sxs-lookup"><span data-stu-id="45a37-136">userName</span></span>|<span data-ttu-id="45a37-137">String</span><span class="sxs-lookup"><span data-stu-id="45a37-137">String</span></span>|<span data-ttu-id="45a37-138">デバイスで報告されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="45a37-138">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="45a37-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="45a37-139">deviceCount</span></span>|<span data-ttu-id="45a37-140">Int32</span><span class="sxs-lookup"><span data-stu-id="45a37-140">Int32</span></span>|<span data-ttu-id="45a37-141">目的のためにユーザーに属しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="45a37-141">Count of Devices that belongs to a user for an intent</span></span>|
|<span data-ttu-id="45a37-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="45a37-142">lastReportedDateTime</span></span>|<span data-ttu-id="45a37-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="45a37-143">DateTimeOffset</span></span>|<span data-ttu-id="45a37-144">インテントレポートの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="45a37-144">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="45a37-145">state</span><span class="sxs-lookup"><span data-stu-id="45a37-145">state</span></span>|[<span data-ttu-id="45a37-146">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="45a37-146">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="45a37-147">目的のユーザー状態。</span><span class="sxs-lookup"><span data-stu-id="45a37-147">User state for an intent.</span></span> <span data-ttu-id="45a37-148">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="45a37-148">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45a37-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45a37-149">Relationships</span></span>
<span data-ttu-id="45a37-150">なし</span><span class="sxs-lookup"><span data-stu-id="45a37-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45a37-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45a37-151">JSON Representation</span></span>
<span data-ttu-id="45a37-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45a37-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```





