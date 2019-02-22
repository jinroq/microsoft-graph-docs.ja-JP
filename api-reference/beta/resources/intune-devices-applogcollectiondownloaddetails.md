---
title: appLogCollectionDownloadDetails リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3449e1f1a2b8651cea407690019d458d5ac24fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147755"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="1d1ec-103">appLogCollectionDownloadDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d1ec-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="1d1ec-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d1ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d1ec-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d1ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d1ec-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1d1ec-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1d1ec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d1ec-107">Properties</span></span>
|<span data-ttu-id="1d1ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d1ec-108">Property</span></span>|<span data-ttu-id="1d1ec-109">型</span><span class="sxs-lookup"><span data-stu-id="1d1ec-109">Type</span></span>|<span data-ttu-id="1d1ec-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d1ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d1ec-111">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="1d1ec-111">downloadUrl</span></span>|<span data-ttu-id="1d1ec-112">String</span><span class="sxs-lookup"><span data-stu-id="1d1ec-112">String</span></span>|<span data-ttu-id="1d1ec-113">完成した、完了した処理のための SAS Url をダウンロードする</span><span class="sxs-lookup"><span data-stu-id="1d1ec-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="1d1ec-114">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="1d1ec-114">decryptionKey</span></span>|<span data-ttu-id="1d1ec-115">String</span><span class="sxs-lookup"><span data-stu-id="1d1ec-115">String</span></span>|<span data-ttu-id="1d1ec-116">DecryptionKey as string</span><span class="sxs-lookup"><span data-stu-id="1d1ec-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="1d1ec-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1d1ec-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="1d1ec-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="1d1ec-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="1d1ec-119">コンテンツの DecryptionAlgorithm。</span><span class="sxs-lookup"><span data-stu-id="1d1ec-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="1d1ec-120">可能な値は`aes256`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1d1ec-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d1ec-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1d1ec-121">Relationships</span></span>
<span data-ttu-id="1d1ec-122">なし</span><span class="sxs-lookup"><span data-stu-id="1d1ec-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d1ec-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d1ec-123">JSON Representation</span></span>
<span data-ttu-id="1d1ec-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d1ec-124">Here is a JSON representation of the resource.</span></span>
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




