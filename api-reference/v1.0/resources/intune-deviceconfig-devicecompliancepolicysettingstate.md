---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 63c60b2d7d714f7040c894da872c017e06ad0249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832874"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="3c2e5-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c2e5-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="3c2e5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c2e5-105">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-105">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="3c2e5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c2e5-106">Properties</span></span>
|<span data-ttu-id="3c2e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c2e5-107">Property</span></span>|<span data-ttu-id="3c2e5-108">種類</span><span class="sxs-lookup"><span data-stu-id="3c2e5-108">Type</span></span>|<span data-ttu-id="3c2e5-109">説明</span><span class="sxs-lookup"><span data-stu-id="3c2e5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c2e5-110">setting</span><span class="sxs-lookup"><span data-stu-id="3c2e5-110">setting</span></span>|<span data-ttu-id="3c2e5-111">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-111">String</span></span>|<span data-ttu-id="3c2e5-112">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-112">The setting that is being reported</span></span>|
|<span data-ttu-id="3c2e5-113">settingName</span><span class="sxs-lookup"><span data-stu-id="3c2e5-113">settingName</span></span>|<span data-ttu-id="3c2e5-114">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-114">String</span></span>|<span data-ttu-id="3c2e5-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="3c2e5-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="3c2e5-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="3c2e5-116">instanceDisplayName</span></span>|<span data-ttu-id="3c2e5-117">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-117">String</span></span>|<span data-ttu-id="3c2e5-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="3c2e5-119">state</span><span class="sxs-lookup"><span data-stu-id="3c2e5-119">state</span></span>|[<span data-ttu-id="3c2e5-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="3c2e5-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="3c2e5-121">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-121">The compliance state of the setting.</span></span> <span data-ttu-id="3c2e5-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="3c2e5-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="3c2e5-123">errorCode</span></span>|<span data-ttu-id="3c2e5-124">Int64</span><span class="sxs-lookup"><span data-stu-id="3c2e5-124">Int64</span></span>|<span data-ttu-id="3c2e5-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="3c2e5-125">Error code for the setting</span></span>|
|<span data-ttu-id="3c2e5-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="3c2e5-126">errorDescription</span></span>|<span data-ttu-id="3c2e5-127">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-127">String</span></span>|<span data-ttu-id="3c2e5-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="3c2e5-128">Error description</span></span>|
|<span data-ttu-id="3c2e5-129">userId</span><span class="sxs-lookup"><span data-stu-id="3c2e5-129">userId</span></span>|<span data-ttu-id="3c2e5-130">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-130">String</span></span>|<span data-ttu-id="3c2e5-131">UserId</span><span class="sxs-lookup"><span data-stu-id="3c2e5-131">UserId</span></span>|
|<span data-ttu-id="3c2e5-132">userName</span><span class="sxs-lookup"><span data-stu-id="3c2e5-132">userName</span></span>|<span data-ttu-id="3c2e5-133">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-133">String</span></span>|<span data-ttu-id="3c2e5-134">UserName</span><span class="sxs-lookup"><span data-stu-id="3c2e5-134">UserName</span></span>|
|<span data-ttu-id="3c2e5-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="3c2e5-135">userEmail</span></span>|<span data-ttu-id="3c2e5-136">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-136">String</span></span>|<span data-ttu-id="3c2e5-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="3c2e5-137">UserEmail</span></span>|
|<span data-ttu-id="3c2e5-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c2e5-138">userPrincipalName</span></span>|<span data-ttu-id="3c2e5-139">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-139">String</span></span>|<span data-ttu-id="3c2e5-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="3c2e5-141">ソース</span><span class="sxs-lookup"><span data-stu-id="3c2e5-141">sources</span></span>|<span data-ttu-id="3c2e5-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3c2e5-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="3c2e5-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="3c2e5-143">Contributing policies</span></span>|
|<span data-ttu-id="3c2e5-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="3c2e5-144">currentValue</span></span>|<span data-ttu-id="3c2e5-145">String</span><span class="sxs-lookup"><span data-stu-id="3c2e5-145">String</span></span>|<span data-ttu-id="3c2e5-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="3c2e5-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c2e5-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3c2e5-147">Relationships</span></span>
<span data-ttu-id="3c2e5-148">なし</span><span class="sxs-lookup"><span data-stu-id="3c2e5-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c2e5-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c2e5-149">JSON Representation</span></span>
<span data-ttu-id="3c2e5-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c2e5-150">Here is a JSON representation of the resource.</span></span>
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



