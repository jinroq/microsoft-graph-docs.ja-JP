---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e67e76dcec3390f172f4d2819bf7d22ee63f7da5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262546"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="aa778-103">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa778-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="aa778-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aa778-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa778-105">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="aa778-105">Store App for Windows information protection</span></span>


<span data-ttu-id="aa778-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aa778-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="aa778-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa778-107">Properties</span></span>
|<span data-ttu-id="aa778-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa778-108">Property</span></span>|<span data-ttu-id="aa778-109">型</span><span class="sxs-lookup"><span data-stu-id="aa778-109">Type</span></span>|<span data-ttu-id="aa778-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa778-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa778-111">displayName</span><span class="sxs-lookup"><span data-stu-id="aa778-111">displayName</span></span>|<span data-ttu-id="aa778-112">文字列</span><span class="sxs-lookup"><span data-stu-id="aa778-112">String</span></span>|<span data-ttu-id="aa778-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="aa778-113">App display name.</span></span> <span data-ttu-id="aa778-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aa778-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="aa778-115">説明</span><span class="sxs-lookup"><span data-stu-id="aa778-115">description</span></span>|<span data-ttu-id="aa778-116">文字列</span><span class="sxs-lookup"><span data-stu-id="aa778-116">String</span></span>|<span data-ttu-id="aa778-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="aa778-117">The app's description.</span></span> <span data-ttu-id="aa778-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aa778-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="aa778-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="aa778-119">publisherName</span></span>|<span data-ttu-id="aa778-120">String</span><span class="sxs-lookup"><span data-stu-id="aa778-120">String</span></span>|<span data-ttu-id="aa778-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="aa778-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="aa778-122">productName</span><span class="sxs-lookup"><span data-stu-id="aa778-122">productName</span></span>|<span data-ttu-id="aa778-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="aa778-123">String</span></span>|<span data-ttu-id="aa778-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="aa778-124">The product name.</span></span> <span data-ttu-id="aa778-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aa778-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="aa778-126">denied</span><span class="sxs-lookup"><span data-stu-id="aa778-126">denied</span></span>|<span data-ttu-id="aa778-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="aa778-127">Boolean</span></span>|<span data-ttu-id="aa778-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="aa778-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="aa778-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="aa778-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="aa778-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aa778-130">Relationships</span></span>
<span data-ttu-id="aa778-131">なし</span><span class="sxs-lookup"><span data-stu-id="aa778-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aa778-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa778-132">JSON Representation</span></span>
<span data-ttu-id="aa778-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aa778-133">Here is a JSON representation of the resource.</span></span>
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



