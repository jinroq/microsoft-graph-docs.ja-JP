---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
ms.openlocfilehash: 7ca50fe6a6186578739b166b1239a309824d1e51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316115"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="8c189-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c189-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="8c189-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8c189-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c189-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c189-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c189-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c189-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c189-107">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="8c189-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="8c189-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c189-108">Properties</span></span>
|<span data-ttu-id="8c189-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c189-109">Property</span></span>|<span data-ttu-id="8c189-110">種類</span><span class="sxs-lookup"><span data-stu-id="8c189-110">Type</span></span>|<span data-ttu-id="8c189-111">説明</span><span class="sxs-lookup"><span data-stu-id="8c189-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c189-112">setting</span><span class="sxs-lookup"><span data-stu-id="8c189-112">setting</span></span>|<span data-ttu-id="8c189-113">String</span><span class="sxs-lookup"><span data-stu-id="8c189-113">String</span></span>|<span data-ttu-id="8c189-114">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="8c189-114">The setting that is being reported</span></span>|
|<span data-ttu-id="8c189-115">settingName</span><span class="sxs-lookup"><span data-stu-id="8c189-115">settingName</span></span>|<span data-ttu-id="8c189-116">String</span><span class="sxs-lookup"><span data-stu-id="8c189-116">String</span></span>|<span data-ttu-id="8c189-117">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="8c189-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="8c189-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="8c189-118">instanceDisplayName</span></span>|<span data-ttu-id="8c189-119">String</span><span class="sxs-lookup"><span data-stu-id="8c189-119">String</span></span>|<span data-ttu-id="8c189-120">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="8c189-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="8c189-121">state</span><span class="sxs-lookup"><span data-stu-id="8c189-121">state</span></span>|[<span data-ttu-id="8c189-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="8c189-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="8c189-123">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="8c189-123">The compliance state of the setting.</span></span> <span data-ttu-id="8c189-124">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="8c189-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="8c189-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="8c189-125">errorCode</span></span>|<span data-ttu-id="8c189-126">Int64</span><span class="sxs-lookup"><span data-stu-id="8c189-126">Int64</span></span>|<span data-ttu-id="8c189-127">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="8c189-127">Error code for the setting</span></span>|
|<span data-ttu-id="8c189-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="8c189-128">errorDescription</span></span>|<span data-ttu-id="8c189-129">String</span><span class="sxs-lookup"><span data-stu-id="8c189-129">String</span></span>|<span data-ttu-id="8c189-130">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="8c189-130">Error description</span></span>|
|<span data-ttu-id="8c189-131">userId</span><span class="sxs-lookup"><span data-stu-id="8c189-131">userId</span></span>|<span data-ttu-id="8c189-132">String</span><span class="sxs-lookup"><span data-stu-id="8c189-132">String</span></span>|<span data-ttu-id="8c189-133">UserId</span><span class="sxs-lookup"><span data-stu-id="8c189-133">UserId</span></span>|
|<span data-ttu-id="8c189-134">userName</span><span class="sxs-lookup"><span data-stu-id="8c189-134">userName</span></span>|<span data-ttu-id="8c189-135">String</span><span class="sxs-lookup"><span data-stu-id="8c189-135">String</span></span>|<span data-ttu-id="8c189-136">UserName</span><span class="sxs-lookup"><span data-stu-id="8c189-136">UserName</span></span>|
|<span data-ttu-id="8c189-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="8c189-137">userEmail</span></span>|<span data-ttu-id="8c189-138">String</span><span class="sxs-lookup"><span data-stu-id="8c189-138">String</span></span>|<span data-ttu-id="8c189-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="8c189-139">UserEmail</span></span>|
|<span data-ttu-id="8c189-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8c189-140">userPrincipalName</span></span>|<span data-ttu-id="8c189-141">String</span><span class="sxs-lookup"><span data-stu-id="8c189-141">String</span></span>|<span data-ttu-id="8c189-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="8c189-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="8c189-143">ソース</span><span class="sxs-lookup"><span data-stu-id="8c189-143">sources</span></span>|<span data-ttu-id="8c189-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8c189-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="8c189-145">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="8c189-145">Contributing policies</span></span>|
|<span data-ttu-id="8c189-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="8c189-146">currentValue</span></span>|<span data-ttu-id="8c189-147">String</span><span class="sxs-lookup"><span data-stu-id="8c189-147">String</span></span>|<span data-ttu-id="8c189-148">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="8c189-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c189-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c189-149">Relationships</span></span>
<span data-ttu-id="8c189-150">なし</span><span class="sxs-lookup"><span data-stu-id="8c189-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8c189-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c189-151">JSON Representation</span></span>
<span data-ttu-id="8c189-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c189-152">Here is a JSON representation of the resource.</span></span>
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





