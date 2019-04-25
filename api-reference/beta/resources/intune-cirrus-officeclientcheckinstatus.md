---
title: officeClientCheckinStatus リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 465b07ba286b9ee3a58132424be2a25b1c7e564e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526700"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="604fb-103">officeClientCheckinStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="604fb-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="604fb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="604fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="604fb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="604fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="604fb-106">テナントのチェックイン統計を記述するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="604fb-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="604fb-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="604fb-107">Properties</span></span>
|<span data-ttu-id="604fb-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="604fb-108">Property</span></span>|<span data-ttu-id="604fb-109">型</span><span class="sxs-lookup"><span data-stu-id="604fb-109">Type</span></span>|<span data-ttu-id="604fb-110">説明</span><span class="sxs-lookup"><span data-stu-id="604fb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="604fb-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="604fb-111">userPrincipalName</span></span>|<span data-ttu-id="604fb-112">String</span><span class="sxs-lookup"><span data-stu-id="604fb-112">String</span></span>|<span data-ttu-id="604fb-113">デバイスを使用したユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="604fb-113">User principal name using the device.</span></span>|
|<span data-ttu-id="604fb-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="604fb-114">deviceName</span></span>|<span data-ttu-id="604fb-115">String</span><span class="sxs-lookup"><span data-stu-id="604fb-115">String</span></span>|<span data-ttu-id="604fb-116">チェックインしようとしているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="604fb-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="604fb-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="604fb-117">devicePlatform</span></span>|<span data-ttu-id="604fb-118">String</span><span class="sxs-lookup"><span data-stu-id="604fb-118">String</span></span>|<span data-ttu-id="604fb-119">チェックインしようとしているデバイスプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="604fb-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="604fb-120">deviceplatformversion</span><span class="sxs-lookup"><span data-stu-id="604fb-120">devicePlatformVersion</span></span>|<span data-ttu-id="604fb-121">String</span><span class="sxs-lookup"><span data-stu-id="604fb-121">String</span></span>|<span data-ttu-id="604fb-122">デバイスプラットフォームのバージョンをチェックインしようとしています。</span><span class="sxs-lookup"><span data-stu-id="604fb-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="604fb-123">成功</span><span class="sxs-lookup"><span data-stu-id="604fb-123">wasSuccessful</span></span>|<span data-ttu-id="604fb-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="604fb-124">Boolean</span></span>|<span data-ttu-id="604fb-125">前回のチェックインが成功した場合。</span><span class="sxs-lookup"><span data-stu-id="604fb-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="604fb-126">userId</span><span class="sxs-lookup"><span data-stu-id="604fb-126">userId</span></span>|<span data-ttu-id="604fb-127">String</span><span class="sxs-lookup"><span data-stu-id="604fb-127">String</span></span>|<span data-ttu-id="604fb-128">デバイスを使用するユーザー識別子。</span><span class="sxs-lookup"><span data-stu-id="604fb-128">User identifier using the device.</span></span>|
|<span data-ttu-id="604fb-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="604fb-129">checkinDateTime</span></span>|<span data-ttu-id="604fb-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="604fb-130">DateTimeOffset</span></span>|<span data-ttu-id="604fb-131">前回のデバイスのチェックイン時刻 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="604fb-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="604fb-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="604fb-132">errorMessage</span></span>|<span data-ttu-id="604fb-133">String</span><span class="sxs-lookup"><span data-stu-id="604fb-133">String</span></span>|<span data-ttu-id="604fb-134">前回のチェックインに関連付けられたエラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="604fb-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="604fb-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="604fb-135">appliedPolicies</span></span>|<span data-ttu-id="604fb-136">String collection</span><span class="sxs-lookup"><span data-stu-id="604fb-136">String collection</span></span>|<span data-ttu-id="604fb-137">前回のチェックインとしてデバイスに配信されたポリシーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="604fb-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="604fb-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="604fb-138">Relationships</span></span>
<span data-ttu-id="604fb-139">なし</span><span class="sxs-lookup"><span data-stu-id="604fb-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="604fb-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="604fb-140">JSON Representation</span></span>
<span data-ttu-id="604fb-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="604fb-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeClientCheckinStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeClientCheckinStatus",
  "userPrincipalName": "String",
  "deviceName": "String",
  "devicePlatform": "String",
  "devicePlatformVersion": "String",
  "wasSuccessful": true,
  "userId": "String",
  "checkinDateTime": "String (timestamp)",
  "errorMessage": "String",
  "appliedPolicies": [
    "String"
  ]
}
```



