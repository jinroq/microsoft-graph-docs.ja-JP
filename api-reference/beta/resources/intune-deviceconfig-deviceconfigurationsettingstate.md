---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
ms.openlocfilehash: 551b5ccb215492f48d9cd26bcf8b7e2cb80ed787
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069929"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="f2608-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2608-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="f2608-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2608-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2608-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2608-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2608-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2608-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2608-107">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="f2608-107">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="f2608-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2608-108">Properties</span></span>
|<span data-ttu-id="f2608-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2608-109">Property</span></span>|<span data-ttu-id="f2608-110">型</span><span class="sxs-lookup"><span data-stu-id="f2608-110">Type</span></span>|<span data-ttu-id="f2608-111">説明</span><span class="sxs-lookup"><span data-stu-id="f2608-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2608-112">setting</span><span class="sxs-lookup"><span data-stu-id="f2608-112">setting</span></span>|<span data-ttu-id="f2608-113">String</span><span class="sxs-lookup"><span data-stu-id="f2608-113">String</span></span>|<span data-ttu-id="f2608-114">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="f2608-114">The setting that is being reported</span></span>|
|<span data-ttu-id="f2608-115">settingName</span><span class="sxs-lookup"><span data-stu-id="f2608-115">settingName</span></span>|<span data-ttu-id="f2608-116">String</span><span class="sxs-lookup"><span data-stu-id="f2608-116">String</span></span>|<span data-ttu-id="f2608-117">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="f2608-117">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="f2608-118">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="f2608-118">instanceDisplayName</span></span>|<span data-ttu-id="f2608-119">String</span><span class="sxs-lookup"><span data-stu-id="f2608-119">String</span></span>|<span data-ttu-id="f2608-120">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="f2608-120">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="f2608-121">state</span><span class="sxs-lookup"><span data-stu-id="f2608-121">state</span></span>|[<span data-ttu-id="f2608-122">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="f2608-122">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="f2608-123">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="f2608-123">The compliance state of the setting.</span></span> <span data-ttu-id="f2608-124">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="f2608-124">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="f2608-125">errorCode</span><span class="sxs-lookup"><span data-stu-id="f2608-125">errorCode</span></span>|<span data-ttu-id="f2608-126">Int64</span><span class="sxs-lookup"><span data-stu-id="f2608-126">Int64</span></span>|<span data-ttu-id="f2608-127">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="f2608-127">Error code for the setting</span></span>|
|<span data-ttu-id="f2608-128">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f2608-128">errorDescription</span></span>|<span data-ttu-id="f2608-129">String</span><span class="sxs-lookup"><span data-stu-id="f2608-129">String</span></span>|<span data-ttu-id="f2608-130">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="f2608-130">Error description</span></span>|
|<span data-ttu-id="f2608-131">userId</span><span class="sxs-lookup"><span data-stu-id="f2608-131">userId</span></span>|<span data-ttu-id="f2608-132">String</span><span class="sxs-lookup"><span data-stu-id="f2608-132">String</span></span>|<span data-ttu-id="f2608-133">UserId</span><span class="sxs-lookup"><span data-stu-id="f2608-133">UserId</span></span>|
|<span data-ttu-id="f2608-134">userName</span><span class="sxs-lookup"><span data-stu-id="f2608-134">userName</span></span>|<span data-ttu-id="f2608-135">String</span><span class="sxs-lookup"><span data-stu-id="f2608-135">String</span></span>|<span data-ttu-id="f2608-136">UserName</span><span class="sxs-lookup"><span data-stu-id="f2608-136">UserName</span></span>|
|<span data-ttu-id="f2608-137">userEmail</span><span class="sxs-lookup"><span data-stu-id="f2608-137">userEmail</span></span>|<span data-ttu-id="f2608-138">String</span><span class="sxs-lookup"><span data-stu-id="f2608-138">String</span></span>|<span data-ttu-id="f2608-139">UserEmail</span><span class="sxs-lookup"><span data-stu-id="f2608-139">UserEmail</span></span>|
|<span data-ttu-id="f2608-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f2608-140">userPrincipalName</span></span>|<span data-ttu-id="f2608-141">String</span><span class="sxs-lookup"><span data-stu-id="f2608-141">String</span></span>|<span data-ttu-id="f2608-142">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="f2608-142">UserPrincipalName.</span></span>|
|<span data-ttu-id="f2608-143">ソース</span><span class="sxs-lookup"><span data-stu-id="f2608-143">sources</span></span>|<span data-ttu-id="f2608-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f2608-144">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="f2608-145">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="f2608-145">Contributing policies</span></span>|
|<span data-ttu-id="f2608-146">currentValue</span><span class="sxs-lookup"><span data-stu-id="f2608-146">currentValue</span></span>|<span data-ttu-id="f2608-147">String</span><span class="sxs-lookup"><span data-stu-id="f2608-147">String</span></span>|<span data-ttu-id="f2608-148">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="f2608-148">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2608-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2608-149">Relationships</span></span>
<span data-ttu-id="f2608-150">なし</span><span class="sxs-lookup"><span data-stu-id="f2608-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f2608-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2608-151">JSON Representation</span></span>
<span data-ttu-id="f2608-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2608-152">Here is a JSON representation of the resource.</span></span>
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





