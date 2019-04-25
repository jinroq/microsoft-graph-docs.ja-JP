---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2236e2c63703ea5af2662d5b0f4594e7888799
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552178"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="163c2-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="163c2-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="163c2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="163c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="163c2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="163c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="163c2-106">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="163c2-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="163c2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="163c2-107">Properties</span></span>
|<span data-ttu-id="163c2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="163c2-108">Property</span></span>|<span data-ttu-id="163c2-109">型</span><span class="sxs-lookup"><span data-stu-id="163c2-109">Type</span></span>|<span data-ttu-id="163c2-110">説明</span><span class="sxs-lookup"><span data-stu-id="163c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="163c2-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="163c2-111">encryptionKey</span></span>|<span data-ttu-id="163c2-112">Binary</span><span class="sxs-lookup"><span data-stu-id="163c2-112">Binary</span></span>|<span data-ttu-id="163c2-113">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="163c2-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="163c2-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="163c2-114">initializationVector</span></span>|<span data-ttu-id="163c2-115">Binary</span><span class="sxs-lookup"><span data-stu-id="163c2-115">Binary</span></span>|<span data-ttu-id="163c2-116">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="163c2-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="163c2-117">Mac</span><span class="sxs-lookup"><span data-stu-id="163c2-117">mac</span></span>|<span data-ttu-id="163c2-118">Binary</span><span class="sxs-lookup"><span data-stu-id="163c2-118">Binary</span></span>|<span data-ttu-id="163c2-119">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="163c2-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="163c2-120">macKey</span><span class="sxs-lookup"><span data-stu-id="163c2-120">macKey</span></span>|<span data-ttu-id="163c2-121">Binary</span><span class="sxs-lookup"><span data-stu-id="163c2-121">Binary</span></span>|<span data-ttu-id="163c2-122">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="163c2-122">The key used to get mac.</span></span>|
|<span data-ttu-id="163c2-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="163c2-123">profileIdentifier</span></span>|<span data-ttu-id="163c2-124">String</span><span class="sxs-lookup"><span data-stu-id="163c2-124">String</span></span>|<span data-ttu-id="163c2-125">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="163c2-125">The the profile identifier.</span></span>|
|<span data-ttu-id="163c2-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="163c2-126">fileDigest</span></span>|<span data-ttu-id="163c2-127">Binary</span><span class="sxs-lookup"><span data-stu-id="163c2-127">Binary</span></span>|<span data-ttu-id="163c2-128">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="163c2-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="163c2-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="163c2-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="163c2-130">String</span><span class="sxs-lookup"><span data-stu-id="163c2-130">String</span></span>|<span data-ttu-id="163c2-131">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="163c2-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="163c2-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="163c2-132">Relationships</span></span>
<span data-ttu-id="163c2-133">なし</span><span class="sxs-lookup"><span data-stu-id="163c2-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="163c2-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="163c2-134">JSON Representation</span></span>
<span data-ttu-id="163c2-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="163c2-135">Here is a JSON representation of the resource.</span></span>
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





