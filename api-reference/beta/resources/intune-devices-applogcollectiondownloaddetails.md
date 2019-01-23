---
title: appLogCollectionDownloadDetails リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6946b3cd1aa60c4025859bd8d41d2dc4775bf39d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430244"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="8cdda-103">appLogCollectionDownloadDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cdda-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="8cdda-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cdda-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8cdda-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cdda-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cdda-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cdda-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cdda-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8cdda-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8cdda-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdda-108">Properties</span></span>
|<span data-ttu-id="8cdda-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdda-109">Property</span></span>|<span data-ttu-id="8cdda-110">型</span><span class="sxs-lookup"><span data-stu-id="8cdda-110">Type</span></span>|<span data-ttu-id="8cdda-111">説明</span><span class="sxs-lookup"><span data-stu-id="8cdda-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cdda-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="8cdda-112">downloadUrl</span></span>|<span data-ttu-id="8cdda-113">String</span><span class="sxs-lookup"><span data-stu-id="8cdda-113">String</span></span>|<span data-ttu-id="8cdda-114">完了した AppLogUploadRequest の SA の Url をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="8cdda-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="8cdda-115">するアプリレーション</span><span class="sxs-lookup"><span data-stu-id="8cdda-115">decryptionKey</span></span>|<span data-ttu-id="8cdda-116">String</span><span class="sxs-lookup"><span data-stu-id="8cdda-116">String</span></span>|<span data-ttu-id="8cdda-117">文字列とするアプリレーション</span><span class="sxs-lookup"><span data-stu-id="8cdda-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="8cdda-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8cdda-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="8cdda-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="8cdda-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="8cdda-120">コンテンツの DecryptionAlgorithm です。</span><span class="sxs-lookup"><span data-stu-id="8cdda-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="8cdda-121">使用可能な値: `aes256`。</span><span class="sxs-lookup"><span data-stu-id="8cdda-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cdda-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8cdda-122">Relationships</span></span>
<span data-ttu-id="8cdda-123">なし</span><span class="sxs-lookup"><span data-stu-id="8cdda-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cdda-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cdda-124">JSON Representation</span></span>
<span data-ttu-id="8cdda-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8cdda-125">Here is a JSON representation of the resource.</span></span>
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




