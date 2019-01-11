---
title: fileEncryptionInfo リソースの種類
description: ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed56f695da8dece64702472cd3822603e02dd8b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840692"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="d37b0-103">fileEncryptionInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d37b0-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="d37b0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d37b0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d37b0-105">ビジネス アプリの行のコンテンツ バージョンのファイル暗号化情報のプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d37b0-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="d37b0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d37b0-106">Properties</span></span>
|<span data-ttu-id="d37b0-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d37b0-107">Property</span></span>|<span data-ttu-id="d37b0-108">種類</span><span class="sxs-lookup"><span data-stu-id="d37b0-108">Type</span></span>|<span data-ttu-id="d37b0-109">説明</span><span class="sxs-lookup"><span data-stu-id="d37b0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37b0-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="d37b0-110">encryptionKey</span></span>|<span data-ttu-id="d37b0-111">Binary</span><span class="sxs-lookup"><span data-stu-id="d37b0-111">Binary</span></span>|<span data-ttu-id="d37b0-112">ファイルのコンテンツを暗号化するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="d37b0-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="d37b0-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="d37b0-113">initializationVector</span></span>|<span data-ttu-id="d37b0-114">Binary</span><span class="sxs-lookup"><span data-stu-id="d37b0-114">Binary</span></span>|<span data-ttu-id="d37b0-115">暗号化アルゴリズムに使用される初期化ベクトルです。</span><span class="sxs-lookup"><span data-stu-id="d37b0-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="d37b0-116">Mac</span><span class="sxs-lookup"><span data-stu-id="d37b0-116">mac</span></span>|<span data-ttu-id="d37b0-117">Binary</span><span class="sxs-lookup"><span data-stu-id="d37b0-117">Binary</span></span>|<span data-ttu-id="d37b0-118">暗号化されたファイル コンテンツのハッシュ + IV (コンテンツ ハッシュ) です。</span><span class="sxs-lookup"><span data-stu-id="d37b0-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="d37b0-119">macKey</span><span class="sxs-lookup"><span data-stu-id="d37b0-119">macKey</span></span>|<span data-ttu-id="d37b0-120">Binary</span><span class="sxs-lookup"><span data-stu-id="d37b0-120">Binary</span></span>|<span data-ttu-id="d37b0-121">Mac を取得するために使用するキーです。</span><span class="sxs-lookup"><span data-stu-id="d37b0-121">The key used to get mac.</span></span>|
|<span data-ttu-id="d37b0-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="d37b0-122">profileIdentifier</span></span>|<span data-ttu-id="d37b0-123">String</span><span class="sxs-lookup"><span data-stu-id="d37b0-123">String</span></span>|<span data-ttu-id="d37b0-124">プロファイルの識別子です。</span><span class="sxs-lookup"><span data-stu-id="d37b0-124">The the profile identifier.</span></span>|
|<span data-ttu-id="d37b0-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="d37b0-125">fileDigest</span></span>|<span data-ttu-id="d37b0-126">Binary</span><span class="sxs-lookup"><span data-stu-id="d37b0-126">Binary</span></span>|<span data-ttu-id="d37b0-127">暗号化される前のファイル ダイジェストです。</span><span class="sxs-lookup"><span data-stu-id="d37b0-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="d37b0-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="d37b0-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="d37b0-129">String</span><span class="sxs-lookup"><span data-stu-id="d37b0-129">String</span></span>|<span data-ttu-id="d37b0-130">ファイル ダイジェストのアルゴリズムです。</span><span class="sxs-lookup"><span data-stu-id="d37b0-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d37b0-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d37b0-131">Relationships</span></span>
<span data-ttu-id="d37b0-132">なし</span><span class="sxs-lookup"><span data-stu-id="d37b0-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d37b0-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d37b0-133">JSON Representation</span></span>
<span data-ttu-id="d37b0-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d37b0-134">Here is a JSON representation of the resource.</span></span>
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



