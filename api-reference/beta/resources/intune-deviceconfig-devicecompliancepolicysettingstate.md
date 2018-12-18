---
title: deviceCompliancePolicySettingState リソースの種類
description: 特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。
author: tfitzmac
ms.openlocfilehash: fbad84edffaeb3abdff0c00fdd55c1451d23a721
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327959"
---
# <a name="devicecompliancepolicysettingstate-resource-type"></a><span data-ttu-id="fc077-103">deviceCompliancePolicySettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc077-103">deviceCompliancePolicySettingState resource type</span></span>

> <span data-ttu-id="fc077-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc077-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc077-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc077-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc077-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc077-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc077-107">特定のデバイスに関する、デバイス コンプライアンス ポリシーの設定状態です。</span><span class="sxs-lookup"><span data-stu-id="fc077-107">Device Compilance Policy Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="fc077-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc077-108">Properties</span></span>
|<span data-ttu-id="fc077-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc077-109">Property</span></span>|<span data-ttu-id="fc077-110">種類</span><span class="sxs-lookup"><span data-stu-id="fc077-110">Type</span></span>|<span data-ttu-id="fc077-111">説明</span><span class="sxs-lookup"><span data-stu-id="fc077-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc077-112">setting</span><span class="sxs-lookup"><span data-stu-id="fc077-112">setting</span></span>|<span data-ttu-id="fc077-113">String</span><span class="sxs-lookup"><span data-stu-id="fc077-113">String</span></span>|<span data-ttu-id="fc077-114">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="fc077-114">The setting that is being reported</span></span>|
|<span data-ttu-id="fc077-115">settingName</span><span class="sxs-lookup"><span data-stu-id="fc077-115">settingName</span></span>|<span data-ttu-id="fc077-116">String</span><span class="sxs-lookup"><span data-stu-id="fc077-116">String</span></span>|<span data-ttu-id="fc077-117">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="fc077-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="fc077-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fc077-118">instanceDisplayName</span></span>|<span data-ttu-id="fc077-119">String</span><span class="sxs-lookup"><span data-stu-id="fc077-119">String</span></span>|<span data-ttu-id="fc077-120">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="fc077-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="fc077-121">state</span><span class="sxs-lookup"><span data-stu-id="fc077-121">state</span></span>|[<span data-ttu-id="fc077-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="fc077-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="fc077-123">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="fc077-123">The compliance state of the setting.</span></span> <span data-ttu-id="fc077-124">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="fc077-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="fc077-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="fc077-125">errorCode</span></span>|<span data-ttu-id="fc077-126">Int64</span><span class="sxs-lookup"><span data-stu-id="fc077-126">Int64</span></span>|<span data-ttu-id="fc077-127">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="fc077-127">Error code for the setting</span></span>|
|<span data-ttu-id="fc077-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="fc077-128">errorDescription</span></span>|<span data-ttu-id="fc077-129">String</span><span class="sxs-lookup"><span data-stu-id="fc077-129">String</span></span>|<span data-ttu-id="fc077-130">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="fc077-130">Error description</span></span>|
|<span data-ttu-id="fc077-131">userId</span><span class="sxs-lookup"><span data-stu-id="fc077-131">userId</span></span>|<span data-ttu-id="fc077-132">String</span><span class="sxs-lookup"><span data-stu-id="fc077-132">String</span></span>|<span data-ttu-id="fc077-133">UserId</span><span class="sxs-lookup"><span data-stu-id="fc077-133">UserId</span></span>|
|<span data-ttu-id="fc077-134">userName</span><span class="sxs-lookup"><span data-stu-id="fc077-134">userName</span></span>|<span data-ttu-id="fc077-135">String</span><span class="sxs-lookup"><span data-stu-id="fc077-135">String</span></span>|<span data-ttu-id="fc077-136">UserName</span><span class="sxs-lookup"><span data-stu-id="fc077-136">UserName</span></span>|
|<span data-ttu-id="fc077-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="fc077-137">userEmail</span></span>|<span data-ttu-id="fc077-138">String</span><span class="sxs-lookup"><span data-stu-id="fc077-138">String</span></span>|<span data-ttu-id="fc077-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="fc077-139">UserEmail</span></span>|
|<span data-ttu-id="fc077-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fc077-140">userPrincipalName</span></span>|<span data-ttu-id="fc077-141">String</span><span class="sxs-lookup"><span data-stu-id="fc077-141">String</span></span>|<span data-ttu-id="fc077-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="fc077-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="fc077-143">ソース</span><span class="sxs-lookup"><span data-stu-id="fc077-143">sources</span></span>|<span data-ttu-id="fc077-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fc077-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="fc077-145">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="fc077-145">Contributing policies</span></span>|
|<span data-ttu-id="fc077-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="fc077-146">currentValue</span></span>|<span data-ttu-id="fc077-147">String</span><span class="sxs-lookup"><span data-stu-id="fc077-147">String</span></span>|<span data-ttu-id="fc077-148">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="fc077-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc077-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fc077-149">Relationships</span></span>
<span data-ttu-id="fc077-150">なし</span><span class="sxs-lookup"><span data-stu-id="fc077-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fc077-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc077-151">JSON Representation</span></span>
<span data-ttu-id="fc077-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fc077-152">Here is a JSON representation of the resource.</span></span>
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





