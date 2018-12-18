---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: tfitzmac
ms.openlocfilehash: 5164e6d1a9165139de1895dfae38dd8c90927504
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345515"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="e2126-103">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e2126-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="e2126-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2126-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2126-105">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="e2126-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="e2126-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e2126-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e2126-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2126-107">Properties</span></span>
|<span data-ttu-id="e2126-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2126-108">Property</span></span>|<span data-ttu-id="e2126-109">種類</span><span class="sxs-lookup"><span data-stu-id="e2126-109">Type</span></span>|<span data-ttu-id="e2126-110">説明</span><span class="sxs-lookup"><span data-stu-id="e2126-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2126-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e2126-111">displayName</span></span>|<span data-ttu-id="e2126-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-112">String</span></span>|<span data-ttu-id="e2126-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="e2126-113">App display name.</span></span> <span data-ttu-id="e2126-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e2126-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e2126-115">説明</span><span class="sxs-lookup"><span data-stu-id="e2126-115">description</span></span>|<span data-ttu-id="e2126-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-116">String</span></span>|<span data-ttu-id="e2126-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e2126-117">The app's description.</span></span> <span data-ttu-id="e2126-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e2126-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e2126-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="e2126-119">publisherName</span></span>|<span data-ttu-id="e2126-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-120">String</span></span>|<span data-ttu-id="e2126-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="e2126-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e2126-122">productName</span><span class="sxs-lookup"><span data-stu-id="e2126-122">productName</span></span>|<span data-ttu-id="e2126-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-123">String</span></span>|<span data-ttu-id="e2126-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="e2126-124">The product name.</span></span> <span data-ttu-id="e2126-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e2126-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e2126-126">denied</span><span class="sxs-lookup"><span data-stu-id="e2126-126">denied</span></span>|<span data-ttu-id="e2126-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e2126-127">Boolean</span></span>|<span data-ttu-id="e2126-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="e2126-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="e2126-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e2126-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="e2126-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="e2126-130">binaryName</span></span>|<span data-ttu-id="e2126-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-131">String</span></span>|<span data-ttu-id="e2126-132">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="e2126-132">The binary name.</span></span>|
|<span data-ttu-id="e2126-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="e2126-133">binaryVersionLow</span></span>|<span data-ttu-id="e2126-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-134">String</span></span>|<span data-ttu-id="e2126-135">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="e2126-135">The lower binary version.</span></span>|
|<span data-ttu-id="e2126-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="e2126-136">binaryVersionHigh</span></span>|<span data-ttu-id="e2126-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e2126-137">String</span></span>|<span data-ttu-id="e2126-138">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="e2126-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e2126-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e2126-139">Relationships</span></span>
<span data-ttu-id="e2126-140">なし</span><span class="sxs-lookup"><span data-stu-id="e2126-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e2126-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e2126-141">JSON Representation</span></span>
<span data-ttu-id="e2126-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e2126-142">Here is a JSON representation of the resource.</span></span>
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



