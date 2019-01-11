---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c381541379feacff7611e77882069c5fe2119e67
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822065"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a><span data-ttu-id="56906-103">windowsInformationProtectionDesktopApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56906-103">windowsInformationProtectionDesktopApp resource type</span></span>

> <span data-ttu-id="56906-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56906-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56906-105">Windows 情報保護用デスクトップ アプリ</span><span class="sxs-lookup"><span data-stu-id="56906-105">Desktop App for Windows information protection</span></span>

<span data-ttu-id="56906-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="56906-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="56906-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56906-107">Properties</span></span>
|<span data-ttu-id="56906-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56906-108">Property</span></span>|<span data-ttu-id="56906-109">種類</span><span class="sxs-lookup"><span data-stu-id="56906-109">Type</span></span>|<span data-ttu-id="56906-110">説明</span><span class="sxs-lookup"><span data-stu-id="56906-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56906-111">displayName</span><span class="sxs-lookup"><span data-stu-id="56906-111">displayName</span></span>|<span data-ttu-id="56906-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-112">String</span></span>|<span data-ttu-id="56906-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="56906-113">App display name.</span></span> <span data-ttu-id="56906-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="56906-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="56906-115">説明</span><span class="sxs-lookup"><span data-stu-id="56906-115">description</span></span>|<span data-ttu-id="56906-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-116">String</span></span>|<span data-ttu-id="56906-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="56906-117">The app's description.</span></span> <span data-ttu-id="56906-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="56906-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="56906-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="56906-119">publisherName</span></span>|<span data-ttu-id="56906-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-120">String</span></span>|<span data-ttu-id="56906-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="56906-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="56906-122">productName</span><span class="sxs-lookup"><span data-stu-id="56906-122">productName</span></span>|<span data-ttu-id="56906-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-123">String</span></span>|<span data-ttu-id="56906-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="56906-124">The product name.</span></span> <span data-ttu-id="56906-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="56906-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="56906-126">denied</span><span class="sxs-lookup"><span data-stu-id="56906-126">denied</span></span>|<span data-ttu-id="56906-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="56906-127">Boolean</span></span>|<span data-ttu-id="56906-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="56906-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="56906-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="56906-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="56906-130">binaryName</span><span class="sxs-lookup"><span data-stu-id="56906-130">binaryName</span></span>|<span data-ttu-id="56906-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-131">String</span></span>|<span data-ttu-id="56906-132">バイナリの名前。</span><span class="sxs-lookup"><span data-stu-id="56906-132">The binary name.</span></span>|
|<span data-ttu-id="56906-133">binaryVersionLow</span><span class="sxs-lookup"><span data-stu-id="56906-133">binaryVersionLow</span></span>|<span data-ttu-id="56906-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-134">String</span></span>|<span data-ttu-id="56906-135">下位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="56906-135">The lower binary version.</span></span>|
|<span data-ttu-id="56906-136">binaryVersionHigh</span><span class="sxs-lookup"><span data-stu-id="56906-136">binaryVersionHigh</span></span>|<span data-ttu-id="56906-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="56906-137">String</span></span>|<span data-ttu-id="56906-138">上位のバイナリ バージョン。</span><span class="sxs-lookup"><span data-stu-id="56906-138">The high binary version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56906-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="56906-139">Relationships</span></span>
<span data-ttu-id="56906-140">なし</span><span class="sxs-lookup"><span data-stu-id="56906-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="56906-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56906-141">JSON Representation</span></span>
<span data-ttu-id="56906-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="56906-142">Here is a JSON representation of the resource.</span></span>
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



