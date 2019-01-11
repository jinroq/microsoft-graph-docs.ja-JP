---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 250542a7ff87b02ee271c0fbb8682f9855cc24ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833937"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="ec7c9-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec7c9-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="ec7c9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec7c9-105">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="ec7c9-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="ec7c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec7c9-106">Properties</span></span>
|<span data-ttu-id="ec7c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec7c9-107">Property</span></span>|<span data-ttu-id="ec7c9-108">種類</span><span class="sxs-lookup"><span data-stu-id="ec7c9-108">Type</span></span>|<span data-ttu-id="ec7c9-109">説明</span><span class="sxs-lookup"><span data-stu-id="ec7c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec7c9-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ec7c9-110">displayName</span></span>|<span data-ttu-id="ec7c9-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ec7c9-111">String</span></span>|<span data-ttu-id="ec7c9-112">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-112">App display name.</span></span>|
|<span data-ttu-id="ec7c9-113">説明</span><span class="sxs-lookup"><span data-stu-id="ec7c9-113">description</span></span>|<span data-ttu-id="ec7c9-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ec7c9-114">String</span></span>|<span data-ttu-id="ec7c9-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-115">The app's description.</span></span>|
|<span data-ttu-id="ec7c9-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="ec7c9-116">publisherName</span></span>|<span data-ttu-id="ec7c9-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ec7c9-117">String</span></span>|<span data-ttu-id="ec7c9-118">発行元名</span><span class="sxs-lookup"><span data-stu-id="ec7c9-118">The publisher name</span></span>|
|<span data-ttu-id="ec7c9-119">productName</span><span class="sxs-lookup"><span data-stu-id="ec7c9-119">productName</span></span>|<span data-ttu-id="ec7c9-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ec7c9-120">String</span></span>|<span data-ttu-id="ec7c9-121">製品名。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-121">The product name.</span></span>|
|<span data-ttu-id="ec7c9-122">denied</span><span class="sxs-lookup"><span data-stu-id="ec7c9-122">denied</span></span>|<span data-ttu-id="ec7c9-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ec7c9-123">Boolean</span></span>|<span data-ttu-id="ec7c9-124">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec7c9-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec7c9-125">Relationships</span></span>
<span data-ttu-id="ec7c9-126">なし</span><span class="sxs-lookup"><span data-stu-id="ec7c9-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ec7c9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec7c9-127">JSON Representation</span></span>
<span data-ttu-id="ec7c9-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ec7c9-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



