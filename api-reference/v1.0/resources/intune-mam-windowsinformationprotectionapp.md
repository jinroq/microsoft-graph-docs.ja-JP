---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d025b20e5341c17f756e86bb6bb84faf92a61a3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971880"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="7d43b-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d43b-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="7d43b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7d43b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d43b-105">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="7d43b-105">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="7d43b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d43b-106">Properties</span></span>
|<span data-ttu-id="7d43b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d43b-107">Property</span></span>|<span data-ttu-id="7d43b-108">種類</span><span class="sxs-lookup"><span data-stu-id="7d43b-108">Type</span></span>|<span data-ttu-id="7d43b-109">説明</span><span class="sxs-lookup"><span data-stu-id="7d43b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d43b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="7d43b-110">displayName</span></span>|<span data-ttu-id="7d43b-111">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d43b-111">String</span></span>|<span data-ttu-id="7d43b-112">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="7d43b-112">App display name.</span></span>|
|<span data-ttu-id="7d43b-113">説明</span><span class="sxs-lookup"><span data-stu-id="7d43b-113">description</span></span>|<span data-ttu-id="7d43b-114">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d43b-114">String</span></span>|<span data-ttu-id="7d43b-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7d43b-115">The app's description.</span></span>|
|<span data-ttu-id="7d43b-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="7d43b-116">publisherName</span></span>|<span data-ttu-id="7d43b-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d43b-117">String</span></span>|<span data-ttu-id="7d43b-118">発行元名</span><span class="sxs-lookup"><span data-stu-id="7d43b-118">The publisher name</span></span>|
|<span data-ttu-id="7d43b-119">productName</span><span class="sxs-lookup"><span data-stu-id="7d43b-119">productName</span></span>|<span data-ttu-id="7d43b-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7d43b-120">String</span></span>|<span data-ttu-id="7d43b-121">製品名。</span><span class="sxs-lookup"><span data-stu-id="7d43b-121">The product name.</span></span>|
|<span data-ttu-id="7d43b-122">denied</span><span class="sxs-lookup"><span data-stu-id="7d43b-122">denied</span></span>|<span data-ttu-id="7d43b-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="7d43b-123">Boolean</span></span>|<span data-ttu-id="7d43b-124">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="7d43b-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d43b-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7d43b-125">Relationships</span></span>
<span data-ttu-id="7d43b-126">なし</span><span class="sxs-lookup"><span data-stu-id="7d43b-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d43b-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d43b-127">JSON Representation</span></span>
<span data-ttu-id="7d43b-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7d43b-128">Here is a JSON representation of the resource.</span></span>
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



