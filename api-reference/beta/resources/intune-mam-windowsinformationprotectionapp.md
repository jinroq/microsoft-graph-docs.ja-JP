---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
ms.openlocfilehash: 6f5bf2cd42ba2df96f3e9cc2b9b1c1954420c572
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073452"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="81bfa-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81bfa-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="81bfa-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81bfa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81bfa-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81bfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81bfa-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81bfa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81bfa-107">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="81bfa-107">App for Windows information protection</span></span>
## <a name="properties"></a><span data-ttu-id="81bfa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bfa-108">Properties</span></span>
|<span data-ttu-id="81bfa-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81bfa-109">Property</span></span>|<span data-ttu-id="81bfa-110">型</span><span class="sxs-lookup"><span data-stu-id="81bfa-110">Type</span></span>|<span data-ttu-id="81bfa-111">説明</span><span class="sxs-lookup"><span data-stu-id="81bfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81bfa-112">displayName</span><span class="sxs-lookup"><span data-stu-id="81bfa-112">displayName</span></span>|<span data-ttu-id="81bfa-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bfa-113">String</span></span>|<span data-ttu-id="81bfa-114">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="81bfa-114">App display name.</span></span>|
|<span data-ttu-id="81bfa-115">説明</span><span class="sxs-lookup"><span data-stu-id="81bfa-115">description</span></span>|<span data-ttu-id="81bfa-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bfa-116">String</span></span>|<span data-ttu-id="81bfa-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="81bfa-117">The app's description.</span></span>|
|<span data-ttu-id="81bfa-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="81bfa-118">publisherName</span></span>|<span data-ttu-id="81bfa-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bfa-119">String</span></span>|<span data-ttu-id="81bfa-120">発行元名</span><span class="sxs-lookup"><span data-stu-id="81bfa-120">The publisher name</span></span>|
|<span data-ttu-id="81bfa-121">productName</span><span class="sxs-lookup"><span data-stu-id="81bfa-121">productName</span></span>|<span data-ttu-id="81bfa-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="81bfa-122">String</span></span>|<span data-ttu-id="81bfa-123">製品名。</span><span class="sxs-lookup"><span data-stu-id="81bfa-123">The product name.</span></span>|
|<span data-ttu-id="81bfa-124">denied</span><span class="sxs-lookup"><span data-stu-id="81bfa-124">denied</span></span>|<span data-ttu-id="81bfa-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="81bfa-125">Boolean</span></span>|<span data-ttu-id="81bfa-126">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="81bfa-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81bfa-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81bfa-127">Relationships</span></span>
<span data-ttu-id="81bfa-128">なし</span><span class="sxs-lookup"><span data-stu-id="81bfa-128">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81bfa-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81bfa-129">JSON Representation</span></span>
<span data-ttu-id="81bfa-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81bfa-130">Here is a JSON representation of the resource.</span></span>
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





