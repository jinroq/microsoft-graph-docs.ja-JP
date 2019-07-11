---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 528c68b352f45a4b029a09c37585eda2be540d1a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620200"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f3482-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3482-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f3482-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3482-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3482-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3482-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3482-106">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3482-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f3482-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3482-107">Properties</span></span>
|<span data-ttu-id="f3482-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3482-108">Property</span></span>|<span data-ttu-id="f3482-109">型</span><span class="sxs-lookup"><span data-stu-id="f3482-109">Type</span></span>|<span data-ttu-id="f3482-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3482-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3482-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f3482-111">encryptionKey</span></span>|<span data-ttu-id="f3482-112">Binary</span><span class="sxs-lookup"><span data-stu-id="f3482-112">Binary</span></span>|<span data-ttu-id="f3482-113">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="f3482-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f3482-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f3482-114">initializationVector</span></span>|<span data-ttu-id="f3482-115">Binary</span><span class="sxs-lookup"><span data-stu-id="f3482-115">Binary</span></span>|<span data-ttu-id="f3482-116">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="f3482-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f3482-117">Mac</span><span class="sxs-lookup"><span data-stu-id="f3482-117">mac</span></span>|<span data-ttu-id="f3482-118">Binary</span><span class="sxs-lookup"><span data-stu-id="f3482-118">Binary</span></span>|<span data-ttu-id="f3482-119">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="f3482-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f3482-120">macKey</span><span class="sxs-lookup"><span data-stu-id="f3482-120">macKey</span></span>|<span data-ttu-id="f3482-121">Binary</span><span class="sxs-lookup"><span data-stu-id="f3482-121">Binary</span></span>|<span data-ttu-id="f3482-122">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="f3482-122">The key used to get mac.</span></span>|
|<span data-ttu-id="f3482-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3482-123">profileIdentifier</span></span>|<span data-ttu-id="f3482-124">String</span><span class="sxs-lookup"><span data-stu-id="f3482-124">String</span></span>|<span data-ttu-id="f3482-125">プロファイル識別子。</span><span class="sxs-lookup"><span data-stu-id="f3482-125">The profile identifier.</span></span>|
|<span data-ttu-id="f3482-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f3482-126">fileDigest</span></span>|<span data-ttu-id="f3482-127">Binary</span><span class="sxs-lookup"><span data-stu-id="f3482-127">Binary</span></span>|<span data-ttu-id="f3482-128">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="f3482-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f3482-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f3482-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="f3482-130">String</span><span class="sxs-lookup"><span data-stu-id="f3482-130">String</span></span>|<span data-ttu-id="f3482-131">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="f3482-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3482-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3482-132">Relationships</span></span>
<span data-ttu-id="f3482-133">なし</span><span class="sxs-lookup"><span data-stu-id="f3482-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3482-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3482-134">JSON Representation</span></span>
<span data-ttu-id="f3482-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3482-135">Here is a JSON representation of the resource.</span></span>
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





