---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83ad9e3e500ab5276e4643055f602e763de34fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564254"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="107bc-103">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="107bc-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="107bc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="107bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="107bc-105">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="107bc-105">Desktop App for Windows information protection</span></span>


<span data-ttu-id="107bc-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="107bc-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="107bc-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="107bc-107">Properties</span></span>
|<span data-ttu-id="107bc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="107bc-108">Property</span></span>|<span data-ttu-id="107bc-109">型</span><span class="sxs-lookup"><span data-stu-id="107bc-109">Type</span></span>|<span data-ttu-id="107bc-110">説明</span><span class="sxs-lookup"><span data-stu-id="107bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="107bc-111">displayName</span><span class="sxs-lookup"><span data-stu-id="107bc-111">displayName</span></span>|<span data-ttu-id="107bc-112">String</span><span class="sxs-lookup"><span data-stu-id="107bc-112">String</span></span>|<span data-ttu-id="107bc-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="107bc-113">App display name.</span></span> <span data-ttu-id="107bc-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="107bc-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="107bc-115">説明</span><span class="sxs-lookup"><span data-stu-id="107bc-115">description</span></span>|<span data-ttu-id="107bc-116">String</span><span class="sxs-lookup"><span data-stu-id="107bc-116">String</span></span>|<span data-ttu-id="107bc-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="107bc-117">The app's description.</span></span> <span data-ttu-id="107bc-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="107bc-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="107bc-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="107bc-119">publisherName</span></span>|<span data-ttu-id="107bc-120">String</span><span class="sxs-lookup"><span data-stu-id="107bc-120">String</span></span>|<span data-ttu-id="107bc-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="107bc-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="107bc-122">productName</span><span class="sxs-lookup"><span data-stu-id="107bc-122">productName</span></span>|<span data-ttu-id="107bc-123">String</span><span class="sxs-lookup"><span data-stu-id="107bc-123">String</span></span>|<span data-ttu-id="107bc-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="107bc-124">The product name.</span></span> <span data-ttu-id="107bc-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="107bc-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="107bc-126">denied</span><span class="sxs-lookup"><span data-stu-id="107bc-126">denied</span></span>|<span data-ttu-id="107bc-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="107bc-127">Boolean</span></span>|<span data-ttu-id="107bc-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="107bc-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="107bc-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="107bc-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="107bc-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="107bc-130">binaryName</span></span>|<span data-ttu-id="107bc-131">String</span><span class="sxs-lookup"><span data-stu-id="107bc-131">String</span></span>|<span data-ttu-id="107bc-132">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="107bc-132">The binary name.</span></span>|
|<span data-ttu-id="107bc-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="107bc-133">binaryVersionLow</span></span>|<span data-ttu-id="107bc-134">String</span><span class="sxs-lookup"><span data-stu-id="107bc-134">String</span></span>|<span data-ttu-id="107bc-135">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="107bc-135">The lower binary version.</span></span>|
|<span data-ttu-id="107bc-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="107bc-136">binaryVersionHigh</span></span>|<span data-ttu-id="107bc-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="107bc-137">String</span></span>|<span data-ttu-id="107bc-138">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="107bc-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="107bc-139">関係</span><span class="sxs-lookup"><span data-stu-id="107bc-139">Relationships</span></span>
<span data-ttu-id="107bc-140">なし</span><span class="sxs-lookup"><span data-stu-id="107bc-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="107bc-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="107bc-141">JSON Representation</span></span>
<span data-ttu-id="107bc-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="107bc-142">Here is a JSON representation of the resource.</span></span>
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



