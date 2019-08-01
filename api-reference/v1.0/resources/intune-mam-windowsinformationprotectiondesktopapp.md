---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d9187858aa90480ba8720bc2111f3ba071492e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037703"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="8cfa1-103">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cfa1-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="8cfa1-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cfa1-105">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="8cfa1-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="8cfa1-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8cfa1-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8cfa1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cfa1-107">Properties</span></span>
|<span data-ttu-id="8cfa1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cfa1-108">Property</span></span>|<span data-ttu-id="8cfa1-109">型</span><span class="sxs-lookup"><span data-stu-id="8cfa1-109">Type</span></span>|<span data-ttu-id="8cfa1-110">説明</span><span class="sxs-lookup"><span data-stu-id="8cfa1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cfa1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8cfa1-111">displayName</span></span>|<span data-ttu-id="8cfa1-112">文字列</span><span class="sxs-lookup"><span data-stu-id="8cfa1-112">String</span></span>|<span data-ttu-id="8cfa1-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-113">App display name.</span></span> <span data-ttu-id="8cfa1-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8cfa1-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="8cfa1-115">description</span><span class="sxs-lookup"><span data-stu-id="8cfa1-115">description</span></span>|<span data-ttu-id="8cfa1-116">String</span><span class="sxs-lookup"><span data-stu-id="8cfa1-116">String</span></span>|<span data-ttu-id="8cfa1-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-117">The app's description.</span></span> <span data-ttu-id="8cfa1-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8cfa1-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="8cfa1-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="8cfa1-119">publisherName</span></span>|<span data-ttu-id="8cfa1-120">String</span><span class="sxs-lookup"><span data-stu-id="8cfa1-120">String</span></span>|<span data-ttu-id="8cfa1-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="8cfa1-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="8cfa1-122">productName</span><span class="sxs-lookup"><span data-stu-id="8cfa1-122">productName</span></span>|<span data-ttu-id="8cfa1-123">String</span><span class="sxs-lookup"><span data-stu-id="8cfa1-123">String</span></span>|<span data-ttu-id="8cfa1-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-124">The product name.</span></span> <span data-ttu-id="8cfa1-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8cfa1-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="8cfa1-126">denied</span><span class="sxs-lookup"><span data-stu-id="8cfa1-126">denied</span></span>|<span data-ttu-id="8cfa1-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8cfa1-127">Boolean</span></span>|<span data-ttu-id="8cfa1-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="8cfa1-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8cfa1-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="8cfa1-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="8cfa1-130">binaryName</span></span>|<span data-ttu-id="8cfa1-131">String</span><span class="sxs-lookup"><span data-stu-id="8cfa1-131">String</span></span>|<span data-ttu-id="8cfa1-132">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-132">The binary name.</span></span>|
|<span data-ttu-id="8cfa1-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="8cfa1-133">binaryVersionLow</span></span>|<span data-ttu-id="8cfa1-134">String</span><span class="sxs-lookup"><span data-stu-id="8cfa1-134">String</span></span>|<span data-ttu-id="8cfa1-135">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-135">The lower binary version.</span></span>|
|<span data-ttu-id="8cfa1-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="8cfa1-136">binaryVersionHigh</span></span>|<span data-ttu-id="8cfa1-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8cfa1-137">String</span></span>|<span data-ttu-id="8cfa1-138">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cfa1-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cfa1-139">Relationships</span></span>
<span data-ttu-id="8cfa1-140">なし</span><span class="sxs-lookup"><span data-stu-id="8cfa1-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cfa1-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cfa1-141">JSON Representation</span></span>
<span data-ttu-id="8cfa1-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cfa1-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



