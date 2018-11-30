---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
ms.openlocfilehash: 056d4e1b501d438feb5bbda6b7910c9998c73cdb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022011"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="061b0-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="061b0-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="061b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="061b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="061b0-105">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="061b0-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="061b0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="061b0-106">Properties</span></span>
|<span data-ttu-id="061b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="061b0-107">Property</span></span>|<span data-ttu-id="061b0-108">型</span><span class="sxs-lookup"><span data-stu-id="061b0-108">Type</span></span>|<span data-ttu-id="061b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="061b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="061b0-110">setting</span><span class="sxs-lookup"><span data-stu-id="061b0-110">setting</span></span>|<span data-ttu-id="061b0-111">String</span><span class="sxs-lookup"><span data-stu-id="061b0-111">String</span></span>|<span data-ttu-id="061b0-112">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="061b0-112">The setting that is being reported</span></span>|
|<span data-ttu-id="061b0-113">settingName</span><span class="sxs-lookup"><span data-stu-id="061b0-113">settingName</span></span>|<span data-ttu-id="061b0-114">String</span><span class="sxs-lookup"><span data-stu-id="061b0-114">String</span></span>|<span data-ttu-id="061b0-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="061b0-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="061b0-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="061b0-116">instanceDisplayName</span></span>|<span data-ttu-id="061b0-117">String</span><span class="sxs-lookup"><span data-stu-id="061b0-117">String</span></span>|<span data-ttu-id="061b0-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="061b0-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="061b0-119">state</span><span class="sxs-lookup"><span data-stu-id="061b0-119">state</span></span>|[<span data-ttu-id="061b0-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="061b0-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="061b0-121">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="061b0-121">The compliance state of the setting.</span></span> <span data-ttu-id="061b0-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="061b0-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="061b0-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="061b0-123">errorCode</span></span>|<span data-ttu-id="061b0-124">Int64</span><span class="sxs-lookup"><span data-stu-id="061b0-124">Int64</span></span>|<span data-ttu-id="061b0-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="061b0-125">Error code for the setting</span></span>|
|<span data-ttu-id="061b0-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="061b0-126">errorDescription</span></span>|<span data-ttu-id="061b0-127">String</span><span class="sxs-lookup"><span data-stu-id="061b0-127">String</span></span>|<span data-ttu-id="061b0-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="061b0-128">Error description</span></span>|
|<span data-ttu-id="061b0-129">userId</span><span class="sxs-lookup"><span data-stu-id="061b0-129">userId</span></span>|<span data-ttu-id="061b0-130">String</span><span class="sxs-lookup"><span data-stu-id="061b0-130">String</span></span>|<span data-ttu-id="061b0-131">UserId</span><span class="sxs-lookup"><span data-stu-id="061b0-131">UserId</span></span>|
|<span data-ttu-id="061b0-132">userName</span><span class="sxs-lookup"><span data-stu-id="061b0-132">userName</span></span>|<span data-ttu-id="061b0-133">String</span><span class="sxs-lookup"><span data-stu-id="061b0-133">String</span></span>|<span data-ttu-id="061b0-134">UserName</span><span class="sxs-lookup"><span data-stu-id="061b0-134">UserName</span></span>|
|<span data-ttu-id="061b0-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="061b0-135">userEmail</span></span>|<span data-ttu-id="061b0-136">String</span><span class="sxs-lookup"><span data-stu-id="061b0-136">String</span></span>|<span data-ttu-id="061b0-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="061b0-137">UserEmail</span></span>|
|<span data-ttu-id="061b0-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="061b0-138">userPrincipalName</span></span>|<span data-ttu-id="061b0-139">String</span><span class="sxs-lookup"><span data-stu-id="061b0-139">String</span></span>|<span data-ttu-id="061b0-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="061b0-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="061b0-141">ソース</span><span class="sxs-lookup"><span data-stu-id="061b0-141">sources</span></span>|<span data-ttu-id="061b0-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="061b0-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="061b0-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="061b0-143">Contributing policies</span></span>|
|<span data-ttu-id="061b0-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="061b0-144">currentValue</span></span>|<span data-ttu-id="061b0-145">String</span><span class="sxs-lookup"><span data-stu-id="061b0-145">String</span></span>|<span data-ttu-id="061b0-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="061b0-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="061b0-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="061b0-147">Relationships</span></span>
<span data-ttu-id="061b0-148">なし</span><span class="sxs-lookup"><span data-stu-id="061b0-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="061b0-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="061b0-149">JSON Representation</span></span>
<span data-ttu-id="061b0-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="061b0-150">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceConfigurationSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationSettingState",
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



