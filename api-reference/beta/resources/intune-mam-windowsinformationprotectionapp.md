---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 45d428ee18e92e76f5a13c568373219f904fd886
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403687"
---
# <a name="windowsinformationprotectionapp-resource-type"></a><span data-ttu-id="06992-103">windowsInformationProtectionApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06992-103">windowsInformationProtectionApp resource type</span></span>

> <span data-ttu-id="06992-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06992-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="06992-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06992-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="06992-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06992-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06992-107">Windows 情報保護用アプリ</span><span class="sxs-lookup"><span data-stu-id="06992-107">App for Windows information protection</span></span>

## <a name="properties"></a><span data-ttu-id="06992-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06992-108">Properties</span></span>
|<span data-ttu-id="06992-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06992-109">Property</span></span>|<span data-ttu-id="06992-110">型</span><span class="sxs-lookup"><span data-stu-id="06992-110">Type</span></span>|<span data-ttu-id="06992-111">説明</span><span class="sxs-lookup"><span data-stu-id="06992-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06992-112">displayName</span><span class="sxs-lookup"><span data-stu-id="06992-112">displayName</span></span>|<span data-ttu-id="06992-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="06992-113">String</span></span>|<span data-ttu-id="06992-114">アプリの表示名。</span><span class="sxs-lookup"><span data-stu-id="06992-114">App display name.</span></span>|
|<span data-ttu-id="06992-115">説明</span><span class="sxs-lookup"><span data-stu-id="06992-115">description</span></span>|<span data-ttu-id="06992-116">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="06992-116">String</span></span>|<span data-ttu-id="06992-117">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="06992-117">The app's description.</span></span>|
|<span data-ttu-id="06992-118">publisherName</span><span class="sxs-lookup"><span data-stu-id="06992-118">publisherName</span></span>|<span data-ttu-id="06992-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="06992-119">String</span></span>|<span data-ttu-id="06992-120">発行元名</span><span class="sxs-lookup"><span data-stu-id="06992-120">The publisher name</span></span>|
|<span data-ttu-id="06992-121">productName</span><span class="sxs-lookup"><span data-stu-id="06992-121">productName</span></span>|<span data-ttu-id="06992-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="06992-122">String</span></span>|<span data-ttu-id="06992-123">製品名。</span><span class="sxs-lookup"><span data-stu-id="06992-123">The product name.</span></span>|
|<span data-ttu-id="06992-124">denied</span><span class="sxs-lookup"><span data-stu-id="06992-124">denied</span></span>|<span data-ttu-id="06992-125">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="06992-125">Boolean</span></span>|<span data-ttu-id="06992-126">true の場合、アプリは拒否された保護または除外です。</span><span class="sxs-lookup"><span data-stu-id="06992-126">If true, app is denied protection or exemption.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06992-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="06992-127">Relationships</span></span>
<span data-ttu-id="06992-128">なし</span><span class="sxs-lookup"><span data-stu-id="06992-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06992-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06992-129">JSON Representation</span></span>
<span data-ttu-id="06992-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="06992-130">Here is a JSON representation of the resource.</span></span>
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




