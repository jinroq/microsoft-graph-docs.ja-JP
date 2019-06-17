---
title: securityBaselineDeviceState リソースの種類
description: デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9fb2195a2cdf68c85e05988b1d2063d21a97228
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983443"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="dcb70-103">securityBaselineDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcb70-103">securityBaselineDeviceState resource type</span></span>

> <span data-ttu-id="dcb70-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcb70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcb70-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcb70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcb70-106">デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。</span><span class="sxs-lookup"><span data-stu-id="dcb70-106">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="dcb70-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dcb70-107">Methods</span></span>
|<span data-ttu-id="dcb70-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dcb70-108">Method</span></span>|<span data-ttu-id="dcb70-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dcb70-109">Return Type</span></span>|<span data-ttu-id="dcb70-110">説明</span><span class="sxs-lookup"><span data-stu-id="dcb70-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dcb70-111">リスト securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="dcb70-111">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="dcb70-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dcb70-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="dcb70-113">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dcb70-113">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="dcb70-114">SecurityBaselineDeviceState を取得する</span><span class="sxs-lookup"><span data-stu-id="dcb70-114">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="dcb70-115">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="dcb70-115">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="dcb70-116">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dcb70-116">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="dcb70-117">SecurityBaselineDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="dcb70-117">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="dcb70-118">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="dcb70-118">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="dcb70-119">新しい[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dcb70-119">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="dcb70-120">SecurityBaselineDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="dcb70-120">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="dcb70-121">None</span><span class="sxs-lookup"><span data-stu-id="dcb70-121">None</span></span>|<span data-ttu-id="dcb70-122">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dcb70-122">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="dcb70-123">SecurityBaselineDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="dcb70-123">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="dcb70-124">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="dcb70-124">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="dcb70-125">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dcb70-125">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dcb70-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcb70-126">Properties</span></span>
|<span data-ttu-id="dcb70-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcb70-127">Property</span></span>|<span data-ttu-id="dcb70-128">型</span><span class="sxs-lookup"><span data-stu-id="dcb70-128">Type</span></span>|<span data-ttu-id="dcb70-129">説明</span><span class="sxs-lookup"><span data-stu-id="dcb70-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcb70-130">id</span><span class="sxs-lookup"><span data-stu-id="dcb70-130">id</span></span>|<span data-ttu-id="dcb70-131">文字列</span><span class="sxs-lookup"><span data-stu-id="dcb70-131">String</span></span>|<span data-ttu-id="dcb70-132">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="dcb70-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="dcb70-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="dcb70-133">managedDeviceId</span></span>|<span data-ttu-id="dcb70-134">String</span><span class="sxs-lookup"><span data-stu-id="dcb70-134">String</span></span>|<span data-ttu-id="dcb70-135">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="dcb70-135">Intune device id</span></span>|
|<span data-ttu-id="dcb70-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="dcb70-136">deviceDisplayName</span></span>|<span data-ttu-id="dcb70-137">String</span><span class="sxs-lookup"><span data-stu-id="dcb70-137">String</span></span>|<span data-ttu-id="dcb70-138">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="dcb70-138">Display name of the device</span></span>|
|<span data-ttu-id="dcb70-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="dcb70-139">userPrincipalName</span></span>|<span data-ttu-id="dcb70-140">String</span><span class="sxs-lookup"><span data-stu-id="dcb70-140">String</span></span>|<span data-ttu-id="dcb70-141">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="dcb70-141">User Principal Name</span></span>|
|<span data-ttu-id="dcb70-142">state</span><span class="sxs-lookup"><span data-stu-id="dcb70-142">state</span></span>|[<span data-ttu-id="dcb70-143">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="dcb70-143">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="dcb70-144">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="dcb70-144">Security baseline compliance state.</span></span> <span data-ttu-id="dcb70-145">使用可能な値: `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="dcb70-145">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="dcb70-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="dcb70-146">lastReportedDateTime</span></span>|<span data-ttu-id="dcb70-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dcb70-147">DateTimeOffset</span></span>|<span data-ttu-id="dcb70-148">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="dcb70-148">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcb70-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcb70-149">Relationships</span></span>
<span data-ttu-id="dcb70-150">なし</span><span class="sxs-lookup"><span data-stu-id="dcb70-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dcb70-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcb70-151">JSON Representation</span></span>
<span data-ttu-id="dcb70-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcb70-152">Here is a JSON representation of the resource.</span></span>
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





