---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03d8adbbf43b38bfc7d13bec2db09c2be8c3b2ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868972"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="b7f41-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7f41-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="b7f41-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b7f41-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7f41-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7f41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7f41-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b7f41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7f41-107">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7f41-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="b7f41-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7f41-108">Properties</span></span>
|<span data-ttu-id="b7f41-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7f41-109">Property</span></span>|<span data-ttu-id="b7f41-110">種類</span><span class="sxs-lookup"><span data-stu-id="b7f41-110">Type</span></span>|<span data-ttu-id="b7f41-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7f41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f41-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="b7f41-112">encryptionKey</span></span>|<span data-ttu-id="b7f41-113">Binary</span><span class="sxs-lookup"><span data-stu-id="b7f41-113">Binary</span></span>|<span data-ttu-id="b7f41-114">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="b7f41-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="b7f41-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="b7f41-115">initializationVector</span></span>|<span data-ttu-id="b7f41-116">Binary</span><span class="sxs-lookup"><span data-stu-id="b7f41-116">Binary</span></span>|<span data-ttu-id="b7f41-117">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="b7f41-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="b7f41-118">Mac</span><span class="sxs-lookup"><span data-stu-id="b7f41-118">mac</span></span>|<span data-ttu-id="b7f41-119">Binary</span><span class="sxs-lookup"><span data-stu-id="b7f41-119">Binary</span></span>|<span data-ttu-id="b7f41-120">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="b7f41-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="b7f41-121">macKey</span><span class="sxs-lookup"><span data-stu-id="b7f41-121">macKey</span></span>|<span data-ttu-id="b7f41-122">Binary</span><span class="sxs-lookup"><span data-stu-id="b7f41-122">Binary</span></span>|<span data-ttu-id="b7f41-123">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="b7f41-123">The key used to get mac.</span></span>|
|<span data-ttu-id="b7f41-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7f41-124">profileIdentifier</span></span>|<span data-ttu-id="b7f41-125">String</span><span class="sxs-lookup"><span data-stu-id="b7f41-125">String</span></span>|<span data-ttu-id="b7f41-126">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="b7f41-126">The the profile identifier.</span></span>|
|<span data-ttu-id="b7f41-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="b7f41-127">fileDigest</span></span>|<span data-ttu-id="b7f41-128">Binary</span><span class="sxs-lookup"><span data-stu-id="b7f41-128">Binary</span></span>|<span data-ttu-id="b7f41-129">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="b7f41-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="b7f41-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b7f41-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="b7f41-131">String</span><span class="sxs-lookup"><span data-stu-id="b7f41-131">String</span></span>|<span data-ttu-id="b7f41-132">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="b7f41-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7f41-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7f41-133">Relationships</span></span>
<span data-ttu-id="b7f41-134">なし</span><span class="sxs-lookup"><span data-stu-id="b7f41-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7f41-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7f41-135">JSON Representation</span></span>
<span data-ttu-id="b7f41-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7f41-136">Here is a JSON representation of the resource.</span></span>
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





