---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 270dd0b6328cd8290e656e46a0ff40551d2a5cbf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917798"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="b0e08-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0e08-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="b0e08-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b0e08-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0e08-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0e08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0e08-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0e08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0e08-107">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="b0e08-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="b0e08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0e08-108">Properties</span></span>
|<span data-ttu-id="b0e08-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0e08-109">Property</span></span>|<span data-ttu-id="b0e08-110">種類</span><span class="sxs-lookup"><span data-stu-id="b0e08-110">Type</span></span>|<span data-ttu-id="b0e08-111">説明</span><span class="sxs-lookup"><span data-stu-id="b0e08-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0e08-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b0e08-112">displayName</span></span>|<span data-ttu-id="b0e08-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0e08-113">String</span></span>|<span data-ttu-id="b0e08-114">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="b0e08-114">App display name.</span></span>|
|<span data-ttu-id="b0e08-115">説明</span><span class="sxs-lookup"><span data-stu-id="b0e08-115">description</span></span>|<span data-ttu-id="b0e08-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0e08-116">String</span></span>|<span data-ttu-id="b0e08-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b0e08-117">The app's description.</span></span>|
|<span data-ttu-id="b0e08-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="b0e08-118">publisherName</span></span>|<span data-ttu-id="b0e08-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0e08-119">String</span></span>|<span data-ttu-id="b0e08-120">発行元名</span><span class="sxs-lookup"><span data-stu-id="b0e08-120">The publisher name</span></span>|
|<span data-ttu-id="b0e08-121">productName</span><span class="sxs-lookup"><span data-stu-id="b0e08-121">productName</span></span>|<span data-ttu-id="b0e08-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b0e08-122">String</span></span>|<span data-ttu-id="b0e08-123">製品名。</span><span class="sxs-lookup"><span data-stu-id="b0e08-123">The product name.</span></span>|
|<span data-ttu-id="b0e08-124">denied</span><span class="sxs-lookup"><span data-stu-id="b0e08-124">denied</span></span>|<span data-ttu-id="b0e08-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b0e08-125">Boolean</span></span>|<span data-ttu-id="b0e08-126">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="b0e08-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0e08-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0e08-127">Relationships</span></span>
<span data-ttu-id="b0e08-128">なし</span><span class="sxs-lookup"><span data-stu-id="b0e08-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b0e08-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0e08-129">JSON Representation</span></span>
<span data-ttu-id="b0e08-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0e08-130">Here is a JSON representation of the resource.</span></span>
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





