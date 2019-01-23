---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b17930161f66ca83d59e3f2f62777a79f82b79f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425737"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="096b4-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="096b4-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="096b4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="096b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="096b4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="096b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="096b4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="096b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="096b4-107">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="096b4-107">Device Compilance Policy Setting State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="096b4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="096b4-108">Properties</span></span>
|<span data-ttu-id="096b4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="096b4-109">Property</span></span>|<span data-ttu-id="096b4-110">型</span><span class="sxs-lookup"><span data-stu-id="096b4-110">Type</span></span>|<span data-ttu-id="096b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="096b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="096b4-112">setting</span><span class="sxs-lookup"><span data-stu-id="096b4-112">setting</span></span>|<span data-ttu-id="096b4-113">String</span><span class="sxs-lookup"><span data-stu-id="096b4-113">String</span></span>|<span data-ttu-id="096b4-114">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="096b4-114">The setting that is being reported</span></span>|
|<span data-ttu-id="096b4-115">settingName</span><span class="sxs-lookup"><span data-stu-id="096b4-115">settingName</span></span>|<span data-ttu-id="096b4-116">String</span><span class="sxs-lookup"><span data-stu-id="096b4-116">String</span></span>|<span data-ttu-id="096b4-117">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="096b4-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="096b4-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="096b4-118">instanceDisplayName</span></span>|<span data-ttu-id="096b4-119">String</span><span class="sxs-lookup"><span data-stu-id="096b4-119">String</span></span>|<span data-ttu-id="096b4-120">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="096b4-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="096b4-121">state</span><span class="sxs-lookup"><span data-stu-id="096b4-121">state</span></span>|[<span data-ttu-id="096b4-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="096b4-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="096b4-123">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="096b4-123">The compliance state of the setting.</span></span> <span data-ttu-id="096b4-124">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="096b4-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="096b4-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="096b4-125">errorCode</span></span>|<span data-ttu-id="096b4-126">Int64</span><span class="sxs-lookup"><span data-stu-id="096b4-126">Int64</span></span>|<span data-ttu-id="096b4-127">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="096b4-127">Error code for the setting</span></span>|
|<span data-ttu-id="096b4-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="096b4-128">errorDescription</span></span>|<span data-ttu-id="096b4-129">String</span><span class="sxs-lookup"><span data-stu-id="096b4-129">String</span></span>|<span data-ttu-id="096b4-130">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="096b4-130">Error description</span></span>|
|<span data-ttu-id="096b4-131">userId</span><span class="sxs-lookup"><span data-stu-id="096b4-131">userId</span></span>|<span data-ttu-id="096b4-132">String</span><span class="sxs-lookup"><span data-stu-id="096b4-132">String</span></span>|<span data-ttu-id="096b4-133">UserId</span><span class="sxs-lookup"><span data-stu-id="096b4-133">UserId</span></span>|
|<span data-ttu-id="096b4-134">userName</span><span class="sxs-lookup"><span data-stu-id="096b4-134">userName</span></span>|<span data-ttu-id="096b4-135">String</span><span class="sxs-lookup"><span data-stu-id="096b4-135">String</span></span>|<span data-ttu-id="096b4-136">UserName</span><span class="sxs-lookup"><span data-stu-id="096b4-136">UserName</span></span>|
|<span data-ttu-id="096b4-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="096b4-137">userEmail</span></span>|<span data-ttu-id="096b4-138">String</span><span class="sxs-lookup"><span data-stu-id="096b4-138">String</span></span>|<span data-ttu-id="096b4-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="096b4-139">UserEmail</span></span>|
|<span data-ttu-id="096b4-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="096b4-140">userPrincipalName</span></span>|<span data-ttu-id="096b4-141">String</span><span class="sxs-lookup"><span data-stu-id="096b4-141">String</span></span>|<span data-ttu-id="096b4-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="096b4-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="096b4-143">ソース</span><span class="sxs-lookup"><span data-stu-id="096b4-143">sources</span></span>|<span data-ttu-id="096b4-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="096b4-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="096b4-145">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="096b4-145">Contributing policies</span></span>|
|<span data-ttu-id="096b4-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="096b4-146">currentValue</span></span>|<span data-ttu-id="096b4-147">String</span><span class="sxs-lookup"><span data-stu-id="096b4-147">String</span></span>|<span data-ttu-id="096b4-148">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="096b4-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="096b4-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="096b4-149">Relationships</span></span>
<span data-ttu-id="096b4-150">なし</span><span class="sxs-lookup"><span data-stu-id="096b4-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="096b4-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="096b4-151">JSON Representation</span></span>
<span data-ttu-id="096b4-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="096b4-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingState",
  "setting": "String",
  "settingName": "String",
  "instanceDisplayName": "String",
  "state": "String",
  "errorCode": 1024,
  "errorDescription": "String",
  "userId": "String",
  "userName": "String",
  "userEmail": "String",
  "userPrincipalName": "String",
  "sources": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "String",
      "displayName": "String"
    }
  ],
  "currentValue": "String"
}
```




