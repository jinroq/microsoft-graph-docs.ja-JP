---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c375b0c380cc719c8f49ba683a580133835e3a75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968163"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="77cb8-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="77cb8-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="77cb8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77cb8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77cb8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77cb8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77cb8-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="77cb8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="77cb8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cb8-107">Properties</span></span>
|<span data-ttu-id="77cb8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77cb8-108">Property</span></span>|<span data-ttu-id="77cb8-109">型</span><span class="sxs-lookup"><span data-stu-id="77cb8-109">Type</span></span>|<span data-ttu-id="77cb8-110">説明</span><span class="sxs-lookup"><span data-stu-id="77cb8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77cb8-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="77cb8-111">userPrincipalName</span></span>|<span data-ttu-id="77cb8-112">String</span><span class="sxs-lookup"><span data-stu-id="77cb8-112">String</span></span>|<span data-ttu-id="77cb8-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="77cb8-113">User name</span></span>|
|<span data-ttu-id="77cb8-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="77cb8-114">dataToSync</span></span>|<span data-ttu-id="77cb8-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="77cb8-115">Boolean</span></span>|<span data-ttu-id="77cb8-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="77cb8-116">Data to sync</span></span>|
|<span data-ttu-id="77cb8-117">dataQuota</span><span class="sxs-lookup"><span data-stu-id="77cb8-117">dataQuota</span></span>|<span data-ttu-id="77cb8-118">Int64</span><span class="sxs-lookup"><span data-stu-id="77cb8-118">Int64</span></span>|<span data-ttu-id="77cb8-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="77cb8-119">Data quota</span></span>|
|<span data-ttu-id="77cb8-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="77cb8-120">dataUsed</span></span>|<span data-ttu-id="77cb8-121">Int64</span><span class="sxs-lookup"><span data-stu-id="77cb8-121">Int64</span></span>|<span data-ttu-id="77cb8-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="77cb8-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="77cb8-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="77cb8-123">Relationships</span></span>
<span data-ttu-id="77cb8-124">なし</span><span class="sxs-lookup"><span data-stu-id="77cb8-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77cb8-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77cb8-125">JSON Representation</span></span>
<span data-ttu-id="77cb8-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="77cb8-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedAppleDeviceUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedAppleDeviceUser",
  "userPrincipalName": "String",
  "dataToSync": true,
  "dataQuota": 1024,
  "dataUsed": 1024
}
```





