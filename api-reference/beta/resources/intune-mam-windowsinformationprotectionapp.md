---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 61ada685166fbe3ca7ef02fa8f87e5383666e9ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967906"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="2c0c6-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2c0c6-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="2c0c6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2c0c6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c0c6-106">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="2c0c6-106">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="2c0c6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c0c6-107">Properties</span></span>
|<span data-ttu-id="2c0c6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2c0c6-108">Property</span></span>|<span data-ttu-id="2c0c6-109">型</span><span class="sxs-lookup"><span data-stu-id="2c0c6-109">Type</span></span>|<span data-ttu-id="2c0c6-110">説明</span><span class="sxs-lookup"><span data-stu-id="2c0c6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c0c6-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2c0c6-111">displayName</span></span>|<span data-ttu-id="2c0c6-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2c0c6-112">String</span></span>|<span data-ttu-id="2c0c6-113">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-113">App display name.</span></span>|
|<span data-ttu-id="2c0c6-114">description</span><span class="sxs-lookup"><span data-stu-id="2c0c6-114">description</span></span>|<span data-ttu-id="2c0c6-115">String</span><span class="sxs-lookup"><span data-stu-id="2c0c6-115">String</span></span>|<span data-ttu-id="2c0c6-116">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-116">The app's description.</span></span>|
|<span data-ttu-id="2c0c6-117">publisherName</span><span class="sxs-lookup"><span data-stu-id="2c0c6-117">publisherName</span></span>|<span data-ttu-id="2c0c6-118">String</span><span class="sxs-lookup"><span data-stu-id="2c0c6-118">String</span></span>|<span data-ttu-id="2c0c6-119">発行元名</span><span class="sxs-lookup"><span data-stu-id="2c0c6-119">The publisher name</span></span>|
|<span data-ttu-id="2c0c6-120">productName</span><span class="sxs-lookup"><span data-stu-id="2c0c6-120">productName</span></span>|<span data-ttu-id="2c0c6-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2c0c6-121">String</span></span>|<span data-ttu-id="2c0c6-122">製品名。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-122">The product name.</span></span>|
|<span data-ttu-id="2c0c6-123">denied</span><span class="sxs-lookup"><span data-stu-id="2c0c6-123">denied</span></span>|<span data-ttu-id="2c0c6-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2c0c6-124">Boolean</span></span>|<span data-ttu-id="2c0c6-125">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-125">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c0c6-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2c0c6-126">Relationships</span></span>
<span data-ttu-id="2c0c6-127">なし</span><span class="sxs-lookup"><span data-stu-id="2c0c6-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c0c6-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2c0c6-128">JSON Representation</span></span>
<span data-ttu-id="2c0c6-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2c0c6-129">Here is a JSON representation of the resource.</span></span>
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





