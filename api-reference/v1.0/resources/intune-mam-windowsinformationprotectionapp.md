---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 32dd1213bb06fbaa80a744d78453b12f6eeff7dd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037759"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="b7d1d-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7d1d-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="b7d1d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7d1d-105">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="b7d1d-105">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="b7d1d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7d1d-106">Properties</span></span>
|<span data-ttu-id="b7d1d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7d1d-107">Property</span></span>|<span data-ttu-id="b7d1d-108">型</span><span class="sxs-lookup"><span data-stu-id="b7d1d-108">Type</span></span>|<span data-ttu-id="b7d1d-109">説明</span><span class="sxs-lookup"><span data-stu-id="b7d1d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7d1d-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b7d1d-110">displayName</span></span>|<span data-ttu-id="b7d1d-111">文字列</span><span class="sxs-lookup"><span data-stu-id="b7d1d-111">String</span></span>|<span data-ttu-id="b7d1d-112">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-112">App display name.</span></span>|
|<span data-ttu-id="b7d1d-113">description</span><span class="sxs-lookup"><span data-stu-id="b7d1d-113">description</span></span>|<span data-ttu-id="b7d1d-114">String</span><span class="sxs-lookup"><span data-stu-id="b7d1d-114">String</span></span>|<span data-ttu-id="b7d1d-115">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-115">The app's description.</span></span>|
|<span data-ttu-id="b7d1d-116">publisherName</span><span class="sxs-lookup"><span data-stu-id="b7d1d-116">publisherName</span></span>|<span data-ttu-id="b7d1d-117">String</span><span class="sxs-lookup"><span data-stu-id="b7d1d-117">String</span></span>|<span data-ttu-id="b7d1d-118">発行元名</span><span class="sxs-lookup"><span data-stu-id="b7d1d-118">The publisher name</span></span>|
|<span data-ttu-id="b7d1d-119">productName</span><span class="sxs-lookup"><span data-stu-id="b7d1d-119">productName</span></span>|<span data-ttu-id="b7d1d-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b7d1d-120">String</span></span>|<span data-ttu-id="b7d1d-121">製品名。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-121">The product name.</span></span>|
|<span data-ttu-id="b7d1d-122">denied</span><span class="sxs-lookup"><span data-stu-id="b7d1d-122">denied</span></span>|<span data-ttu-id="b7d1d-123">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="b7d1d-123">Boolean</span></span>|<span data-ttu-id="b7d1d-124">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-124">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7d1d-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7d1d-125">Relationships</span></span>
<span data-ttu-id="b7d1d-126">なし</span><span class="sxs-lookup"><span data-stu-id="b7d1d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7d1d-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7d1d-127">JSON Representation</span></span>
<span data-ttu-id="b7d1d-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7d1d-128">Here is a JSON representation of the resource.</span></span>
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



