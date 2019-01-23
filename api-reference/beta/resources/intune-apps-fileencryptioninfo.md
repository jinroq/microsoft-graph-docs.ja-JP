---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 074bf24638bf0ba7d613399e1b8894de7f30dfbb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410897"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="63405-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63405-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="63405-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="63405-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="63405-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63405-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63405-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63405-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63405-107">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="63405-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="63405-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63405-108">Properties</span></span>
|<span data-ttu-id="63405-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63405-109">Property</span></span>|<span data-ttu-id="63405-110">型</span><span class="sxs-lookup"><span data-stu-id="63405-110">Type</span></span>|<span data-ttu-id="63405-111">説明</span><span class="sxs-lookup"><span data-stu-id="63405-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63405-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="63405-112">encryptionKey</span></span>|<span data-ttu-id="63405-113">Binary</span><span class="sxs-lookup"><span data-stu-id="63405-113">Binary</span></span>|<span data-ttu-id="63405-114">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="63405-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="63405-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="63405-115">initializationVector</span></span>|<span data-ttu-id="63405-116">Binary</span><span class="sxs-lookup"><span data-stu-id="63405-116">Binary</span></span>|<span data-ttu-id="63405-117">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="63405-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="63405-118">Mac</span><span class="sxs-lookup"><span data-stu-id="63405-118">mac</span></span>|<span data-ttu-id="63405-119">Binary</span><span class="sxs-lookup"><span data-stu-id="63405-119">Binary</span></span>|<span data-ttu-id="63405-120">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="63405-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="63405-121">macKey</span><span class="sxs-lookup"><span data-stu-id="63405-121">macKey</span></span>|<span data-ttu-id="63405-122">Binary</span><span class="sxs-lookup"><span data-stu-id="63405-122">Binary</span></span>|<span data-ttu-id="63405-123">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="63405-123">The key used to get mac.</span></span>|
|<span data-ttu-id="63405-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="63405-124">profileIdentifier</span></span>|<span data-ttu-id="63405-125">String</span><span class="sxs-lookup"><span data-stu-id="63405-125">String</span></span>|<span data-ttu-id="63405-126">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="63405-126">The the profile identifier.</span></span>|
|<span data-ttu-id="63405-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="63405-127">fileDigest</span></span>|<span data-ttu-id="63405-128">Binary</span><span class="sxs-lookup"><span data-stu-id="63405-128">Binary</span></span>|<span data-ttu-id="63405-129">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="63405-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="63405-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="63405-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="63405-131">String</span><span class="sxs-lookup"><span data-stu-id="63405-131">String</span></span>|<span data-ttu-id="63405-132">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="63405-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63405-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="63405-133">Relationships</span></span>
<span data-ttu-id="63405-134">なし</span><span class="sxs-lookup"><span data-stu-id="63405-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63405-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63405-135">JSON Representation</span></span>
<span data-ttu-id="63405-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="63405-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```




