---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3ce294f8c22dea483f9b72b167b7ee092e339b7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142561"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="83183-103">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83183-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="83183-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83183-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83183-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83183-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83183-106">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="83183-106">Store App for Windows information protection</span></span>


<span data-ttu-id="83183-107">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="83183-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="83183-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83183-108">Properties</span></span>
|<span data-ttu-id="83183-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83183-109">Property</span></span>|<span data-ttu-id="83183-110">型</span><span class="sxs-lookup"><span data-stu-id="83183-110">Type</span></span>|<span data-ttu-id="83183-111">説明</span><span class="sxs-lookup"><span data-stu-id="83183-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83183-112">displayName</span><span class="sxs-lookup"><span data-stu-id="83183-112">displayName</span></span>|<span data-ttu-id="83183-113">文字列</span><span class="sxs-lookup"><span data-stu-id="83183-113">String</span></span>|<span data-ttu-id="83183-114">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="83183-114">App display name.</span></span> <span data-ttu-id="83183-115">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="83183-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="83183-116">説明</span><span class="sxs-lookup"><span data-stu-id="83183-116">description</span></span>|<span data-ttu-id="83183-117">文字列</span><span class="sxs-lookup"><span data-stu-id="83183-117">String</span></span>|<span data-ttu-id="83183-118">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="83183-118">The app's description.</span></span> <span data-ttu-id="83183-119">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="83183-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="83183-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="83183-120">publisherName</span></span>|<span data-ttu-id="83183-121">String</span><span class="sxs-lookup"><span data-stu-id="83183-121">String</span></span>|<span data-ttu-id="83183-122">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="83183-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="83183-123">productName</span><span class="sxs-lookup"><span data-stu-id="83183-123">productName</span></span>|<span data-ttu-id="83183-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="83183-124">String</span></span>|<span data-ttu-id="83183-125">製品名。</span><span class="sxs-lookup"><span data-stu-id="83183-125">The product name.</span></span> <span data-ttu-id="83183-126">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="83183-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="83183-127">denied</span><span class="sxs-lookup"><span data-stu-id="83183-127">denied</span></span>|<span data-ttu-id="83183-128">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="83183-128">Boolean</span></span>|<span data-ttu-id="83183-129">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="83183-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="83183-130">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="83183-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="83183-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="83183-131">Relationships</span></span>
<span data-ttu-id="83183-132">なし</span><span class="sxs-lookup"><span data-stu-id="83183-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83183-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83183-133">JSON Representation</span></span>
<span data-ttu-id="83183-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83183-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```




