---
title: securityBaselineDeviceState リソースの種類
description: デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1fb6bd8ee8e474fdf96bc2c70f4db288571d795
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779798"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="0f42d-103">securityBaselineDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f42d-103">securityBaselineDeviceState resource type</span></span>

> <span data-ttu-id="0f42d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f42d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f42d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f42d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f42d-106">デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。</span><span class="sxs-lookup"><span data-stu-id="0f42d-106">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="0f42d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f42d-107">Methods</span></span>
|<span data-ttu-id="0f42d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f42d-108">Method</span></span>|<span data-ttu-id="0f42d-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0f42d-109">Return Type</span></span>|<span data-ttu-id="0f42d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0f42d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0f42d-111">リスト securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="0f42d-111">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="0f42d-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0f42d-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="0f42d-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0f42d-113">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="0f42d-114">securityBaselineDeviceState を取得する</span><span class="sxs-lookup"><span data-stu-id="0f42d-114">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="0f42d-115">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="0f42d-115">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="0f42d-116">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0f42d-116">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="0f42d-117">securityBaselineDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="0f42d-117">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="0f42d-118">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="0f42d-118">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="0f42d-119">新しい[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f42d-119">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="0f42d-120">securityBaselineDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="0f42d-120">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="0f42d-121">なし</span><span class="sxs-lookup"><span data-stu-id="0f42d-121">None</span></span>|<span data-ttu-id="0f42d-122">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="0f42d-122">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="0f42d-123">securityBaselineDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="0f42d-123">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="0f42d-124">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="0f42d-124">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="0f42d-125">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f42d-125">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0f42d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f42d-126">Properties</span></span>
|<span data-ttu-id="0f42d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f42d-127">Property</span></span>|<span data-ttu-id="0f42d-128">型</span><span class="sxs-lookup"><span data-stu-id="0f42d-128">Type</span></span>|<span data-ttu-id="0f42d-129">説明</span><span class="sxs-lookup"><span data-stu-id="0f42d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f42d-130">id</span><span class="sxs-lookup"><span data-stu-id="0f42d-130">id</span></span>|<span data-ttu-id="0f42d-131">String</span><span class="sxs-lookup"><span data-stu-id="0f42d-131">String</span></span>|<span data-ttu-id="0f42d-132">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="0f42d-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="0f42d-133">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="0f42d-133">managedDeviceId</span></span>|<span data-ttu-id="0f42d-134">文字列</span><span class="sxs-lookup"><span data-stu-id="0f42d-134">String</span></span>|<span data-ttu-id="0f42d-135">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="0f42d-135">Intune device id</span></span>|
|<span data-ttu-id="0f42d-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0f42d-136">deviceDisplayName</span></span>|<span data-ttu-id="0f42d-137">String</span><span class="sxs-lookup"><span data-stu-id="0f42d-137">String</span></span>|<span data-ttu-id="0f42d-138">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="0f42d-138">Display name of the device</span></span>|
|<span data-ttu-id="0f42d-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0f42d-139">userPrincipalName</span></span>|<span data-ttu-id="0f42d-140">String</span><span class="sxs-lookup"><span data-stu-id="0f42d-140">String</span></span>|<span data-ttu-id="0f42d-141">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="0f42d-141">User Principal Name</span></span>|
|<span data-ttu-id="0f42d-142">state</span><span class="sxs-lookup"><span data-stu-id="0f42d-142">state</span></span>|[<span data-ttu-id="0f42d-143">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="0f42d-143">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="0f42d-144">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="0f42d-144">Security baseline compliance state.</span></span> <span data-ttu-id="0f42d-145">可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="0f42d-145">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="0f42d-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f42d-146">lastReportedDateTime</span></span>|<span data-ttu-id="0f42d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f42d-147">DateTimeOffset</span></span>|<span data-ttu-id="0f42d-148">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="0f42d-148">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f42d-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f42d-149">Relationships</span></span>
<span data-ttu-id="0f42d-150">なし</span><span class="sxs-lookup"><span data-stu-id="0f42d-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f42d-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f42d-151">JSON Representation</span></span>
<span data-ttu-id="0f42d-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f42d-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





