---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e90f46aea713feffb9e64f798779991f20507519
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940583"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="32912-103">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32912-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="32912-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32912-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32912-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32912-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32912-106">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="32912-106">Desktop App for Windows information protection</span></span>


<span data-ttu-id="32912-107">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32912-107">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="32912-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32912-108">Properties</span></span>
|<span data-ttu-id="32912-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32912-109">Property</span></span>|<span data-ttu-id="32912-110">型</span><span class="sxs-lookup"><span data-stu-id="32912-110">Type</span></span>|<span data-ttu-id="32912-111">説明</span><span class="sxs-lookup"><span data-stu-id="32912-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32912-112">displayName</span><span class="sxs-lookup"><span data-stu-id="32912-112">displayName</span></span>|<span data-ttu-id="32912-113">文字列</span><span class="sxs-lookup"><span data-stu-id="32912-113">String</span></span>|<span data-ttu-id="32912-114">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="32912-114">App display name.</span></span> <span data-ttu-id="32912-115">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32912-115">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="32912-116">description</span><span class="sxs-lookup"><span data-stu-id="32912-116">description</span></span>|<span data-ttu-id="32912-117">String</span><span class="sxs-lookup"><span data-stu-id="32912-117">String</span></span>|<span data-ttu-id="32912-118">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="32912-118">The app's description.</span></span> <span data-ttu-id="32912-119">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32912-119">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="32912-120">publisherName</span><span class="sxs-lookup"><span data-stu-id="32912-120">publisherName</span></span>|<span data-ttu-id="32912-121">String</span><span class="sxs-lookup"><span data-stu-id="32912-121">String</span></span>|<span data-ttu-id="32912-122">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="32912-122">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="32912-123">productName</span><span class="sxs-lookup"><span data-stu-id="32912-123">productName</span></span>|<span data-ttu-id="32912-124">String</span><span class="sxs-lookup"><span data-stu-id="32912-124">String</span></span>|<span data-ttu-id="32912-125">製品名。</span><span class="sxs-lookup"><span data-stu-id="32912-125">The product name.</span></span> <span data-ttu-id="32912-126">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32912-126">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="32912-127">denied</span><span class="sxs-lookup"><span data-stu-id="32912-127">denied</span></span>|<span data-ttu-id="32912-128">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="32912-128">Boolean</span></span>|<span data-ttu-id="32912-129">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="32912-129">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="32912-130">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="32912-130">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="32912-131">binaryName</span><span class="sxs-lookup"><span data-stu-id="32912-131">binaryName</span></span>|<span data-ttu-id="32912-132">String</span><span class="sxs-lookup"><span data-stu-id="32912-132">String</span></span>|<span data-ttu-id="32912-133">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="32912-133">The binary name.</span></span>|
|<span data-ttu-id="32912-134">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="32912-134">binaryVersionLow</span></span>|<span data-ttu-id="32912-135">String</span><span class="sxs-lookup"><span data-stu-id="32912-135">String</span></span>|<span data-ttu-id="32912-136">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="32912-136">The lower binary version.</span></span>|
|<span data-ttu-id="32912-137">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="32912-137">binaryVersionHigh</span></span>|<span data-ttu-id="32912-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="32912-138">String</span></span>|<span data-ttu-id="32912-139">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="32912-139">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32912-140">関係</span><span class="sxs-lookup"><span data-stu-id="32912-140">Relationships</span></span>
<span data-ttu-id="32912-141">なし</span><span class="sxs-lookup"><span data-stu-id="32912-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32912-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32912-142">JSON Representation</span></span>
<span data-ttu-id="32912-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32912-143">Here is a JSON representation of the resource.</span></span>
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




