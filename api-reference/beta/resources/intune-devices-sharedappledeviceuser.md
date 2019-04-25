---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43bc64243cb330f0761c8ded3ab646a0cde4f926
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526113"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="e8f46-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8f46-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="e8f46-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8f46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8f46-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8f46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8f46-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e8f46-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e8f46-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f46-107">Properties</span></span>
|<span data-ttu-id="e8f46-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8f46-108">Property</span></span>|<span data-ttu-id="e8f46-109">型</span><span class="sxs-lookup"><span data-stu-id="e8f46-109">Type</span></span>|<span data-ttu-id="e8f46-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8f46-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8f46-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e8f46-111">userPrincipalName</span></span>|<span data-ttu-id="e8f46-112">String</span><span class="sxs-lookup"><span data-stu-id="e8f46-112">String</span></span>|<span data-ttu-id="e8f46-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="e8f46-113">User name</span></span>|
|<span data-ttu-id="e8f46-114">datatosync</span><span class="sxs-lookup"><span data-stu-id="e8f46-114">dataToSync</span></span>|<span data-ttu-id="e8f46-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="e8f46-115">Boolean</span></span>|<span data-ttu-id="e8f46-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="e8f46-116">Data to sync</span></span>|
|<span data-ttu-id="e8f46-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="e8f46-117">dataQuota</span></span>|<span data-ttu-id="e8f46-118">Int64</span><span class="sxs-lookup"><span data-stu-id="e8f46-118">Int64</span></span>|<span data-ttu-id="e8f46-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="e8f46-119">Data quota</span></span>|
|<span data-ttu-id="e8f46-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="e8f46-120">dataUsed</span></span>|<span data-ttu-id="e8f46-121">Int64</span><span class="sxs-lookup"><span data-stu-id="e8f46-121">Int64</span></span>|<span data-ttu-id="e8f46-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="e8f46-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8f46-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8f46-123">Relationships</span></span>
<span data-ttu-id="e8f46-124">なし</span><span class="sxs-lookup"><span data-stu-id="e8f46-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8f46-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8f46-125">JSON Representation</span></span>
<span data-ttu-id="e8f46-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8f46-126">Here is a JSON representation of the resource.</span></span>
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





