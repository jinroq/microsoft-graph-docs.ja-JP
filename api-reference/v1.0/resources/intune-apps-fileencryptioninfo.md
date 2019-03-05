---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66c4fc3c724eecf3a05dae24cb3f6a52de82d059
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255851"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="2e626-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e626-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="2e626-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e626-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e626-105">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2e626-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="2e626-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e626-106">Properties</span></span>
|<span data-ttu-id="2e626-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e626-107">Property</span></span>|<span data-ttu-id="2e626-108">型</span><span class="sxs-lookup"><span data-stu-id="2e626-108">Type</span></span>|<span data-ttu-id="2e626-109">説明</span><span class="sxs-lookup"><span data-stu-id="2e626-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e626-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="2e626-110">encryptionKey</span></span>|<span data-ttu-id="2e626-111">Binary</span><span class="sxs-lookup"><span data-stu-id="2e626-111">Binary</span></span>|<span data-ttu-id="2e626-112">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="2e626-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="2e626-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="2e626-113">initializationVector</span></span>|<span data-ttu-id="2e626-114">Binary</span><span class="sxs-lookup"><span data-stu-id="2e626-114">Binary</span></span>|<span data-ttu-id="2e626-115">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="2e626-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="2e626-116">Mac</span><span class="sxs-lookup"><span data-stu-id="2e626-116">mac</span></span>|<span data-ttu-id="2e626-117">Binary</span><span class="sxs-lookup"><span data-stu-id="2e626-117">Binary</span></span>|<span data-ttu-id="2e626-118">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="2e626-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="2e626-119">macKey</span><span class="sxs-lookup"><span data-stu-id="2e626-119">macKey</span></span>|<span data-ttu-id="2e626-120">Binary</span><span class="sxs-lookup"><span data-stu-id="2e626-120">Binary</span></span>|<span data-ttu-id="2e626-121">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="2e626-121">The key used to get mac.</span></span>|
|<span data-ttu-id="2e626-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="2e626-122">profileIdentifier</span></span>|<span data-ttu-id="2e626-123">String</span><span class="sxs-lookup"><span data-stu-id="2e626-123">String</span></span>|<span data-ttu-id="2e626-124">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="2e626-124">The the profile identifier.</span></span>|
|<span data-ttu-id="2e626-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="2e626-125">fileDigest</span></span>|<span data-ttu-id="2e626-126">Binary</span><span class="sxs-lookup"><span data-stu-id="2e626-126">Binary</span></span>|<span data-ttu-id="2e626-127">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="2e626-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="2e626-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2e626-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="2e626-129">String</span><span class="sxs-lookup"><span data-stu-id="2e626-129">String</span></span>|<span data-ttu-id="2e626-130">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="2e626-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e626-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e626-131">Relationships</span></span>
<span data-ttu-id="2e626-132">なし</span><span class="sxs-lookup"><span data-stu-id="2e626-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2e626-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e626-133">JSON Representation</span></span>
<span data-ttu-id="2e626-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e626-134">Here is a JSON representation of the resource.</span></span>
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



