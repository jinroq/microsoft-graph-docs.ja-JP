---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4e78aa854b15763cade9a4d6020f1737bbca1642
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814477"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="557c4-103">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="557c4-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="557c4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="557c4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="557c4-105">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="557c4-105">Store App for Windows information protection</span></span>

<span data-ttu-id="557c4-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="557c4-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="557c4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="557c4-107">Properties</span></span>
|<span data-ttu-id="557c4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="557c4-108">Property</span></span>|<span data-ttu-id="557c4-109">種類</span><span class="sxs-lookup"><span data-stu-id="557c4-109">Type</span></span>|<span data-ttu-id="557c4-110">説明</span><span class="sxs-lookup"><span data-stu-id="557c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="557c4-111">displayName</span><span class="sxs-lookup"><span data-stu-id="557c4-111">displayName</span></span>|<span data-ttu-id="557c4-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="557c4-112">String</span></span>|<span data-ttu-id="557c4-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="557c4-113">App display name.</span></span> <span data-ttu-id="557c4-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="557c4-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="557c4-115">説明</span><span class="sxs-lookup"><span data-stu-id="557c4-115">description</span></span>|<span data-ttu-id="557c4-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="557c4-116">String</span></span>|<span data-ttu-id="557c4-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="557c4-117">The app's description.</span></span> <span data-ttu-id="557c4-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="557c4-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="557c4-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="557c4-119">publisherName</span></span>|<span data-ttu-id="557c4-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="557c4-120">String</span></span>|<span data-ttu-id="557c4-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="557c4-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="557c4-122">productName</span><span class="sxs-lookup"><span data-stu-id="557c4-122">productName</span></span>|<span data-ttu-id="557c4-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="557c4-123">String</span></span>|<span data-ttu-id="557c4-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="557c4-124">The product name.</span></span> <span data-ttu-id="557c4-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="557c4-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="557c4-126">denied</span><span class="sxs-lookup"><span data-stu-id="557c4-126">denied</span></span>|<span data-ttu-id="557c4-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="557c4-127">Boolean</span></span>|<span data-ttu-id="557c4-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="557c4-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="557c4-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="557c4-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="557c4-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="557c4-130">Relationships</span></span>
<span data-ttu-id="557c4-131">なし</span><span class="sxs-lookup"><span data-stu-id="557c4-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="557c4-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="557c4-132">JSON Representation</span></span>
<span data-ttu-id="557c4-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="557c4-133">Here is a JSON representation of the resource.</span></span>
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



