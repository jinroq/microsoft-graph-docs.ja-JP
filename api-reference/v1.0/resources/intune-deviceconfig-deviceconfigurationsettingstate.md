---
title: deviceConfigurationSettingState リソースの種類
description: 指定されたデバイスのデバイス構成設定の状態。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68c57b8842136494bf0604a31f62992f7a1c2501
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928011"
---
# <a name="deviceconfigurationsettingstate-resource-type"></a><span data-ttu-id="874e2-103">deviceConfigurationSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="874e2-103">deviceConfigurationSettingState resource type</span></span>

> <span data-ttu-id="874e2-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="874e2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="874e2-105">指定されたデバイスのデバイス構成設定の状態。</span><span class="sxs-lookup"><span data-stu-id="874e2-105">Device Configuration Setting State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="874e2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="874e2-106">Properties</span></span>
|<span data-ttu-id="874e2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="874e2-107">Property</span></span>|<span data-ttu-id="874e2-108">種類</span><span class="sxs-lookup"><span data-stu-id="874e2-108">Type</span></span>|<span data-ttu-id="874e2-109">説明</span><span class="sxs-lookup"><span data-stu-id="874e2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="874e2-110">setting</span><span class="sxs-lookup"><span data-stu-id="874e2-110">setting</span></span>|<span data-ttu-id="874e2-111">String</span><span class="sxs-lookup"><span data-stu-id="874e2-111">String</span></span>|<span data-ttu-id="874e2-112">レポートされている設定値です。</span><span class="sxs-lookup"><span data-stu-id="874e2-112">The setting that is being reported</span></span>|
|<span data-ttu-id="874e2-113">settingName</span><span class="sxs-lookup"><span data-stu-id="874e2-113">settingName</span></span>|<span data-ttu-id="874e2-114">String</span><span class="sxs-lookup"><span data-stu-id="874e2-114">String</span></span>|<span data-ttu-id="874e2-115">レポートされている、ローカライズされた設定名またはユーザー フレンドリな設定名です</span><span class="sxs-lookup"><span data-stu-id="874e2-115">Localized/user friendly setting name that is being reported</span></span>|
|<span data-ttu-id="874e2-116">instanceDisplayName</span><span class="sxs-lookup"><span data-stu-id="874e2-116">instanceDisplayName</span></span>|<span data-ttu-id="874e2-117">String</span><span class="sxs-lookup"><span data-stu-id="874e2-117">String</span></span>|<span data-ttu-id="874e2-118">レポートされている設定インスタンスの名前です。</span><span class="sxs-lookup"><span data-stu-id="874e2-118">Name of setting instance that is being reported.</span></span>|
|<span data-ttu-id="874e2-119">state</span><span class="sxs-lookup"><span data-stu-id="874e2-119">state</span></span>|[<span data-ttu-id="874e2-120">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="874e2-120">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="874e2-121">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="874e2-121">The compliance state of the setting.</span></span> <span data-ttu-id="874e2-122">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="874e2-122">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="874e2-123">errorCode</span><span class="sxs-lookup"><span data-stu-id="874e2-123">errorCode</span></span>|<span data-ttu-id="874e2-124">Int64</span><span class="sxs-lookup"><span data-stu-id="874e2-124">Int64</span></span>|<span data-ttu-id="874e2-125">設定のエラー コード</span><span class="sxs-lookup"><span data-stu-id="874e2-125">Error code for the setting</span></span>|
|<span data-ttu-id="874e2-126">errorDescription</span><span class="sxs-lookup"><span data-stu-id="874e2-126">errorDescription</span></span>|<span data-ttu-id="874e2-127">String</span><span class="sxs-lookup"><span data-stu-id="874e2-127">String</span></span>|<span data-ttu-id="874e2-128">エラーの説明</span><span class="sxs-lookup"><span data-stu-id="874e2-128">Error description</span></span>|
|<span data-ttu-id="874e2-129">userId</span><span class="sxs-lookup"><span data-stu-id="874e2-129">userId</span></span>|<span data-ttu-id="874e2-130">String</span><span class="sxs-lookup"><span data-stu-id="874e2-130">String</span></span>|<span data-ttu-id="874e2-131">UserId</span><span class="sxs-lookup"><span data-stu-id="874e2-131">UserId</span></span>|
|<span data-ttu-id="874e2-132">userName</span><span class="sxs-lookup"><span data-stu-id="874e2-132">userName</span></span>|<span data-ttu-id="874e2-133">String</span><span class="sxs-lookup"><span data-stu-id="874e2-133">String</span></span>|<span data-ttu-id="874e2-134">UserName</span><span class="sxs-lookup"><span data-stu-id="874e2-134">UserName</span></span>|
|<span data-ttu-id="874e2-135">userEmail</span><span class="sxs-lookup"><span data-stu-id="874e2-135">userEmail</span></span>|<span data-ttu-id="874e2-136">String</span><span class="sxs-lookup"><span data-stu-id="874e2-136">String</span></span>|<span data-ttu-id="874e2-137">UserEmail</span><span class="sxs-lookup"><span data-stu-id="874e2-137">UserEmail</span></span>|
|<span data-ttu-id="874e2-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="874e2-138">userPrincipalName</span></span>|<span data-ttu-id="874e2-139">String</span><span class="sxs-lookup"><span data-stu-id="874e2-139">String</span></span>|<span data-ttu-id="874e2-140">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="874e2-140">UserPrincipalName.</span></span>|
|<span data-ttu-id="874e2-141">ソース</span><span class="sxs-lookup"><span data-stu-id="874e2-141">sources</span></span>|<span data-ttu-id="874e2-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="874e2-142">[settingSource](../resources/intune-deviceconfig-settingsource.md) collection</span></span>|<span data-ttu-id="874e2-143">投稿ポリシー</span><span class="sxs-lookup"><span data-stu-id="874e2-143">Contributing policies</span></span>|
|<span data-ttu-id="874e2-144">currentValue</span><span class="sxs-lookup"><span data-stu-id="874e2-144">currentValue</span></span>|<span data-ttu-id="874e2-145">String</span><span class="sxs-lookup"><span data-stu-id="874e2-145">String</span></span>|<span data-ttu-id="874e2-146">デバイスに関する設定の現在の値</span><span class="sxs-lookup"><span data-stu-id="874e2-146">Current value of setting on device</span></span>|

## <a name="relationships"></a><span data-ttu-id="874e2-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="874e2-147">Relationships</span></span>
<span data-ttu-id="874e2-148">なし</span><span class="sxs-lookup"><span data-stu-id="874e2-148">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="874e2-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="874e2-149">JSON Representation</span></span>
<span data-ttu-id="874e2-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="874e2-150">Here is a JSON representation of the resource.</span></span>
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



