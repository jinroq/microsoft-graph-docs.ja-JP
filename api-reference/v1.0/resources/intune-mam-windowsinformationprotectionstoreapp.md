---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aaba3e5a34eb4f985d6afe7879159dd3cff456b8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037619"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="6122d-103">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6122d-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="6122d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6122d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6122d-105">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="6122d-105">Store App for Windows information protection</span></span>


<span data-ttu-id="6122d-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6122d-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6122d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6122d-107">Properties</span></span>
|<span data-ttu-id="6122d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6122d-108">Property</span></span>|<span data-ttu-id="6122d-109">型</span><span class="sxs-lookup"><span data-stu-id="6122d-109">Type</span></span>|<span data-ttu-id="6122d-110">説明</span><span class="sxs-lookup"><span data-stu-id="6122d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6122d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6122d-111">displayName</span></span>|<span data-ttu-id="6122d-112">文字列</span><span class="sxs-lookup"><span data-stu-id="6122d-112">String</span></span>|<span data-ttu-id="6122d-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="6122d-113">App display name.</span></span> <span data-ttu-id="6122d-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6122d-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6122d-115">description</span><span class="sxs-lookup"><span data-stu-id="6122d-115">description</span></span>|<span data-ttu-id="6122d-116">String</span><span class="sxs-lookup"><span data-stu-id="6122d-116">String</span></span>|<span data-ttu-id="6122d-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="6122d-117">The app's description.</span></span> <span data-ttu-id="6122d-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6122d-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6122d-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="6122d-119">publisherName</span></span>|<span data-ttu-id="6122d-120">String</span><span class="sxs-lookup"><span data-stu-id="6122d-120">String</span></span>|<span data-ttu-id="6122d-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="6122d-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6122d-122">productName</span><span class="sxs-lookup"><span data-stu-id="6122d-122">productName</span></span>|<span data-ttu-id="6122d-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6122d-123">String</span></span>|<span data-ttu-id="6122d-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="6122d-124">The product name.</span></span> <span data-ttu-id="6122d-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6122d-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="6122d-126">denied</span><span class="sxs-lookup"><span data-stu-id="6122d-126">denied</span></span>|<span data-ttu-id="6122d-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="6122d-127">Boolean</span></span>|<span data-ttu-id="6122d-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="6122d-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="6122d-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="6122d-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6122d-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6122d-130">Relationships</span></span>
<span data-ttu-id="6122d-131">なし</span><span class="sxs-lookup"><span data-stu-id="6122d-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6122d-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6122d-132">JSON Representation</span></span>
<span data-ttu-id="6122d-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6122d-133">Here is a JSON representation of the resource.</span></span>
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



