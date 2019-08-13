---
title: securityBaselineDeviceState リソースの種類
description: デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3a7787ae8a55192adc75ab05f6e6cd21988ab2f4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319350"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="ff29c-103">securityBaselineDeviceState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff29c-103">securityBaselineDeviceState resource type</span></span>

> <span data-ttu-id="ff29c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff29c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff29c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff29c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff29c-106">デバイスのセキュリティベースラインのセキュリティベースラインコンプライアンスの状態の要約。</span><span class="sxs-lookup"><span data-stu-id="ff29c-106">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="ff29c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff29c-107">Methods</span></span>
|<span data-ttu-id="ff29c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ff29c-108">Method</span></span>|<span data-ttu-id="ff29c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ff29c-109">Return Type</span></span>|<span data-ttu-id="ff29c-110">説明</span><span class="sxs-lookup"><span data-stu-id="ff29c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ff29c-111">リスト securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="ff29c-111">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="ff29c-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ff29c-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="ff29c-113">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ff29c-113">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="ff29c-114">SecurityBaselineDeviceState を取得する</span><span class="sxs-lookup"><span data-stu-id="ff29c-114">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="ff29c-115">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="ff29c-115">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="ff29c-116">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ff29c-116">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="ff29c-117">SecurityBaselineDeviceState を作成する</span><span class="sxs-lookup"><span data-stu-id="ff29c-117">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="ff29c-118">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="ff29c-118">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="ff29c-119">新しい[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ff29c-119">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="ff29c-120">SecurityBaselineDeviceState の削除</span><span class="sxs-lookup"><span data-stu-id="ff29c-120">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="ff29c-121">None</span><span class="sxs-lookup"><span data-stu-id="ff29c-121">None</span></span>|<span data-ttu-id="ff29c-122">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ff29c-122">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="ff29c-123">SecurityBaselineDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="ff29c-123">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="ff29c-124">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="ff29c-124">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="ff29c-125">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ff29c-125">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff29c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff29c-126">Properties</span></span>
|<span data-ttu-id="ff29c-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff29c-127">Property</span></span>|<span data-ttu-id="ff29c-128">型</span><span class="sxs-lookup"><span data-stu-id="ff29c-128">Type</span></span>|<span data-ttu-id="ff29c-129">説明</span><span class="sxs-lookup"><span data-stu-id="ff29c-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff29c-130">id</span><span class="sxs-lookup"><span data-stu-id="ff29c-130">id</span></span>|<span data-ttu-id="ff29c-131">文字列</span><span class="sxs-lookup"><span data-stu-id="ff29c-131">String</span></span>|<span data-ttu-id="ff29c-132">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="ff29c-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="ff29c-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="ff29c-133">managedDeviceId</span></span>|<span data-ttu-id="ff29c-134">String</span><span class="sxs-lookup"><span data-stu-id="ff29c-134">String</span></span>|<span data-ttu-id="ff29c-135">Intune デバイス id</span><span class="sxs-lookup"><span data-stu-id="ff29c-135">Intune device id</span></span>|
|<span data-ttu-id="ff29c-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="ff29c-136">deviceDisplayName</span></span>|<span data-ttu-id="ff29c-137">String</span><span class="sxs-lookup"><span data-stu-id="ff29c-137">String</span></span>|<span data-ttu-id="ff29c-138">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="ff29c-138">Display name of the device</span></span>|
|<span data-ttu-id="ff29c-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ff29c-139">userPrincipalName</span></span>|<span data-ttu-id="ff29c-140">String</span><span class="sxs-lookup"><span data-stu-id="ff29c-140">String</span></span>|<span data-ttu-id="ff29c-141">ユーザー プリンシパル名</span><span class="sxs-lookup"><span data-stu-id="ff29c-141">User Principal Name</span></span>|
|<span data-ttu-id="ff29c-142">state</span><span class="sxs-lookup"><span data-stu-id="ff29c-142">state</span></span>|[<span data-ttu-id="ff29c-143">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="ff29c-143">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="ff29c-144">セキュリティベースラインコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="ff29c-144">Security baseline compliance state.</span></span> <span data-ttu-id="ff29c-145">使用可能な値: `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="ff29c-145">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="ff29c-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ff29c-146">lastReportedDateTime</span></span>|<span data-ttu-id="ff29c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff29c-147">DateTimeOffset</span></span>|<span data-ttu-id="ff29c-148">ポリシーレポートの最終変更日時</span><span class="sxs-lookup"><span data-stu-id="ff29c-148">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff29c-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff29c-149">Relationships</span></span>
<span data-ttu-id="ff29c-150">なし</span><span class="sxs-lookup"><span data-stu-id="ff29c-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff29c-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff29c-151">JSON Representation</span></span>
<span data-ttu-id="ff29c-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff29c-152">Here is a JSON representation of the resource.</span></span>
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



