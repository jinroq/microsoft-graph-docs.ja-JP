---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6f71e4c6340b7dcf859e71cdf829b257794f443a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372637"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="d2ba7-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2ba7-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="d2ba7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2ba7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2ba7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2ba7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2ba7-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2ba7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d2ba7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-107">Properties</span></span>
|<span data-ttu-id="d2ba7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-108">Property</span></span>|<span data-ttu-id="d2ba7-109">型</span><span class="sxs-lookup"><span data-stu-id="d2ba7-109">Type</span></span>|<span data-ttu-id="d2ba7-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2ba7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ba7-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d2ba7-111">userPrincipalName</span></span>|<span data-ttu-id="d2ba7-112">String</span><span class="sxs-lookup"><span data-stu-id="d2ba7-112">String</span></span>|<span data-ttu-id="d2ba7-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="d2ba7-113">User name</span></span>|
|<span data-ttu-id="d2ba7-114">dataToSync</span><span class="sxs-lookup"><span data-stu-id="d2ba7-114">dataToSync</span></span>|<span data-ttu-id="d2ba7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2ba7-115">Boolean</span></span>|<span data-ttu-id="d2ba7-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-116">Data to sync</span></span>|
|<span data-ttu-id="d2ba7-117">dataQuota</span><span class="sxs-lookup"><span data-stu-id="d2ba7-117">dataQuota</span></span>|<span data-ttu-id="d2ba7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="d2ba7-118">Int64</span></span>|<span data-ttu-id="d2ba7-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-119">Data quota</span></span>|
|<span data-ttu-id="d2ba7-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-120">dataUsed</span></span>|<span data-ttu-id="d2ba7-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d2ba7-121">Int64</span></span>|<span data-ttu-id="d2ba7-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2ba7-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2ba7-123">Relationships</span></span>
<span data-ttu-id="d2ba7-124">なし</span><span class="sxs-lookup"><span data-stu-id="d2ba7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2ba7-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2ba7-125">JSON Representation</span></span>
<span data-ttu-id="d2ba7-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2ba7-126">Here is a JSON representation of the resource.</span></span>
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



