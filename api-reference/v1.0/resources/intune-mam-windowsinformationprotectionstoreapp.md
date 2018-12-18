---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
ms.openlocfilehash: b5f13b77a5fbd9464ac968034fb19ae4e6327b9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344668"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a><span data-ttu-id="34642-103">windowsInformationProtectionStoreApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="34642-103">windowsInformationProtectionStoreApp resource type</span></span>

> <span data-ttu-id="34642-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="34642-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="34642-105">Windows 情報保護のストア アプリ</span><span class="sxs-lookup"><span data-stu-id="34642-105">Store App for Windows information protection</span></span>

<span data-ttu-id="34642-106">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="34642-106">Inherits from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34642-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34642-107">Properties</span></span>
|<span data-ttu-id="34642-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34642-108">Property</span></span>|<span data-ttu-id="34642-109">種類</span><span class="sxs-lookup"><span data-stu-id="34642-109">Type</span></span>|<span data-ttu-id="34642-110">説明</span><span class="sxs-lookup"><span data-stu-id="34642-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34642-111">displayName</span><span class="sxs-lookup"><span data-stu-id="34642-111">displayName</span></span>|<span data-ttu-id="34642-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34642-112">String</span></span>|<span data-ttu-id="34642-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="34642-113">App display name.</span></span> <span data-ttu-id="34642-114">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="34642-114">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="34642-115">説明</span><span class="sxs-lookup"><span data-stu-id="34642-115">description</span></span>|<span data-ttu-id="34642-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34642-116">String</span></span>|<span data-ttu-id="34642-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="34642-117">The app's description.</span></span> <span data-ttu-id="34642-118">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="34642-118">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="34642-119">publisherName</span><span class="sxs-lookup"><span data-stu-id="34642-119">publisherName</span></span>|<span data-ttu-id="34642-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34642-120">String</span></span>|<span data-ttu-id="34642-121">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名</span><span class="sxs-lookup"><span data-stu-id="34642-121">The publisher name Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="34642-122">productName</span><span class="sxs-lookup"><span data-stu-id="34642-122">productName</span></span>|<span data-ttu-id="34642-123">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="34642-123">String</span></span>|<span data-ttu-id="34642-124">製品名。</span><span class="sxs-lookup"><span data-stu-id="34642-124">The product name.</span></span> <span data-ttu-id="34642-125">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="34642-125">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|
|<span data-ttu-id="34642-126">denied</span><span class="sxs-lookup"><span data-stu-id="34642-126">denied</span></span>|<span data-ttu-id="34642-127">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="34642-127">Boolean</span></span>|<span data-ttu-id="34642-128">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="34642-128">If true, app is denied protection or exemption.</span></span> <span data-ttu-id="34642-129">[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="34642-129">Inherited from [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="34642-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="34642-130">Relationships</span></span>
<span data-ttu-id="34642-131">なし</span><span class="sxs-lookup"><span data-stu-id="34642-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="34642-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="34642-132">JSON Representation</span></span>
<span data-ttu-id="34642-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="34642-133">Here is a JSON representation of the resource.</span></span>
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



