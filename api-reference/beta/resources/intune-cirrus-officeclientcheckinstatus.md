---
title: officeClientCheckinStatus リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: df8f1927329a34a51b5f6d8738faec05be01b451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012003"
---
# <a name="officeclientcheckinstatus-resource-type"></a><span data-ttu-id="241ed-103">officeClientCheckinStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="241ed-103">officeClientCheckinStatus resource type</span></span>

> <span data-ttu-id="241ed-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="241ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="241ed-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="241ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="241ed-106">テナントのチェックイン統計を記述するエンティティ。</span><span class="sxs-lookup"><span data-stu-id="241ed-106">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="241ed-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="241ed-107">Properties</span></span>
|<span data-ttu-id="241ed-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="241ed-108">Property</span></span>|<span data-ttu-id="241ed-109">型</span><span class="sxs-lookup"><span data-stu-id="241ed-109">Type</span></span>|<span data-ttu-id="241ed-110">説明</span><span class="sxs-lookup"><span data-stu-id="241ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="241ed-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="241ed-111">userPrincipalName</span></span>|<span data-ttu-id="241ed-112">String</span><span class="sxs-lookup"><span data-stu-id="241ed-112">String</span></span>|<span data-ttu-id="241ed-113">デバイスを使用したユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="241ed-113">User principal name using the device.</span></span>|
|<span data-ttu-id="241ed-114">deviceName</span><span class="sxs-lookup"><span data-stu-id="241ed-114">deviceName</span></span>|<span data-ttu-id="241ed-115">String</span><span class="sxs-lookup"><span data-stu-id="241ed-115">String</span></span>|<span data-ttu-id="241ed-116">チェックインしようとしているデバイスの名前。</span><span class="sxs-lookup"><span data-stu-id="241ed-116">Device name trying to check-in.</span></span>|
|<span data-ttu-id="241ed-117">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="241ed-117">devicePlatform</span></span>|<span data-ttu-id="241ed-118">String</span><span class="sxs-lookup"><span data-stu-id="241ed-118">String</span></span>|<span data-ttu-id="241ed-119">チェックインしようとしているデバイスプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="241ed-119">Device platform trying to check-in.</span></span>|
|<span data-ttu-id="241ed-120">devicePlatformVersion</span><span class="sxs-lookup"><span data-stu-id="241ed-120">devicePlatformVersion</span></span>|<span data-ttu-id="241ed-121">String</span><span class="sxs-lookup"><span data-stu-id="241ed-121">String</span></span>|<span data-ttu-id="241ed-122">デバイスプラットフォームのバージョンをチェックインしようとしています。</span><span class="sxs-lookup"><span data-stu-id="241ed-122">Device platform version trying to check-in.</span></span>|
|<span data-ttu-id="241ed-123">成功</span><span class="sxs-lookup"><span data-stu-id="241ed-123">wasSuccessful</span></span>|<span data-ttu-id="241ed-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="241ed-124">Boolean</span></span>|<span data-ttu-id="241ed-125">前回のチェックインが成功した場合。</span><span class="sxs-lookup"><span data-stu-id="241ed-125">If the last checkin was successful.</span></span>|
|<span data-ttu-id="241ed-126">userId</span><span class="sxs-lookup"><span data-stu-id="241ed-126">userId</span></span>|<span data-ttu-id="241ed-127">String</span><span class="sxs-lookup"><span data-stu-id="241ed-127">String</span></span>|<span data-ttu-id="241ed-128">デバイスを使用するユーザー識別子。</span><span class="sxs-lookup"><span data-stu-id="241ed-128">User identifier using the device.</span></span>|
|<span data-ttu-id="241ed-129">checkinDateTime</span><span class="sxs-lookup"><span data-stu-id="241ed-129">checkinDateTime</span></span>|<span data-ttu-id="241ed-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="241ed-130">DateTimeOffset</span></span>|<span data-ttu-id="241ed-131">前回のデバイスのチェックイン時刻 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="241ed-131">Last device check-in time in UTC.</span></span>|
|<span data-ttu-id="241ed-132">errorMessage</span><span class="sxs-lookup"><span data-stu-id="241ed-132">errorMessage</span></span>|<span data-ttu-id="241ed-133">String</span><span class="sxs-lookup"><span data-stu-id="241ed-133">String</span></span>|<span data-ttu-id="241ed-134">前回のチェックインに関連付けられたエラーメッセージ。</span><span class="sxs-lookup"><span data-stu-id="241ed-134">Error message if any associated for the last checkin.</span></span>|
|<span data-ttu-id="241ed-135">appliedPolicies</span><span class="sxs-lookup"><span data-stu-id="241ed-135">appliedPolicies</span></span>|<span data-ttu-id="241ed-136">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="241ed-136">String collection</span></span>|<span data-ttu-id="241ed-137">前回のチェックインとしてデバイスに配信されたポリシーの一覧です。</span><span class="sxs-lookup"><span data-stu-id="241ed-137">List of policies delivered to the device as last checkin.</span></span>|

## <a name="relationships"></a><span data-ttu-id="241ed-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="241ed-138">Relationships</span></span>
<span data-ttu-id="241ed-139">なし</span><span class="sxs-lookup"><span data-stu-id="241ed-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="241ed-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="241ed-140">JSON Representation</span></span>
<span data-ttu-id="241ed-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="241ed-141">Here is a JSON representation of the resource.</span></span>
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



