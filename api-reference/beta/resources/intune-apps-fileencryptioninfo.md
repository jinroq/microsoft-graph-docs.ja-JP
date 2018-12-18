---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: a13c451193d248d09e020cc6b308b9f03d991295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307855"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="bfb87-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bfb87-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="bfb87-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bfb87-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfb87-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfb87-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bfb87-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bfb87-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bfb87-107">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bfb87-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="bfb87-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfb87-108">Properties</span></span>
|<span data-ttu-id="bfb87-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bfb87-109">Property</span></span>|<span data-ttu-id="bfb87-110">種類</span><span class="sxs-lookup"><span data-stu-id="bfb87-110">Type</span></span>|<span data-ttu-id="bfb87-111">説明</span><span class="sxs-lookup"><span data-stu-id="bfb87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfb87-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="bfb87-112">encryptionKey</span></span>|<span data-ttu-id="bfb87-113">Binary</span><span class="sxs-lookup"><span data-stu-id="bfb87-113">Binary</span></span>|<span data-ttu-id="bfb87-114">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="bfb87-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="bfb87-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="bfb87-115">initializationVector</span></span>|<span data-ttu-id="bfb87-116">Binary</span><span class="sxs-lookup"><span data-stu-id="bfb87-116">Binary</span></span>|<span data-ttu-id="bfb87-117">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="bfb87-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="bfb87-118">Mac</span><span class="sxs-lookup"><span data-stu-id="bfb87-118">mac</span></span>|<span data-ttu-id="bfb87-119">Binary</span><span class="sxs-lookup"><span data-stu-id="bfb87-119">Binary</span></span>|<span data-ttu-id="bfb87-120">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="bfb87-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="bfb87-121">macKey</span><span class="sxs-lookup"><span data-stu-id="bfb87-121">macKey</span></span>|<span data-ttu-id="bfb87-122">Binary</span><span class="sxs-lookup"><span data-stu-id="bfb87-122">Binary</span></span>|<span data-ttu-id="bfb87-123">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="bfb87-123">The key used to get mac.</span></span>|
|<span data-ttu-id="bfb87-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="bfb87-124">profileIdentifier</span></span>|<span data-ttu-id="bfb87-125">String</span><span class="sxs-lookup"><span data-stu-id="bfb87-125">String</span></span>|<span data-ttu-id="bfb87-126">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="bfb87-126">The the profile identifier.</span></span>|
|<span data-ttu-id="bfb87-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="bfb87-127">fileDigest</span></span>|<span data-ttu-id="bfb87-128">Binary</span><span class="sxs-lookup"><span data-stu-id="bfb87-128">Binary</span></span>|<span data-ttu-id="bfb87-129">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="bfb87-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="bfb87-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="bfb87-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="bfb87-131">String</span><span class="sxs-lookup"><span data-stu-id="bfb87-131">String</span></span>|<span data-ttu-id="bfb87-132">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="bfb87-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bfb87-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bfb87-133">Relationships</span></span>
<span data-ttu-id="bfb87-134">なし</span><span class="sxs-lookup"><span data-stu-id="bfb87-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bfb87-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bfb87-135">JSON Representation</span></span>
<span data-ttu-id="bfb87-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bfb87-136">Here is a JSON representation of the resource.</span></span>
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





