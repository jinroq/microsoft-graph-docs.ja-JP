---
title: sharedAppleDeviceUser リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f737432597d4528d1a682cd15552230af0ae83e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156505"
---
# <a name="sharedappledeviceuser-resource-type"></a><span data-ttu-id="04f1c-103">sharedAppleDeviceUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04f1c-103">sharedAppleDeviceUser resource type</span></span>

> <span data-ttu-id="04f1c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04f1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04f1c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04f1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04f1c-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="04f1c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="04f1c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04f1c-107">Properties</span></span>
|<span data-ttu-id="04f1c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04f1c-108">Property</span></span>|<span data-ttu-id="04f1c-109">型</span><span class="sxs-lookup"><span data-stu-id="04f1c-109">Type</span></span>|<span data-ttu-id="04f1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="04f1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f1c-111">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="04f1c-111">userPrincipalName</span></span>|<span data-ttu-id="04f1c-112">String</span><span class="sxs-lookup"><span data-stu-id="04f1c-112">String</span></span>|<span data-ttu-id="04f1c-113">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="04f1c-113">User name</span></span>|
|<span data-ttu-id="04f1c-114">datatosync</span><span class="sxs-lookup"><span data-stu-id="04f1c-114">dataToSync</span></span>|<span data-ttu-id="04f1c-115">ブール値</span><span class="sxs-lookup"><span data-stu-id="04f1c-115">Boolean</span></span>|<span data-ttu-id="04f1c-116">同期するデータ</span><span class="sxs-lookup"><span data-stu-id="04f1c-116">Data to sync</span></span>|
|<span data-ttu-id="04f1c-117">dataquota</span><span class="sxs-lookup"><span data-stu-id="04f1c-117">dataQuota</span></span>|<span data-ttu-id="04f1c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="04f1c-118">Int64</span></span>|<span data-ttu-id="04f1c-119">データクォータ</span><span class="sxs-lookup"><span data-stu-id="04f1c-119">Data quota</span></span>|
|<span data-ttu-id="04f1c-120">使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="04f1c-120">dataUsed</span></span>|<span data-ttu-id="04f1c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="04f1c-121">Int64</span></span>|<span data-ttu-id="04f1c-122">データクォータ</span><span class="sxs-lookup"><span data-stu-id="04f1c-122">Data quota</span></span>|

## <a name="relationships"></a><span data-ttu-id="04f1c-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04f1c-123">Relationships</span></span>
<span data-ttu-id="04f1c-124">なし</span><span class="sxs-lookup"><span data-stu-id="04f1c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04f1c-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04f1c-125">JSON Representation</span></span>
<span data-ttu-id="04f1c-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04f1c-126">Here is a JSON representation of the resource.</span></span>
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




