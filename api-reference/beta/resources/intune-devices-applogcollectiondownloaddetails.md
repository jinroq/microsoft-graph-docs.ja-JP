---
title: appLogCollectionDownloadDetails リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d4b9ca36f1b9324aac50a808e2ba8fe6db398d4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943194"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="f5b01-103">appLogCollectionDownloadDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5b01-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="f5b01-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5b01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5b01-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5b01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5b01-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f5b01-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f5b01-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b01-107">Properties</span></span>
|<span data-ttu-id="f5b01-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5b01-108">Property</span></span>|<span data-ttu-id="f5b01-109">型</span><span class="sxs-lookup"><span data-stu-id="f5b01-109">Type</span></span>|<span data-ttu-id="f5b01-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5b01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5b01-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="f5b01-111">downloadUrl</span></span>|<span data-ttu-id="f5b01-112">String</span><span class="sxs-lookup"><span data-stu-id="f5b01-112">String</span></span>|<span data-ttu-id="f5b01-113">完成した、完了した処理のための SAS Url をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="f5b01-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="f5b01-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="f5b01-114">decryptionKey</span></span>|<span data-ttu-id="f5b01-115">String</span><span class="sxs-lookup"><span data-stu-id="f5b01-115">String</span></span>|<span data-ttu-id="f5b01-116">DecryptionKey as string</span><span class="sxs-lookup"><span data-stu-id="f5b01-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="f5b01-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f5b01-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="f5b01-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f5b01-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="f5b01-119">コンテンツの DecryptionAlgorithm。</span><span class="sxs-lookup"><span data-stu-id="f5b01-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="f5b01-120">可能な値は`aes256`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f5b01-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5b01-121">関係</span><span class="sxs-lookup"><span data-stu-id="f5b01-121">Relationships</span></span>
<span data-ttu-id="f5b01-122">なし</span><span class="sxs-lookup"><span data-stu-id="f5b01-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5b01-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5b01-123">JSON Representation</span></span>
<span data-ttu-id="f5b01-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5b01-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```




